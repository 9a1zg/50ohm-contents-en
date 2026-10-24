# crtezi_13 — drawing translation report

27 drawings (`crtezi.json`): 1075, 1078, 1080, 1081, 1082, 1092, 1093,
1094, 1095, 1096, 1097, 1103, 1106, 1113, 1114, 1115, 1116, 1117, 1118,
1119, 1120, 1126, 1127, 1131, 1132, 1134, 1139.
25 translated and rebuilt with `darc-drawing.py` (23 at DARC's default
9 cm, 1113 at 18 cm and 1119 at 14 cm, see "Widths"), 2 with nothing to
translate. Every rebuilt drawing was compared side by side with its
original PNG: same drawing, English text, nothing overlapping or cut off.
The two untouched ones were rendered from their SVGs: no German printed.

## Per drawing

- 1075 — the six FET names → "Depletion-mode N-channel junction FET",
  "Depletion-mode P-channel junction FET", "Enhancement-mode N-channel
  MOSFET", "Depletion-mode N-channel MOSFET", "Enhancement-mode P-channel
  MOSFET", "Depletion-mode P-channel MOSFET" (§4 *selbstsperrend /
  selbstleitend*, *Sperrschicht-FET*; word order as the question bank,
  "Depletion-mode N-channel junction FET").
- 1078 — x-axis "Wellenwiderstand $Z_0$ in Ω (log)" → "Characteristic
  impedance $Z_0$ in Ω (log)" (§9, the course text innenwiderstand speaks
  of cables), y-axis "normierter Wert" → "Normalised value", legend
  "Leistung" / "Dämpfung" → "Power" / "Attenuation". `%` comments stay.
- 1080, 1081, 1093, 1094 — decimal commas only: `\qty{2,4}` and
  `\qty{0,3}` → 2.4, 0.3. PC, SDR, LNB, TCXO, GPS, GPSDO, DC, PTT, G
  unchanged.
- 1082 — "Taktgenerator" / "Adresszähler" / "Sinus-Tabelle" / "D/A
  Umsetzer" → "Clock generator" / "Address counter" / "Sine table" / "D/A
  converter", as the §14 row for drawing 438 (the same DDS diagram).
  "Register", "Bits", N unchanged.
- 1092 — the six panel titles: "1. AF wanted signal: single tone", "2. AM
  of 1: single tone modulates carrier amplitude", "3. SSB of 1: one RF
  component, constant envelope", "4. Two-tone AF wanted signal: e.g.
  700 Hz and 1200 Hz", "5. AM of 4: two tones modulate carrier
  amplitude", "6. SSB of 4: two RF components with beat" (ssb_3:
  *Zweiton-Nutzsignal* → two-tone wanted signal, *HF-Linie* → RF
  component as the course text explains the figure; §7 *Hüllkurve*,
  §3 *Schwebung*). `%` comments stay.
- 1095 — x-axis "Frequenz in MHz" → "Frequency in MHz", y-axis
  "Leistung" → "Power", "Bereich um / $f_1$ und $f_2$" → "Region around /
  $f_1$ and $f_2$". Spectral line labels unchanged.
- 1096 — "Eingangsleistung $P_\text{in}$" / "Ausgangsleistung
  $P_\text{out}$" → "Input power" / "Output power" (§6), legend
  "Sättigung" / "$f_1$ und $f_2$" / "3. Ordnung" → "Saturation" / "$f_1$
  and $f_2$" / "3rd order" (§14 *Sättigung*; "3rd order" as the course
  text's "3rd-order"). IP3 unchanged.
- 1097 — "Rauschen" → "Noise" (§6). "Signal", SNR, U, t unchanged.
- 1103 — nothing to translate: the crossed Yagi prints no text; only the
  `%` comments are German.
- 1106 — "Richtantenne" / "Dipol" → "Directional antenna" / "Dipole" (§14
  drawing-label row, as 1022). P_R, P_V, P_D unchanged.
