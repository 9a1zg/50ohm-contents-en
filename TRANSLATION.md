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
  labels in the drawings, which keep them too. That includes word
  subscripts written with `\textrm{}`/`\mathrm{}` (`P_{\textrm{Sender}}`,
  `G_{\textrm{Antenne}}`): they are symbols, used the same way in the course
  text and the drawings, and get translated in one pass together with the
  drawings, never piecemeal. Running words inside `\text{}` (a phrase, not a
  subscript) are translated.
- **Names of German law and institutions:** at first use in a text the
  English name with the German name and abbreviation, e.g. *Amateur Radio
  Ordinance (Amateurfunkverordnung, AFuV)*; afterwards the abbreviation. In
  exam questions, which stand alone, use the form the glossary gives.
- **Call signs, Q codes and international abbreviations** (DL1ABC, QRV, CW,
  SSB) are not translated. **German-only technical abbreviations become their
  English equivalents** in running text: NF → AF, HF → RF, ZF → IF, KW → HF,
  UKW → VHF, EMV → EMC (mind that German HF is English RF, and German KW is
  English HF). Abbreviations of German law and institutions stay (AFuG, AFuV,
  BNetzA, EMVU, BEMFV). Drawings follow the
  same rule (a figure says AF, as the text does).
- **Spelling:** British with *-ise* (authorisation, quantisation), as the RSGB
  writes; *call sign* in two words, as the ITU Radio Regulations do.
- **Exam questions:** `answer_a` is always the correct answer (the generator
  shuffles). A translation must keep it correct and keep b–d wrong, and keep
  the four answers parallel in form. A question stem ending in `…` is
  continued by its answers; keep that working in English.
- **Units after a number: always the symbol**, SI style — `100 Ω`, `4.7 kΩ`,
  `2 mΩ`, also where the German writes the word (`100 Ohm`). The unit *name*
  (*ohm*, *hertz*) only where the unit itself is meant ("Which unit is used
  for impedance? — The ohm"). One answer set never mixes the two.
- **ca. / etwa:** *approx.* / *about*, consistently within an answer set.
- **Address:** German *Sie*/*du* both become plain *you*.
- **Markup:** DARCdown commands, file names, idents and `%` comments are
  never changed (see `README-FORMAT.md`).

## Sources outside this repository

- **Changes to the exam questions** are published by DARC on the AJW
  training-materials page, not only in this repo's history:
  https://www.darc.de/der-club/referate/ajw/ausbildungsunterlagen-n-e-a#c57358.
  Check it when the question bank is brought up to date with upstream, and
  before reporting a suspected question error.

## Tooling (in the `50ohm` workspace repo, shared with the Croatian project)

- `tools/qbank-prevedi.py --content <this repo>` writes translated questions
  and catalogue section titles into `contents/questions/fragenkatalog3b.json`
  (or, with `--file`, another question file such as
  `contents/questions/fragenkatalog_swl.json`) from a batch file, refusing
  anything whose numbers, formulas or markup differ from the German, and
  keeping the file's formatting byte for byte.
- `tools/revizija-guard.py` (with `OHM_HR_CONTENT` pointing here) checks
  structure for the Markdown content.

## Progress

Tracked per batch in `review/prijevod/` (one batch file and one report per
batch) and summarised here as the work goes.

- **Exam questions: done (2026-10-22).** All 1750 questions of
  `contents/questions/fragenkatalog3b.json` in 10 batches
  (`pitanja_01`–`pitanja_10`), each translated and then checked by a second
  pass, followed by a final consistency pass over the whole bank
  (`review/prijevod/zavrsni.md`): units after a number as symbols, late
  glossary terms, identical German with identical English.
- **SWL questions: done (2026-10-23).** The 11 questions and section titles
  of DARC's SWL question set, `contents/questions/fragenkatalog_swl.json`
  (`review/prijevod/swl_pitanja`).
- **Course text: done (2026-10-23).** All 41 units of
  `review/prijevod/tekst/jedinice.json` (sections, slides and worked
  solutions), each translated and then checked by a second pass, plus the
  foreword (`vorwort`), which is in no unit.
- **Static pages: done (2026-10-23).** Tables of contents, static pages,
  snippets and the applets' visible text (unit `toc_static`, translated and
  checked); the course text no longer gives German applet labels in
  brackets, and the applets format numbers with a decimal point.
- **Picture descriptions: done (2026-10-24).** All 1066 (`review/prijevod/
  slike/serije.json`, ten batches), each translated and checked.
- **Drawings: done (2026-10-24).** 375 drawings with printed German text or
  decimal commas translated in their `.tex` and rebuilt (thirteen batches,
  `review/prijevod/slike/crtezi.json`, each checked by eye against the
  original), 57 more rebuilt for decimal points; `latex/` is British.
  Rebuild a drawing with `~/projects/50ohm/tools/darc-drawing.py N`
  (non-default widths in `review/prijevod/slike/sirine.json`). Drawings that
  include a photo missing from the repo (`foto/6` in 689; 671, 690–693, 720
  fail to build for the same reason) need DARC's photo before a rebuild.
