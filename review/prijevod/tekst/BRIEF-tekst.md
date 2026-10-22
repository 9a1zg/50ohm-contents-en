# Brief: translating one unit of the course text

Read `TRANSLATION.md`, `DECISIONS.md` and `TRANSLATION_GLOSSARY.md` in this
repo first; they decide everything this brief does not repeat. The exam
questions are already translated — `[question:XX123]` in the text renders the
English question from the bank, so the prose around it must fit that
question's English wording (look it up in `contents/questions/
fragenkatalog3b.json` when the prose quotes or explains it). Work alone: no
sub-agents, forks or parallel workers.

## Your unit

`review/prijevod/tekst/jedinice.json` lists the units; yours is named in your
assigning prompt. It gives `sections` (translate `contents/sections/<id>.md`
**and** `contents/slides/<id>.md` for each) and `solutions` (translate
`contents/solutions/<number>.md`). A `static` unit is described in its prompt.

## What to translate

All reader-facing text: prose, headings, list items, table cells, slide text,
captions of `[picture:ID:ident:Caption]`, `[photo:…]` and
`[table:ident:Caption]` (only the caption), `[index:Term]` terms, `<qso>`
dialogue, `alt`/`title` text. Translate faithfully and completely — every
sentence, nothing added, nothing summarised. German *du*/*wir* → *you*/*we*.

## What never changes

`[question:…]`, `[ref:…]`, `[include:…]`, picture/photo ids and idents, table
idents, block tags (`<margin>`, `<tip>`, `<indepth>`, `<attention>`,
`<danger>`, `<webonly>`, `<latexonly>`, `<left>`, `<right>`, `<note>`,
`<fragment>`, …) and their position, slide separators `---` and their
attributes, file names, `%` comments, URLs. Formulas: every `$`, every LaTeX
command and every symbol — including German word subscripts like
`P_\mathrm{Sender}` — stay; decimal commas become points (`\qty{3,5}{…}` →
`\qty{3.5}{…}`). Every number stays the same number.

## Conventions worth repeating

- Glossary terms always; a missing term → the RSGB/ITU term, added to the
  glossary. A choice that later units must follow → `DECISIONS.md`.
- German law and institutions as the glossary renders them; at first mention
  in a section the full form ("Amateur Radio Ordinance (Amateurfunkverordnung,
  AFuV)"), afterwards the abbreviation.
- Units after a number: the symbol. Decimal point. British spelling, *-ise*.
- German technical abbreviations → English (NF→AF, HF→RF, ZF→IF, KW→HF,
  UKW→VHF); law abbreviations stay.
- Links to 50ohm.de, darc.de, bundesnetzagentur.de stay as they are.

## Mechanics

1. Translate the files in place.
2. From `~/projects/50ohm`: `OHM_HR_CONTENT=../50ohm-contents-en
   ./tools/revizija-guard.py --brojevi` — it compares your working tree with
   HEAD (the German) and must print `struktura netaknuta`. Fix anything it
   reports (a dropped `$`, a changed number, a lost tag) and run it again.
3. Check nothing German is left: grep your files for common German words
   (`der|die|das|und|ist|nicht|mit|wird|werden|für|bei`) outside formulas,
   URLs and German proper names, and read the hits.
4. Write `review/prijevod/tekst/<unit>.md`: files translated, glossary terms
   added, decisions added, judgement calls (one line each), and suspected
   errors in the German original (file — what — why; translate faithfully,
   do not fix).
5. Commit only your files (`git commit <paths>`; check `git status` first),
   author and committer 9A1ZG via env vars, first line `Translate course text:
   <unit>`, a short body, and the two trailer lines from your assigning
   prompt. Do not push.

## Checker (second agent per unit)

The checker reads the unit commit (`git show <commit> --word-diff=plain` is
useless here — compare `git show <commit>~1:<file>` German with the working
tree English, paragraph by paragraph), and judges: complete (nothing
dropped), faithful, technically right, natural British English, glossary and
decisions followed, prose consistent with the English exam questions it
embeds. It fixes in place, runs `revizija-guard.py --rev <commit>~1
--brojevi`, appends "## Provjera" to the unit report (counts and one line per
substantive change), and commits `Check course text: <unit>`.
