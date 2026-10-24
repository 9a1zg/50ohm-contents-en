# crtezi_05 — drawing translation report

29 drawings (`crtezi.json`): 443, 446, 470, 471, 474, 475, 486, 488, 495,
496, 499, 501, 503, 504, 505, 506, 541, 542, 556, 559, 563, 590, 591, 592,
593, 594, 607, 609, 610.
14 translated and rebuilt with `darc-drawing.py` (13 at width 9 cm, 471 at
25 cm, see below), 15 with nothing to translate. Every rebuilt drawing was
compared side by side with its original PNG: same drawing, English text,
nothing overlapping or cut off. The untouched ones were rendered from their
SVGs (or, for 609/610, read: SVG path data only): no German printed.

## Per drawing

- 443 — "zum Netzteil" → "to power supply", "zum TX" → "to TX" (new §14
  row, worded like „zum Oszillator“ and as the description already had
  them); "PA" and the digits 1–4 unchanged.
- 446 — nothing to translate ("Z = 50 Ω", "X").
- 470 — decimal commas only: `\qty{2,4}{\giga\hertz}` → 2.4,
  `\qty{0,3}{\milli\watt}` → 0.3. PC, SDR, LNB, DC, G, PTT, "TXCO",
  dBm/mW/W values unchanged.
- 471 — the ten spectrum labels as the §14 row for drawing 847:
  "Höhenstrahlung" → "Cosmic radiation", "Gammastrahlung" → "Gamma
  radiation", "Röntgenstrahlung" → "X-ray radiation", "Ultraviolett" →
  "Ultraviolet", "Licht" → "Light", "Infrarot" → "Infrared",
  "Terahertzstrahlung" → "Terahertz radiation", "Mikrowellenstrahlung" →
  "Microwave radiation", "Funkwellen" → "Radio waves", "Wechselströme" →
  "Alternating currents"; "Radar" unchanged. The `%` comments (Beschriftung,
  Begriffe …) kept.
- 474 — nothing to translate (A, B, C, "…").
- 475 — axis "Leistung" → "Power" (§14 row); `$0{,}3$`, `$2{,}7$` → `$0.3$`,
  `$2.7$`.
- 486 — nothing to translate (P, N, "0 V", "+5 V", ⊕/⊖).
- 488 — `$\mathrm{NF}_\mathrm{IN}$` / `$\mathrm{NF}_\mathrm{OUT}$` →
  `$\mathrm{AF}_\mathrm{IN}$` / `$\mathrm{AF}_\mathrm{OUT}$`,
  `$\mathrm{Audioverstärker}$` → `$\mathrm{Audio\ amplifier}$` (the space
  written `\ ` because the label is set in math mode; §14 row, slike_05).
  V_s, IC_1, R_1, C_1, C_2 and pin numbers unchanged.
- 495 — nothing to translate (digits 1–6, "G").
- 496 — "Antenne" → "Antenna", "HF-Diode" → "RF diode" (§14); "C", "µA"
  unchanged.
- 499 — nothing to translate (only the two "A" meters; the `%` comment
  "Außenmantel" stays).
- 501 — "Netzwerk" → "Network", "Audio (NF) RX" / "Audio (NF) TX" → "Audio
  (AF) RX" / "Audio (AF) TX", "Steuer- und / Kontrollsignale" → "Control
  and / monitoring signals" (§14 row for 501, two lines as in the German).
- 503, 504, 505, 506 — nothing to translate ($U$, $t$).
- 541 — `$\text{Lampe}_1$`, `$\text{Lampe}_2$` → `$\text{Lamp}_1$`,
  `$\text{Lamp}_2$` (§14 row, slike_05).
- 542 — nothing to translate (call signs DB0FZ, DB0HOB, DN9YI and
  "Internet"; the German `%` comments stay).
- 556 — nothing to translate ("10 V", "100 Ω").
- 559 — nothing to translate (B, C, E, $U_\mathrm{BE}$).
- 563 — nothing to translate: `\text{mech.} > \frac{\lambda}{4}` and
  $\lambda/4$; "mech." is the same abbreviation (mechanical) in English, as
  the description already quotes it.
- 590 — "HF" → "RF", "Mischer" → "Mixer", "ZF" → "IF", "NF" → "AF" (§14
  rows „ZF“/„NF“ and „Mischer“, DECISIONS NF→AF, HF→RF); "Demodulator",
  "VFO", "BFO" unchanged ("Demodulator" is the English word as well).
- 591, 592, 593, 594 — axis "Leistung" → "Power" (§14 row).
- 607 — "ZF" → "IF"; $U$, $t$, "X", "+" unchanged.
- 609, 610 — nothing to translate: drawings of coaxial connectors made only
  of SVG paths; the commas the heuristic found are SVG path coordinates
  (`M 38.841674,2.923755`), not decimal commas.

Descriptions (`N.txt`): the German brackets dropped in 443, 475, 488, 496,
501, 541, 590, 591–594, 607. The quoted labels already matched the drawings
("Control and monitoring signals" is the two-line label of 501 read as one,
as the description had it); no other change. 470 and 471 had no German
brackets and are unchanged.

## Width of 471

471 was originally built at 25 cm, not DARC's default 9 cm: at 9 cm the
rebuild came out 286.5 pt wide instead of 707.6 pt. Rebuilt with
`darc-drawing.py --width 25 471`, which reproduces the original size
(707.6 × 211.2 → 707.6 × 211.4 pt). A rebuild of 471 must pass
`--width 25` (there is no `sirine.json` entry for it; that file is outside
this batch's files).

## Collisions

None. The English labels stay clear of everything:
- 471 — the white-boxed labels are about as long as the German ones;
  "Alternating currents", "Microwave radiation" and "Terahertz radiation"
  stay clear of each other, the tick marks and the colour bar.
- 501 — "monitoring signals" is a little wider than "Kontrollsignale" and
  still ends left of the antenna; the drawing gets about 1 pt taller
  (84.9 → 85.9 pt).
- 591–594 — the rotated "Power" box is shorter than "Leistung", so the
  drawings are 246.9 pt wide instead of 255.1 pt (as 250–259 in crtezi_03);
  same drawing at equal width.
- 488 — "Audio amplifier" is shorter than "Audioverstärker"; nothing moves.

## Glossary

One new §14 row: „zum Netzteil“ / „zum TX“ (Zeichnung 443) → "to power
supply" / "to TX". Every other label is already in the glossary (§14
drawing-label rows for „ZF“/„NF“, „Leistung“, „Mischer“, 488/496/541,
501, and the spectrum row for 847).

## Suspected errors

In the German drawings:
- 470.tex — the two oscillator blocks are labelled "TXCO"; the usual
  abbreviation for a temperature-compensated crystal oscillator is TCXO.
  Kept as in the German (the description also says "TXCO").

In DARC's German alt text (left as translated):
- 488.txt — quotes the supply terminal as "V_S"; the drawing prints
  $\mathrm{V}_\mathrm{s}$ with a lower-case s.
- 501.txt — "in three lines" for the texts above the connection; the
  drawing sets them in four lines (the control signals label is broken
  over two).
