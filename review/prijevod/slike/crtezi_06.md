# crtezi_06 — drawing translation report

29 drawings (`crtezi.json`): 611, 613, 615, 620, 628, 630, 633, 636, 637,
638, 639, 642, 643, 644, 645, 650, 651, 652, 654, 655, 656, 657, 665, 666,
668, 670, 672, 673, 674.
22 translated and rebuilt with `darc-drawing.py` (all at DARC's default
9 cm; sizes within about 1.5 pt of the originals), 7 with nothing to
translate. Every rebuilt drawing was compared side by side with its
original PNG: same drawing, English text, nothing overlapping or cut off.
The untouched ones were rendered from their SVGs: no German printed.

## Per drawing

- 611 — nothing to translate: two coaxial connectors drawn only with
  `\draw svg` paths; no text at all.
- 613 — nothing to translate: Yagi-Uda antenna, lines only (the `%`
  comments are English already).
- 615 — "Anpass-" / "glied" (two lines above and below the block) →
  "Matching" / "network" (§14 row „Anpassglied“, 615). `% Anpassglied:`
  comment kept.
- 620 — nothing to translate: the meter prints "V"; battery, resistor, LED.
- 628 — axis labels "Feldstärke" → "Field strength" (§3), "Ort" →
  "Position" (§14 *Ort (Achsenbeschriftung einer Momentaufnahme)*, as the
  funkwellen text says "position"); "1", "2" unchanged.
- 630 — "Netzwerk" → "Network" (§14 row 501), "CAT-" / "Interface" → "CAT" /
  "interface" (§6 *CAT-Schnittstelle*), "Digimode-" / "Interface" (twice) →
  "Data mode" / "interface" (§14 *Digimode-Interface*). The line breaks stay
  where the German had them; the German hyphens go because the English is
  two words. Audio, USB, CAT, PTT unchanged; the German `%` comments stay.
- 633 — "Dipolschenkel 1" / "Dipolschenkel 2" → "Dipole leg 1" / "Dipole
  leg 2" (§14 row 633). The currents and the formula unchanged; the
  commented-out pins (Koaxialkabel, Abschirmung, Innenleiter) are `%`
  comments and stay.
- 636, 637, 638, 639 — "Kanaldecodierer" → "Channel decoder",
  "Quellendecodierer" → "Source decoder" (§14 *Quellencodierer / …
  Quellendecodierer*), "FPGA oder Software" → "FPGA or software" (§14 row
  636–645). "De-Mapper" and the bit labels unchanged. The `~` padding in
  front of the first label of 638 and 639 kept.
- 642, 643, 644, 645 — "Quellencodierer" → "Source encoder",
  "Kanalcodierer" → "Channel encoder" (same §14 row), "FPGA oder Software"
  → "FPGA or software"; "Mapper" unchanged. The `~` padding after the last
  label of 644 and 645 kept.
- 650 — nothing to translate: `\text{mech.}~\frac{5}{8}\lambda` and
  λ/4; "mech." reads the same in English (as 563 in crtezi_05, and the
  description already quotes "mech. 5/8 λ").
- 651 — decimal commas only: `\qty{2,4}{\giga\hertz}` → 2.4,
  `\qty{2,256}{\giga\hertz}` → 2.256. "144 MHz", "10 MHz", "TCXO", "PLL",
  "G", "Ext. GPSDO" unchanged.
- 652 — nothing to translate ("IQ", "G", "?", the A/D and D/A letters of
  the converter shapes).
- 654 — "Präfix" → "Prefix" (§1, §14 row 654); "Numeral", "Suffix" and the
  call sign letters unchanged.
- 655 — "Durchlass-" / "bereich" → "Passband" (one word, so on one line),
  "Sperrbereich" → "Stopband" (§14 row 400–411). Tick labels and `f`, `A`
  unchanged. The pgfplots option `/pgf/number format/use comma` was left
  as it is (a style option, which the brief says not to touch): the plot
  prints no number through it, its tick labels are written out and the
  y-ticks are empty.
- 656 — nothing to translate: map of Europe with country prefixes only
  (DL, F, OZ, 9A, …).
- 657 — "Kabel" → "Cable", "Antenne" → "Antenna" (§14 row 439/430/45);
  "Transceiver" unchanged.
- 665 — "1. Ziffer" → "1st digit", "2. Ziffer" → "2nd digit",
  "Multiplikator" → "Multiplier", "Toleranz" → "Tolerance" (§14 row 665).
- 666 — "Kathode" → "Cathode" (§4 *Anode / Kathode*). "Anode" unchanged.
  The small letters "node" and "athode", which turn the drawn "A" and "K"
  into *Anode* / *Kathode*, kept exactly as printed (as the slike_06
  report decided for the description; the course text explains the aid
  with "the letters A and K, the usual symbols for anode and cathode").
- 668 — nothing to translate ("Remote", "Internet", "DL1FLO"; German `%`
  comments stay).
- 670 — "SWR-Meter" → "SWR meter", "Antenne" → "Antenna", "Vorlaufend" →
  "Forward", "Reflektiert" → "Reflected" (§14 row 670/657/633);
  "Transceiver" unchanged.
- 672 — `\qty{28,410}` / `\qty{28,415}` → 28.410 / 28.415; "begehrte" /
  "Station" → "Sought-after" / "station", "Antwort-" / "Frequenz" →
  "Reply" / "frequency" (§14 row 672/673), line breaks as in the German.
