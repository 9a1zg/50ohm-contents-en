# Brief: translating one batch of exam questions

Read `TRANSLATION.md` and `TRANSLATION_GLOSSARY.md` in this repo first. They
decide everything this brief does not repeat. Work alone: no sub-agents,
forks or parallel workers.

## Your batch

`review/prijevod/serije.json` lists the batches; yours is named in your
assigning prompt (e.g. `pitanja_03`) and holds ~175 question numbers.

Read the German from `contents/questions/fragenkatalog3b.json` with Python
(never open the 17 000-line CRLF file in an editor, never write it yourself).
For each question you translate five fields: `question`, `answer_a` (always
the correct answer), `answer_b`, `answer_c`, `answer_d`. Pictures are
referenced separately and are not part of the text.

## How to translate an exam question

- Faithful and exam-grade: the English must ask exactly what the German asks,
  `answer_a` must stay correct and b–d must stay wrong — no more and no less
  plausible than in German. Keep the four answers parallel in form.
- A stem that ends in "…" is completed by each answer: make every answer read
  as a correct English continuation of the English stem.
- Numbers: identical, decimal point instead of comma (`2,7 kHz` → `2.7 kHz`,
  inside `$…$` too). The tool refuses a field whose numbers changed.
- Formulas: keep every `$`, every LaTeX command and every symbol exactly; only
  words inside `\text{}`/`\textrm{}` are translated. The tool refuses a field
  whose formula structure changed.
- German units written as words (`Ohm`, `Volt`) — keep the unit; in English
  `ohm`/`ohms` in running text, `Ω` is fine where the German uses a symbol.
- German institutions and law: as the glossary gives them. Questions stand
  alone, so do not rely on an abbreviation having been introduced before.
- Terminology: glossary first. If a term is missing, choose the RSGB/ITU term
  and **add it to `TRANSLATION_GLOSSARY.md`** in the right topic section.

## Mechanics

1. Write `review/prijevod/<batch>.json`:
   `{"pitanja": {"AA101": {"question": "...", "answer_a": "...", ...}, ...}}`
   with all five fields for every question in the batch.
2. Dry run, from `~/projects/50ohm`:
   `./tools/qbank-prevedi.py --content ../50ohm-contents-en ../50ohm-contents-en/review/prijevod/<batch>.json`
   It must report 0 refused. Fix and repeat. Read its warnings ("možda njemačke
   riječi") and make sure nothing German is left.
3. Apply: the same with `--apply`.
4. Write `review/prijevod/<batch>.md`: what you added to the glossary, and any
   question where the English needed a judgement call (one line each) — e.g.
   a German pun, a stem/answer structure that does not carry over, a
   suspected error in the German original (note it, translate faithfully).
5. Commit in `~/projects/50ohm-contents-en`, only your files
   (`git commit <paths>`; check `git status` first), author and committer
   9A1ZG via env vars, first line `Translate exam questions: <batch>`, a short
   body, and the two trailer lines from your assigning prompt. Do not push.

## Checker (second agent per batch)

The checker reads `git show <commit>` for the batch, prints every question
German / English side by side with Python, and judges each: meaning
identical? `answer_a` still correct and b–d still wrong? natural British
English? glossary followed? Corrections go into
`review/prijevod/<batch>.provjera.json` (same format, only the fields
changed) and are applied with `--retranslate`. The checker appends a
"## Provjera" section to `<batch>.md` (count checked/changed, one line per
change and why) and commits `Check exam questions: <batch>`.
