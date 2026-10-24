# crtezi_01 — drawing translation report

29 drawings (`crtezi.json`): 34, 35, 44, 45, 48, 49, 51, 61, 62, 63, 65, 66,
67, 68, 69, 70, 71, 72, 73, 74, 77, 80, 82, 83, 84, 85, 86, 90, 93.
12 translated and rebuilt with `darc-drawing.py` (width 9 cm), 17 with
nothing to translate. Every rebuilt drawing was compared with its original
PNG: same drawing, English text, nothing overlapping or cut off. All sizes
within 2 pt of the originals.

## Per drawing

- 34 — nothing to translate (a–d, `40 m`).
- 35 — nothing to translate (`~ 230 V`, "E", "+"; the `%` comments are
  German, kept).
- 44 — "zum Oszillator" → "to oscillator" (two rotated lines "to" /
  "oscillator"); `\qty{0,3}-\qty{3,4}{\kilo\hertz}` → `0.3`, `3.4`.
- 45 — "Ausgang" → "Output". Terminal letters A, B, C kept.
- 48 — nothing to translate (P, N, ⊕, ⊖).
- 49 — "Metallbeläge" → "Metal foils", "Dielektrikum" → "Dielectric",
  "Wickel" → "Roll".
- 51 — nothing to translate (no printed text).
- 61, 62, 63 — nothing to translate (`0 V`).
- 65 — "Ausgang" → "Output".
- 66 — nothing to translate (`~ 230 V`, ~, +, –, `C_S`).
- 67, 68, 69, 70 — nothing to translate (~, +, –).
- 71, 72, 73, 74 — nothing to translate (+, –).
- 77 — nothing to translate: terminal letters "E" and "A" stay, as the
  glossary decides (§14 row "ZF, NF, … zum Oszillator": "the terminal
  letters E / A stay, like U_E / U_A"); Δφ, VCO unchanged.
- 80 — "HF" → "RF", "Mischer" → "Mixer", "ZF" → "IF"; symbol `f_OSZ` kept.
- 82, 83, 84 — "HF" → "RF", "1.ZF" → "1st IF", "2.ZF" → "2nd IF",
  "NF" → "AF"; VFO, CO, BFO, X, Y, Z kept.
- 85, 86 — "1.\,Filter" → "1st filter", "2.\,Filter" → "2nd filter",
  "HF" → "RF", "Mischer" → "Mixer"; `f_OSZ`, CO, RX, f / 9f kept.
- 90 — "HF" → "RF", "1.ZF" → "1st IF", "2.ZF" → "2nd IF", "NF" → "AF";
  VFO, CO1, CO2 kept.
- 93 — as 90, plus `\qty{9,455}{\mega\hertz}` → `9.455`.

Descriptions (`N.txt`) of the 12 translated drawings: the German brackets
for the translated labels removed ("RF" ("HF") → "RF", "Mixer" ("Mischer")
→ "Mixer", …); quoted labels already matched the new drawings. Nothing else
changed. Drawings with nothing to translate: `.tex`, `.svg`, `.txt` untouched.

## Collisions

None. The longer English labels ("1st filter", "2nd filter", "Output",
"Metal foils", "2nd IF") fit where the German ones were; no wording, line
break or position needed changing.

## Glossary

No rows added: every label is already in §14 (rows for *Wickel /
Metallbeläge / Dielektrikum*, *Mischer / 1.ZF*, *1. Filter / 2. Filter*,
*Ausgang*, *zum Oszillator*, terminal letters E / A).

## Suspected errors in the German drawings

- 90.tex, 93.tex — the last filter, after "2.ZF" (9 MHz), is labelled "NF"
  with "455 kHz" beside it. 455 kHz is a third IF, not AF (compare 913's
  "ZF 455 kHz"; already noted for 90's description in slike_08).
  Translated faithfully as "AF".

## Provjera

29 drawings checked against commit 184a985: 12 translated, 17 with nothing to
translate. 0 changes.

- 44, 45, 49, 65, 80, 82, 83, 84, 85, 86, 90, 93 — `.tex` diffs change only
  printed text (and the decimal commas in 44, 93); wording follows the
  glossary (§14 drawing-label rows, *Ausgang*, *Mischer*, *Dielektrikum*,
  *Metallbeläge*) and the descriptions. Old and new SVGs rendered side by
  side: no German left, nothing overlapping or cut off (93's "9.455 MHz" at
  the bottom edge fits), sizes as the originals. Descriptions lost only the
  German brackets; quoted labels match the drawings.
- 34, 35, 48, 51, 61, 62, 63, 66, 67, 68, 69, 70, 71, 72, 73, 74, 77 —
  rendered: no German printed (letters a–d, E, A, P, N, +, –, ~, `0 V`,
  `230 V`, `C_S`, VCO, Δφ only).
