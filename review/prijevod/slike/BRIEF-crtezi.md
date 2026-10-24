# Brief: translating one batch of drawings

Read `DECISIONS.md` (sections "Picture descriptions" and "Drawings"),
`TRANSLATION.md` and `TRANSLATION_GLOSSARY.md` in this repo first. Work alone:
no sub-agents, forks or parallel workers. Do not draft outside the repo.

## Your batch

`review/prijevod/slike/crtezi.json` lists the batches; yours is named in your
assigning prompt. For each drawing N: `contents/drawings/N.tex` (the source),
`N.svg` (built from it, never edited by hand) and `N.txt` (its description,
already in English). The list was made by a heuristic (German-looking words
or decimal commas in the `.tex`, or German labels quoted in the
description), so some drawings may have nothing to translate — then leave
them untouched and say so in the report.

## For each drawing

1. Read `N.tex` and translate every piece of text that is printed: node
   texts, labels, axis labels (`xlabel`, `ylabel`), legend entries, tick
   labels written as words, `\text{…}` inside formulas. Change nothing else
   — no coordinates, styles, colours or macros — except the smallest fix
   for a collision (see DECISIONS.md). Keep `%` comments as they are.
   Decimal commas → points. Glossary terms; the wording should match how
   the description (`N.txt`) and the course text name the thing.
2. Build: `~/projects/50ohm/tools/darc-drawing.py --png <tmpdir> N` (run
   from anywhere; one build takes about half a minute; you can pass several
   numbers). Use a new empty directory under your scratchpad for the PNGs.
   A `BUILD FAILED` restores the old SVG; fix the `.tex` and build again.
3. Look at `<tmpdir>/N.png` next to `<tmpdir>/N.orig.png` (Read shows the
   image). Same drawing, English text, nothing overlapping, nothing cut off.
   Fix and rebuild until it is right.
4. Update `N.txt`: remove the German brackets for labels the drawing now
   shows in English, and make the quoted labels match the drawing exactly.
   Nothing else in the description changes.
5. Never touch `latex/`, `src/` or other drawings.

## After the batch

1. Write `review/prijevod/slike/<batch>.md`: per drawing one line — what
   was translated, or "nothing to translate"; collisions and how you fixed
   them; glossary rows added; suspected errors in the German drawing (file
   — what — why; translate faithfully, do not fix).
2. Commit only your files (`git commit <paths>`; `git status` first — the
   `.tex`, `.svg` and `.txt` of your drawings, the report, glossary),
   author and committer 9A1ZG via env vars, first line `Translate drawings:
   <batch>`, a short body, and the two trailer lines from your assigning
   prompt. Do not push.

## Checker (second agent per batch)

For each drawing of the batch: `git show <commit> -- contents/drawings/N.tex`
— only printed text changed (plus any reported collision fix), translation
right and consistent with glossary and description. Render the committed
SVG and the one before (`git show <commit>~1:contents/drawings/N.svg |
rsvg-convert -w 900 -b white -o old.png`; same for the new one) and look at
both: no German left, nothing overlapping or cut off. Also check drawings
reported "nothing to translate" really print no German. Fix in place
(rebuild with `darc-drawing.py`), append "## Provjera" to the batch report
(counts, one line per change), commit `Check drawings: <batch>`.