- 1113 — "Reaktives Nahfeld" / "Strahlendes Nahfeld" / "Fernfeld" →
  "Reactive near field" / "Radiating near field" / "Far field" (§14
  *Nahfeld (reaktives / strahlendes) / Fernfeld*, as nahfeld).
- 1114, 1115 — "Distanz, normiert:" → "Distance, normalised:",
  "elektrische / magnetische Feldstärke, normiert:" → "Electric / Magnetic
  field strength, normalised:", the three region names as 1113, tick
  labels `$0{,}01$`, `$0{,}1$` → 0.01, 0.1.
- 1116 — as 1114 for the x-axis, ticks and regions; y-axis
  "Feldwellenwiderstand:" → "Wave impedance:" (§14 *Feldwellenwiderstand
  $Z_\mathrm{F}(d)$* → wave impedance; `\text{ in }` already English),
  "Elektrischer Dipol" / "Magnetische Loop" → "Electric dipole" /
  "Magnetic loop".
- 1117 — "Phasenmodulator" → "Phase modulator". I(t), Q(t), φ, A, G
  unchanged.
- 1118 — "Emitterschaltung" / "Kollektorschaltung" → "Common-emitter
  circuit" / "Common-collector circuit" (§5, as the caption). B, C, E,
  U_E, U_A unchanged.
- 1119 — "Stromsteuerkennlinie" → "Current transfer" / "characteristic"
  (two lines, see "Collisions"; §14 *Steuerkennlinie*), "Eingangskennlinie"
  → "Input characteristic", "Ausgangskennlinien" → "Output
  characteristics", "Arbeitspunkt" → "Operating point" (§5); U_BE tick
  labels `0{,}6`, `0{,}7`, `0{,}8` → 0.6, 0.7, 0.8. Axis labels
  "$U_{CE}$ in V" etc. already English.
- 1120 — "Verluste durch Abwärme und Ruheströme" → "Losses due to waste
  heat and quiescent currents" (§5 *Ruhestrom*), "HF Nutzleistung" →
  "Usable RF power" (verstaerker_wirkungsgrad: "usable RF power"),
  "Zugeführte Gleichstromleistung" → "DC input power supplied" (§14, AF401).
  P_DC, P_HF, P_V unchanged.
- 1126 — "kurze Torzeit" / "lange Torzeit" → "short gate time" / "long
  gate time" (§11 *Torzeit*); `\qty{1,1}` → 1.1.
- 1127 — "Träger" → "Carrier" (§7). LSB, USB unchanged.
- 1131 — "Anti-Aliasing" / "Filter" → "Anti-aliasing" / "filter",
  "Rekonstruktions" / "Filter" → "Reconstruction" / "filter" (§8
  *Antialiasingfilter*, §14 *Rekonstruktionsfilter*; two-line label with
  a lower-case second line, as 1051/1052). Terminals E, A stay (§14
  *ZF/NF* row).
- 1132 — "Weitere / Teile / des / Empfängers" → "Further / parts / of the
  / receiver", "Kontroll- / information" → "Control / information", as the
  §14 row for drawing 439.
- 1134 — nothing to translate: the four panels print only angle numbers
  and $l = \frac{1}{4}\lambda$ etc.; every German word is in `%` comments.
- 1139 — x-axis "Frequenz in MHz" → "Frequency in MHz", y-axis "Grenzwert
  in dBc" → "Limit in dBc" (§1.4 *Grenzwert*), legend "Vfg. 33/2007 (2)"
  → "Order 33/2007 (2)" (§14 *Verfügung 33/2007*). ETSI entries
  unchanged; the commented-out tick labels with decimal commas stay as
  comments.

Descriptions (`N.txt`): none changed. 1075, 1078, 1080–1082, 1092–1095,
1113–1116, 1118, 1119, 1126, 1131, 1132, 1134 and 1139 are "TODO"
(DECISIONS.md), 1096, 1097, 1120 and 1127 are empty, and 1103, 1106 and
1117 have no `.txt`. None quotes a German label.

## Widths

