# crtezi_02 — drawing translation report

29 drawings (`crtezi.json`): 96, 98, 103, 104, 105, 106, 109, 110, 114, 117,
118, 121, 137, 138, 139, 141, 142, 149, 153, 155, 158, 175, 192, 193, 194,
195, 200, 201, 202.
20 translated and rebuilt with `darc-drawing.py` (width 9 cm), 9 with
nothing to translate. Every rebuilt drawing was compared with its original
PNG (202 also at 2700 px around the cable labels): same drawing, English
text, nothing overlapping or cut off. All sizes within 1.3 pt of the
originals.

## Per drawing

- 96 — "Digitale Signal-" / "verarbeitung" → "Digital signal" /
  "processing" (same two lines).
- 98 — "NF" → "AF", "Balance-" / "modulator" → "Balanced" / "modulator",
  "Mischer" → "Mixer", "Treiber" → "Driver"; CO, VFO, PA, ALC, G, ? kept.
- 103, 104 — nothing to translate (seven-segment digits, "MHz", "X"; the
  decimal point is a segment dot).
- 105 — "Antennen-" / "tuner" → "Antenna" / "tuner"; TX, `15 m`, 1–4 kept.
- 106 — nothing to translate (no printed text).
- 109, 110, 114, 117, 118, 121 — decimal commas only:
  `\qty{-0,4}{V}` → `\qty{-0.4}{V}` and so on (both values in each).
- 137, 138, 139 — nothing to translate: terminal letters "E" / "A" stay
  (glossary §14), `R_1`, `R_2`, `C_1`, `C_2`, +, – unchanged.
- 141 — "ZF" → "IF", "NF" → "AF".
- 142 — "ZF" → "IF"; "X", "+" kept.
- 149 — "ZF=\qty{10,7}{MHz}" → "IF=\qty{10.7}{MHz}", "NF" → "AF",
  `$f_\mathrm{res}\neq \mathrm{ZF}$` → `\mathrm{IF}` (IF is the abbreviation
  here, not a symbol subscript; `f_res` kept).
- 153 — "ZF-Amp." → "IF amp.", "NF" → "AF"; BFO, + kept.
- 155 — "NF/BB" → "AF/BB" (BB = baseband in both languages).
- 158 — "NF/Basisband" → "AF/baseband", "zum Oszillator" → "to oscillator".
- 175, 195, 200 — nothing to translate (`U_E`, `U_A`, IC1, symbols only).
- 192, 193 — "Erde" → "Earth".
- 194 — "Erde" → "Earth"; S, H, E kept.
- 201 — `+\qty{13,8}{\volt}` → `13.8`; IC1, +5 V, `R_L = 10 Ω` unchanged.
- 202 — axis labels "Frequenz [MHz]" → "Frequency [MHz]",
  "Grunddämpfung a_0 je 100 m Leitungslänge in dB" → "Basic attenuation a_0
  per 100 m cable length in dB"; cable labels "PTFE 1.8 mm RG178",
  "Voll-PE" → "Solid PE" (2.8 / 4.95 / 10.3 mm), "PE-Schaum" → "Foam PE"
  (7.3 / 10.3 / 12.7 mm), "PE-Schaum Massivschirm 16,4 mm" → "Foam PE solid
  screen 16.4 mm"; all decimal commas → points. The `%` comments and the
  tick labels (already points) unchanged.

Descriptions (`N.txt`): the German brackets dropped in 96, 105, 141, 142,
149, 153, 155, 158, 192, 193, 202. Quoted labels made to match the drawing
exactly:
- 149 — "f_res  IF" → "f_res ≠ IF" (the ≠ was lost already in DARC's alt
  text, which reads „f_res  ZF“).
- 201 — "+ 13.8 V" → "+13.8 V", "+ 5 V" → "+5 V" (the drawing prints no
  space).
- 202 — "α0" → "a_0" (the drawing prints a Latin a, `\mathrm{a}_0`);
  "Solid PE 2.9 mm RG174" → "2.8 mm"; the foam list "7.3 / 4.9 / 2.7 /
  1.64 mm" and "Foam PE solid screen" → "Foam PE 7.3 mm", "Foam PE 10.3 mm",
  "Foam PE 12.7 mm" and "Foam PE solid screen 16.4 mm", the labels the
  drawing actually carries.
98 and 194 quote none of the translated labels (98 only "CO", 194 only "S",
"E", "H"); their descriptions are unchanged, as are those of the diode
drawings 109–121 (already decimal points) and of the drawings with nothing
to translate.

## Collisions

None. "Balanced", "Antenna", "Digital signal", "IF amp.", "to oscillator"
and the longer 202 labels fit where the German ones were. In 202 the German
"PE-Schaum Massivschirm 16,4 mm" ran across the 12.7 mm line; the shorter
"Foam PE solid screen 16.4 mm" no longer does. No wording, line break or
position changed.

## Glossary

No new rows: every label is in §9 (*Voll-PE / PE-Schaum / Massivschirm*,
*Antennentuner*) or §14 (drawing-label rows for ZF / NF / ZF-Amp. /
NF/Basisband / zum Oszillator, Treiber / Balance-modulator / Digitale
Signalverarbeitung, NF/BB, Frequenz [Hz]), §12 *Erde*. Row
"Grunddämpfung α0 …" (§14) now reads *a_0*, with a note, because the
description now quotes the drawing's Latin a.

## Suspected errors

In the German drawings: none found.

In DARC's German alt text (translated faithfully earlier, now corrected
only where it quotes the drawing's labels):
- 202.txt — quotes „Voll‑PE 2,9 mm RG174“ (drawing: 2,8 mm), the foam cables
  as „4,9 mm“, „2,7 mm“, „1,64 mm“ (drawing: 10,3, 12,7, 16,4 mm) and the
  y-axis symbol as α0 (drawing: a_0); apparently misread from the image.
- 149.txt — „f_res  ZF“ has lost the ≠ that the drawing prints.
