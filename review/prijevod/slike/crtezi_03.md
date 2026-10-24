# crtezi_03 — drawing translation report

29 drawings (`crtezi.json`): 203, 204, 250, 251, 252, 253, 257, 258, 259,
263, 264, 266, 268, 278, 279, 280, 281, 282, 283, 284, 285, 286, 287, 288,
289, 290, 291, 292, 293.
26 translated and rebuilt with `darc-drawing.py` (width 9 cm), 3 with
nothing to translate. Every rebuilt drawing was compared with its original
PNG (264 also at 3000 px around the "Directional antenna" label): same
drawing, English text, nothing overlapping or cut off.

## Per drawing

- 203, 204 — "Erde" → "Earth" (as 192–194); E, H, S kept.
- 250, 251, 252, 253, 258, 259 — y-axis "Leistung" → "Power"; `f`,
  "28 MHz" / "29 MHz" / "30 MHz" unchanged.
- 257 — nothing to translate (`f`, `U` only).
- 263 — nothing to translate ("a", "b" only).
- 264 — "Richtantenne" → "Directional antenna", "Dipol" → "Dipole";
  `P_\text{R}`, `P_\text{V}`, `P_\text{D}` kept (symbols); the `%` comments
  ("Bemaßung" etc.) unchanged.
- 266 — decimal commas only: `0{,}4`, `0{,}6`, `0{,}8` → `0.4`, `0.6`,
  `0.8`. The axis option `use comma` was left as it is: every number the
  drawing prints is given explicitly (`xticklabels`, the nodes), so it
  prints nothing and changing it would be a style change.
- 268 — nothing to translate (no printed text).
- 278–293 — decimal commas only in the transistor voltages
  (`+2,0\,V` → `+2.0\,V` and so on; "0 V" unchanged).

Descriptions (`N.txt`): the German brackets dropped in 250, 251, 252, 253,
258, 259 ("Power") and 264 ("Dipole", "Directional antenna"). Quoted labels
made to match the drawing exactly:
- 278 — short description "+2.0" → "+2.0 V" (the drawing prints the unit,
  the detailed description already had it).
203 and 204 quote no "Earth" label (they say "above the ground" in running
text, which is not a quoted label, so unchanged); 266 and 279–293 already
quoted the labels with decimal points. The descriptions write the negative
voltages with "–" where the drawing prints a text hyphen; left as they are
(same sign, typographic only).

## Collisions

None. "Directional antenna" is longer than "Richtantenne" and extends a
little further right than the axis line, as the German label did; it stays
clear of the grey lobe (checked at 3000 px). No wording, line break or
position changed.

Sizes: 264 widens from 256.7 to 259.5 pt (the longer label), so at 9 cm
the drawing is about 1 % smaller; 250–259 go from 255.1 to 246.9 pt wide
(the rotated "Power" box is smaller than "Leistung"); the transistor
drawings 278–293 are about 2 pt lower than the originals. All look the same
side by side at equal width.

## Glossary

No new rows: "Leistung" / "Dipol" / "Richtantenne" are the §14
drawing-label row, *Erde* is §12 (and §4 *Erde (Schaltzeichen)*).

## Suspected errors

In the German drawings: none found. (289 and 293 are identical in DARC's
source — both −2,0 / −5,6 / −2,6 V; not an error in a drawing as such, just
noted.)

In DARC's German alt text:
- 257.txt — the detailed description says the vertical axis is labelled
  „Leistung“ (translated "Power" ("Leistung")), but the drawing prints `U`,
  as the short description correctly says; it also puts the dashed line "in
  the right part" while the short description says "middle part" (the line
  is at the centre). 257 has nothing to translate, so per the brief its
  description was left untouched; the "Power" ("Leistung") quote should
  become "U" when the description is corrected.
