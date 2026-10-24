# crtezi_07 — drawing translation report

29 drawings (`crtezi.json`): 675, 676, 680, 681, 689, 694, 697, 699, 702,
705, 706, 710, 713, 714, 727, 728, 729, 730, 731, 732, 733, 734, 735, 736,
737, 740, 741, 742, 743.
24 translated and rebuilt with `darc-drawing.py` (22 at DARC's default
9 cm, 675 and 676 at 4 cm, see "Widths"), 5 with nothing to translate.
Every rebuilt drawing was compared side by side with its original PNG: same
drawing, English text, nothing overlapping or cut off. The untouched ones
were rendered from their SVGs: no German printed.

## Per drawing

- 675 — "Quellencodierer" → "Source encoder" (§14 *Quellencodierer / …*).
  "0101", "01" unchanged.
- 676 — "Kanalcodierer" → "Channel encoder" (same row).
- 680 — "Netzgerät" → "Power supply unit" (§5 *Netzteil / Netzgerät*, as
  the course caption "Connecting the power supply unit and the
  transceiver"), `\qty{13,8}{V}` → 13.8, "Sicherung" → "Fuse" (§4),
  "Gleichstrom (I)" → "Direct current (I)", "Kurzschluss- und
  Verpolungsgefahr" → "Risk of short circuit and reverse polarity" (§14),
  "Hohe Spannung" → "High voltage" (§14 row 680/681). "Transceiver (TRX)",
  "~ 230 V" unchanged. One collision, see below.
- 681 — "Lebensgefahr" → "Danger to life" (§12). "120 mA", "120 V", "1 kΩ"
  unchanged.
- 689 — "Grün" / "Gelb" / "Rot" → "Green" / "Yellow" / "Red". "SMD",
  "D", "1 cm", "3 mm", "10 mm" unchanged. Built with a temporary photo, see
  "689 and its photo".
- 694 — "Batterie" → "Battery", "Widerstand" → "Resistor", "Kondensator" →
  "Capacitor", "Spule" → "Inductor", "Schalter" → "Switch", "Antenne" →
  "Antenna", "Masse und / Erde" → "Chassis and / earth" (§4 *Masse
  (Schaltzeichen)* / *Erde*; line break as in the German), "Spannungs- /
  messgerät" → "Voltmeter", "Strom- / messgerät" → "Ammeter" (one line
  each, as the English is one word; §14 row 694). "Diode", "LED",
  "Transistor" unchanged.
- 697 — decimal commas only: the four `0,5 | 45°` labels → `0.5 | 45°`.
  "8QAM", "I", "Q" unchanged; the `% … r=0,5` comments stay. See
  "Suspected errors".
- 699 — "IPv4-Adresse" → "IPv4 address", "Netzmaske" → "Netmask",
  "Netzanteil" → "Network part", "Hostanteil" → "Host part" (§14 rows
  *Netzanteil / Hostanteil*, *… / Netzmaske*, 699/706).
- 702 — "Phasen- / wechsel" → "Phase / change" (§14 row 700–705; the
  English is two words, so the hyphen goes and the break stays), the four
  `0,5 | …°` labels → `0.5 | …°`.
- 705 — "Phasen- / wechsel" → "Phase / change" in the `phaseshiftPic`; the
  three commented-out `%\node … {Phasen-\\…wechsel}` lines are `%` comments
  and stay.
- 706 — "internes / Netz" → "internal / network", "Internet- / anschluss" →
  "Internet / connection", "Server- / netz" → "Server / network" (§14 row
  699/706, label case kept); "Router" unchanged. Line breaks where the
  German had them.
- 710, 713, 714 — nothing to translate: charges drawn as circles with "+"
  and "−" only (714 also the smartphone of `\smartphone` and a large "+" /
  "−"). German `%` comments stay.
- 727 — "Positive Halbwelle" / "Negative Halbwelle" → "Positive half cycle"
  / "Negative half cycle" (§3 *Halbwelle*).
- 728 — "Periode" (twice) → "Period" (§3).
- 729 — axis labels "Jahre" → "Years", "Sonnenflecken im Mittel pro Monat"
  → "Mean sunspots per month" (§14 row 727–729). The data block unchanged.
- 730 — "Lautstärke" → "Volume", "Tiefe / Töne" → "Low / tones", "Hohe /
  Töne" → "High / tones", "Laut" → "Loud", "Leise" → "Quiet",
  "Information / (Sprache)" → "Information / (speech)" (§14 row 730).
- 731 — "Höhe [km]" → "Height [km]", "bis 10" → "up to 10", "Erde" →
  "Earth" (white on the blue earth; §14 row *„Erde“ (Bodenfläche)*),
  "Troposphäre" → "Troposphere", "D-Region" / "E-Region" → "D region" /
  "E region" (§10), "$\text{F}_1+\text{F}_2$-Regionen" →
  "$\text{F}_1+\text{F}_2$ regions", "Ionosphäre" → "Ionosphere".
  "Sporadic-E" is printed in English and stays (§14 row 731–733).
  "50-90", "90-130", "130-400" unchanged.
- 732 — "Sender" → "Transmitter", "Empfänger" → "Receiver" (§6),
  "Raumwelle" → "Sky wave", "Bodenwelle" → "Ground wave" (§10). The
  `~~~` / `\quad\quad~~` padding in front of the two wave labels kept.
- 733 — "Sender" / "Empfänger" as 732, "VHF-Signale" → "VHF signals",
  "Erde" → "Earth" (as 731). "Sporadic-E" unchanged.
- 734 — "Kalte Luft" → "Cold air", "Warme Luft" → "Warm air", "Sehr kalte
  Luft" → "Very cold air" (§14 row 734). German `%` comments stay.