- 673 — `\qty{28,410}` / `28,420` / `28,430` → points; "begehrte" /
  "Station" → "Sought-after" / "station", "Antwort-" / "bereich" → "Reply" /
  "range" (same row).
- 674 — "Sender" → "Transmitter", "Empfänger" → "Receiver" (§14 row 741),
  "Kanal" (the text argument of `\AsymCloud`) → "Channel" (§6).

Descriptions (`N.txt`): the German brackets dropped in 615, 628, 630, 633,
636–639, 642–645, 654, 655, 657, 665, 666, 670, 672, 673, 674. The quoted
labels match the drawings (labels set on two lines quoted as one, as
before: "Matching network", "Data mode interface", "Sought-after station",
"Reply frequency", "Reply range"). One change beyond the brackets, because
the brief asks the quoted labels to match the drawing exactly: in 642–645
the descriptions called the blocks "Source decoder" ("Quellendecodierer")
and "Channel decoder" ("Kanaldecodierer"), while the drawings print the
encoders (see slike_06, "Suspected errors"); they now quote "Source
encoder" and "Channel encoder". In 630, row 5 keeps its wording `a "Data
mode" interface` (the quoted part is printed as it stands). 651 had no
German brackets ("2.4 GHz", "2.256 GHz" already with points) and is
unchanged, as are the seven drawings with nothing to translate.

## Collisions

None. The English labels stay clear of everything:
- 636–645 — "Source decoder" / "Source encoder" are shorter and "Channel
  encoder" a little longer than the German; the labels stay inside the
  dashed frame and clear of the blocks. Drawings 0.1 pt taller.
- 674 — "Channel" ends clear of the lightning symbol in the cloud;
  "Transmitter" is a little wider than "Sender" and the drawing 0.5 pt
  wider (265.3 → 265.9 pt).
- 628 — "Position" stays below the axis, clear of the curve's last descent.
- 630 — "Data mode" fits the interface boxes as "Digimode-" did.
- 655 — "Passband" on one line sits where the two German lines were.

## Glossary

No new rows: every label is already in the glossary (§1 *Präfix*, §3
*Feldstärke*, §4 *Anode / Kathode*, §6 *CAT-Schnittstelle*, *Kanal*; §14
rows *Ort*, *Quellencodierer … Quellendecodierer*, *Digimode-Interface*,
and the drawing-label rows for 615, 501 („Netzwerk“), 400–411, 439/430/45,
633/657/670, 636–645/654, 665, 672/673, 741). The note of the §14 row *Ort
(Achsenbeschriftung einer Momentaufnahme)*, "the drawing keeps "Ort" until
the drawings are done", now says that drawing 628 prints "Position" (it
was the only drawing printing „Ort“).

## Suspected errors

In the German drawings: none found.

In DARC's German alt text (left as translated, except 642–645 above):
- 620.txt — already reported in slike_06: the detailed description has a
  meter labelled "A" for an ammeter; the drawing prints "V" (a voltmeter),
  as the short description says. Not changed: the drawing has nothing to
  translate, and the error is not in a translated label.
- 633.txt — "voltmeter with an AC symbol" between outer and inner conductor
  (both descriptions): `633.tex` draws `sV`, a sinusoidal voltage source
  (circle with a sine wave), not a meter. Translated as written.
- 642–645.txt — "Quellendecodierer" / "Kanaldecodierer" for the encoder
  blocks (slike_06); the quoted labels now follow the drawings.

## Provjera

29 drawings checked against commit d2835e4: 22 translated, 7 with nothing
to translate. 0 changes.

- 615, 628, 630, 633, 636–639, 642–645, 651, 654, 655, 657, 665, 666, 670,
  672–674 — `.tex` diffs change only printed text and the decimal commas
  (no coordinates, styles, options, padding `~` or `%` comments touched;
  655's `use comma` option prints no number, its tick labels are written
  out). Wording follows the glossary (§1 *Präfix*, §3 *Feldstärke*, §4
  *Kathode*, §6 *CAT-Schnittstelle*, *Kanal*; §14 rows *Ort*,
  *Quellencodierer … Quellendecodierer*, *Digimode-Interface*,
  *Dipolschenkel*, *Anpassglied*, *Multiplikator (Farbcode)* and the
  drawing-label rows for 400–411, 633/657/670, 636–645/654, 665, 672/673,
  741). Old and new SVGs rendered side by side: no German left, nothing
  overlapping or cut off (636–645's labels inside the dashed frame and
  clear of the blocks; 674's "Transmitter" inside the drawing, "Channel"
  clear of the lightning; 655's one-line "Passband" clear of the curve;
  672's two-line labels clear of the ticks). Descriptions lost only the
  German brackets; quoted labels match the drawings word for word; the
  642–645 switch from "decoder" to "encoder" matches what those drawings
  print, as reported.
- 611, 613, 620, 650, 652, 656, 668 — rendered: no German printed (paths
  only in 611/613; "V", "mech.", "IQ", "?", A/D, country prefixes,
  "Remote", "Internet", "DL1FLO"). Untouched in the commit.
- The glossary change (§14 *Ort* note now naming drawing 628) matches the
  drawing. The suspected alt-text errors (620 "A" meter, 633 voltmeter vs
  `sV` source, 642–645 decoders) are confirmed against the renders and
  left as reported.