- 1113 — originally built at 18 cm (510.2 pt wide), not 9 cm: at 9 cm
  the rebuild came out 258.8 pt wide and "Reactive near field" ran into
  "Radiating near field". Rebuilt with `darc-drawing.py --width 18 1113`,
  which reproduces the original size exactly (510.2 × 60.1 pt); the
  labels are then as clear of each other as the German ones.
- 1119 — originally built at 14 cm (396.85 pt wide). Rebuilt with
  `darc-drawing.py --width 14 1119`.
A rebuild of either must pass the same `--width` (no `sirine.json`
exists).

## Collisions

- 1119 — "Current transfer characteristic" on one line was far wider than
  "Stromsteuerkennlinie" and stuck out to the left, so the drawing came
  out at 211.3 instead of 239.8 pt high (everything shrank about 12 %).
  Fix: a line break ("Current transfer" / "characteristic", the node is
  already `align=right` with a break before the formula). No coordinates
  changed. Now 396.85 × 252.6 pt: the extra line adds height on top;
  "Input characteristic" is now the leftmost text. Nothing overlaps;
  "Operating point" crosses the load line and the I_C curves on its white
  background exactly as "Arbeitspunkt" does.

Size changes worth noting (autoscale to the build width with labels of
another width; nothing overlaps):
- 1106 — 256.9 × 154.3 → 259.5 × 148.2 pt: "Directional antenna" sticks
  out further right than "Richtantenne".
- 1120 — 255.1 × 148.3 → 255.1 × 136.1 pt: the rotated "DC input power
  supplied" is shorter than "Zugeführte Gleichstromleistung".
- 1132 — 255.1 × 154.2 → 255.1 × 163.7 pt: "receiver" is narrower than
  "Empfängers".
- 1082 — 258.2 × 104.6 → 258.2 × 113.4 pt: the rotated "Clock generator"
  and "Address counter" are longer than the German.
- 1075 — 215.1 → 210.5 pt wide; 1114, 1115 — about 3 pt higher (longer
  rotated y-axis labels, still within the drawing).
- 1118 — 252.0 → 255.1 pt wide: "Common-collector circuit" is wider than
  "Kollektorschaltung" (the two titles stay well apart).
- 1095 — 236.5 → 234.3 pt wide ("Power" is shorter than "Leistung").
All other widths and heights are within 2 pt of the originals.

## Glossary

One row added in §14 (after the crtezi_12 row): *„normierter Wert“ /
„Distanz, normiert“ / „elektrische / magnetische Feldstärke, normiert“ /
„Bereich um f1 und f2“ / „Nutzsignal NF: Einton“ / „Einton moduliert
Trägeramplitude“ / „HF-Linie(n)“ / „Elektrischer Dipol“, „Magnetische
Loop“ / „Stromsteuerkennlinie“ / „Ausgangskennlinien“ / „HF
Nutzleistung“ / „Verluste durch Abwärme und Ruheströme“ / „kurze / lange
Torzeit“ / „Grenzwert in dBc“ / „Vfg. 33/2007 (2)“ / „Rekonstruktions“ +
„Filter“*, with the English as above.

## Suspected errors

In the German drawings (translated faithfully, not fixed):
- 1127.tex — the carrier frequency Ω is typeset as `$\unit{\ohm}$` (the
  ohm unit symbol) in "Ω − ω", "Ω", "Ω + ω": an upright unit sign
  instead of the variable $\Omega$ the course text uses
  ($U_\mathrm{AM}(t) = … \cos(\Omega t)$). It prints the same glyph, so
  readers will hardly notice.
- 1139.tex — the 160 m band is drawn as `rectangle (1.81,-100)
  rectangle (2.0,-100)`: both corners at −100, so the band has no
  height and is not shaded, unlike every other amateur band (the others
  go to 100). The 2200 m band (0.1357 MHz) lies left of `xmin=0.15` and
  is not visible either, which may be intended.
- 1075.txt … 1139.txt — no description yet ("TODO" or empty); not this
  phase's to write.
