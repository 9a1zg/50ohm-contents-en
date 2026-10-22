# English translation of 50ohm.de — how it is done

This repository is DARC's `50ohm-contents-dl` with its full history, being
translated into English. Remote `upstream` is DARC's GitHub (pull-only);
`origin` is the translator's GitLab. When it is ready it will be published
on GitHub for DARC to take over.

## What this translation is

- **A faithful translation of the German original, for DARC.** Not a
  localisation. The licence classes stay N, E and A; the Bundesnetzagentur,
  the AFuG, the AFuV and every other German rule stay German, because this is
  the German exam in English. Nothing is adapted to another country.
- **British English**, as used in IARU Region 1 and by the RSGB: *licence*
  (noun) / *license* (verb), *metre*, *centre*, *colour*, *programme*,
  *mains*, *earth* (for Erde/Erdung). Terminology in `TRANSLATION_GLOSSARY.md`,
  which is authoritative.
- **Translated from the German.** The Croatian translation
  (`50ohm-contents-hr`) may be consulted as a cross-check, never as a source.
- **Order of work:** the exam question bank first, then the course text
  (sections, slides, solutions), then picture descriptions and the static
  pages.

## Conventions

- **Numbers:** decimal point, not comma — `3,5 MHz` becomes `3.5 MHz`,
  `\qty{29,7}{\mega\hertz}` becomes `\qty{29.7}{\mega\hertz}`. Every number
  stays the same number; the tooling checks this.
- **Formulas and symbols** stay exactly as in the German, including German
  subscripts such as `R_\mathrm{ges}` or `U_\mathrm{eff}`: they match the
  labels in the drawings, which are not translated yet. Only words inside
  `\text{}`/`\textrm{}` are translated.
- **Names of German law and institutions:** at first use in a text the
  English name with the German name and abbreviation, e.g. *Amateur Radio
  Ordinance (Amateurfunkverordnung, AFuV)*; afterwards the abbreviation. In
  exam questions, which stand alone, use the form the glossary gives.
- **Call signs, Q codes, abbreviations** (DL1ABC, QRV, CW, SSB) are not
  translated.
- **Exam questions:** `answer_a` is always the correct answer (the generator
  shuffles). A translation must keep it correct and keep b–d wrong, and keep
  the four answers parallel in form. A question stem ending in `…` is
  continued by its answers; keep that working in English.
- **Address:** German *Sie*/*du* both become plain *you*.
- **Markup:** DARCdown commands, file names, idents and `%` comments are
  never changed (see `README-FORMAT.md`).

## Tooling (in the `50ohm` workspace repo, shared with the Croatian project)

- `tools/qbank-prevedi.py --content <this repo>` writes translated questions
  and catalogue section titles into `contents/questions/fragenkatalog3b.json`
  from a batch file, refusing anything whose numbers, formulas or markup differ
  from the German, and keeping the file's CRLF formatting byte for byte.
- `tools/revizija-guard.py` (with `OHM_HR_CONTENT` pointing here) checks
  structure for the Markdown content.

## Progress

Tracked per batch in `review/prijevod/` (one batch file and one report per
batch) and summarised here as the work goes.
