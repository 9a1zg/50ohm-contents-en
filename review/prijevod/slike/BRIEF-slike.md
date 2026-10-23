# Brief: translating one batch of picture descriptions

Read `TRANSLATION.md`, `DECISIONS.md` (section "Picture descriptions") and
`TRANSLATION_GLOSSARY.md` in this repo first. Work alone: no sub-agents,
forks or parallel workers. Do not draft outside the repo; edit the files in
place.

## Your batch

`review/prijevod/slike/serije.json` lists the batches; yours is named in your
assigning prompt. Each entry of `files` is `drawings/N.txt` or `photos/N.txt`
under `contents/`. These are the alt texts / long descriptions of the course
pictures, read by screen-reader users. Only the `.txt` files — never touch the
`.svg`, `.tex`, `.png` or `.jpg` beside them.

## How to translate

- Faithfully and completely: every sentence, nothing added, nothing summarised,
  nothing "corrected" from looking at the picture. You may open the `.tex` (or
  look at the `.svg`/photo) to understand what is meant, so the English uses
  the right technical term.
- Keep the file's structure: the same paragraphs, the same numbering. Section
  labels become `1) Short description:` / `2) Detailed description:`, and
  `Zusammenfassung:` / `Detaillierte Beschreibung:` become `Summary:` /
  `Detailed description:`; other labels likewise, consistently.
- First line `Dieser Alt-Text wurde noch nicht überprüft.` →
  `This alt text has not yet been checked.` A file that is only `TODO` stays.
- Quoted text that is printed on a component or a photo (type numbers,
  makers' markings, "LM7905CT") stays exactly as printed. Quoted labels of a
  drawing that are German words: English, then the German in brackets —
  „Sender“ → "transmitter" ("Sender") — because the drawing still shows the
  German. Symbols and formulas (`f`, `2f`, `U_B`, `R1`) stay as they are.
- English quotation marks "…", decimal point, units as symbols after numbers,
  British spelling with -ise, German technical abbreviations in English
  (NF→AF, HF→RF, ZF→IF, KW→HF, UKW→VHF), glossary terms.
- Every number stays the same number.

## Mechanics

1. Translate every file of your batch in place.
2. Check: `~/projects/50ohm/tools/alttext-check.py $(python3 -c "import json;print(' '.join(next(u['files'] for u in json.load(open('review/prijevod/slike/serije.json')) if u['id']=='<batch>')))")`
   from this repo. It reports numbers that went missing, German words left
   outside quotes and brackets, and files left unchanged. Fix real findings;
   a German word that is legitimately there (a quoted label in brackets, a
   proper name) can stay — say so in your report. A `TODO` file is not
   reported.
3. Write `review/prijevod/slike/<batch>.md`: files translated, files left
   `TODO`, glossary terms added, judgement calls (one line each), suspected
   errors in the German descriptions (file — what — why; translate
   faithfully, do not fix).
4. Commit only your files (`git commit <paths>`; `git status` first), author
   and committer 9A1ZG via env vars, first line `Translate picture
   descriptions: <batch>`, a short body, and the two trailer lines from your
   assigning prompt. Do not push.

## Checker (second agent per batch)

Compare each file's German (`git show <commit>~1:contents/<file>`) with the
English in the working tree: complete, faithful, technically right, natural
British English, glossary and decisions followed, labels handled as above.
Fix in place, run `alttext-check.py --rev <commit>~1 <files>`, append
"## Provjera" to the batch report (counts and one line per substantive
change), commit `Check picture descriptions: <batch>`.