- 735, 736 — nothing to translate: block diagrams numbered 1–8 / 1–6 and the
  generator's "G".
- 737 — "Starkes Signal" → "Strong signal", "Schwaches Signal" → "Weak
  signal", "Rauschen" → "Noise" (§14 row 737). "Squelch" unchanged.
- 740 — "Spannungseinstellung" → "Voltage setting", "Überlast" →
  "Overload", "Ausgang" → "Output" (§14 row 740). "V", "A", "ON", "OFF"
  unchanged.
- 741 — as 732, plus "Tote Zone" → "Skip zone" (§10 *tote Zone*).
- 742 — axis label "Frequenz [Hz]" → "Frequency [Hz]" (§14 row 742);
  tick labels and "dB" unchanged.
- 743 — "Leistung" (three times) → "Power" (§3), `\qty{2,7}` (twice) →
  2.7. "AM", "USB", "LSB", "6 kHz", "300 Hz", "3 kHz", `f_\mathrm{T}`
  unchanged.

Descriptions (`N.txt`): the German brackets dropped in 675, 676, 680, 681,
689, 694, 699, 702, 705, 706, 727–734, 737, 740–743. The quoted labels
match the drawings (labels set on two lines quoted as one, as before:
"Server network", "internal network", "Internet connection", "Phase
change", "Low tones", "Information (speech)", "Risk of short circuit and
reverse polarity", "Chassis and earth"). One change beyond the brackets:
694's short description said the symbols are "each with a German label
below it" (DARC: „jeweils mit deutscher Beschriftung darunter“; slike_06
kept it "while the drawing is untranslated"); the drawing now prints English,
so it reads "each with an English label below it". 697 had no German
brackets ("0.5 | 45°" already with a point) and is unchanged, as are the
five drawings with nothing to translate.

## Collisions

- 680 — "Risk of short circuit and reverse polarity" in one line ran into
  "⎓13.8 V" below the power supply unit. No shorter wording keeps the
  glossary term, so the label is broken into two lines (the second step in
  DECISIONS.md): `\shortstack{Risk of short circuit\\and reverse polarity}`
  inside the existing `\textit`; position, colour and size unchanged. The
  drawing is 7.1 pt taller (84.1 → 91.2 pt); the second line stays clear of
  the earth symbol.

Everything else fits without a change:
- 706 — "connection" is wider than "anschluss": the drawing is 4.8 pt wider
  (267.3 → 272.1 pt); "internal network" and "Server network" stay inside
  their clouds.
- 732, 733, 741 — "Transmitter" is wider than "Sender" and still inside
  the drawing; "Sky wave" / "Ground wave" are shorter than the German. The
  drawings get 3.4–5.0 pt lower ("Receiver" has no descender).
- 694 — "Voltmeter" / "Ammeter" on one line make the drawing 2 pt lower.

## Widths

675 and 676 were originally built at 4 cm, not 9 cm: at 9 cm the rebuild
came out 254.3 pt wide instead of 113.3 pt. Rebuilt with
`darc-drawing.py --width 4 675 676`, which reproduces the original size
exactly (113.256 × 41.995 pt). A rebuild of either must pass `--width 4`
(no `sirine.json` entry; that file is outside this batch). All other
widths are within 1.5 pt of the originals except 706 (+4.8 pt); heights
within 2 pt except 680 (+7.1), 732/741 (−3.4) and 733 (−5.0), all named
under "Collisions".

## 689 and its photo

689 draws its labels over `\includegraphics{foto/6}`, and there is no
`contents/photos/6.*` in the repository (nor in its history), so the build
failed ("File `foto/6' not found"). The photo is embedded in the original
`689.svg` (an RGB image plus an alpha mask, 1225 × 1388 px); it was
extracted from `HEAD:contents/drawings/689.svg`, put together as an RGBA
PNG, placed at `contents/photos/6.png` only for the build, and removed
again: it is not committed. The rebuilt drawing shows the same photo at the
same size (260.7 → 260.6 pt). A later rebuild of 689 needs the same step, or DARC's photo;
so may the other drawings that include a `foto/N` (671, 690–693, 748, 791).

## Glossary

No new rows: every label is already in the glossary (§3 *Leistung*,
*Periode*, *Halbwelle*; §4 *Sicherung*, *Masse / Erde (Schaltzeichen)*; §5
*Netzteil / Netzgerät*; §6 *Sender*, *Empfänger*; §10 *D-Region …*,
*Raumwelle*, *Bodenwelle*, *tote Zone*, *Troposphäre*, *Ionosphäre*; §12
*Lebensgefahr*; §14 *Kurzschluss- und Verpolungsgefahr*, *Quellencodierer …*,
*Netzanteil / Hostanteil*, and the drawing-label rows for 680/681, 700–705,
699/706, 730, 731–733, 727–729, 694, 734, 737, 740, 741, 742 and *„Erde“
(Bodenfläche)*). "VHF-Signale" → "VHF signals" follows UKW → VHF.

## Suspected errors

In the German drawings:
- 697 — all four inner constellation points are labelled „0,5 | 45°“,
  although they sit at 45°, 135°, 225° and 315° (the companion drawing 702
  labels them 0,5 | 45°, 135°, 225°, 315°). Translated faithfully as
  "0.5 | 45°" four times.
- 742 — the extra x tick labels "5000", "10000", "20000" crowd each other at
  the right-hand end of the log axis (they touch); the same in the original,
  not changed.

In DARC's German alt text (left as translated):
- 729.txt — "maxima … at intervals of about 1 year": already reported in
  slike_06 (the eleven-year cycle).
- 714.txt — "a stylised radio" (both descriptions): `714.tex` draws
  `\smartphone`, and the render shows a smartphone. Translated as written.
