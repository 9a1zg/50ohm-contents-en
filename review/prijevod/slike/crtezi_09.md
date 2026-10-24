# crtezi_09 — drawing translation report

29 drawings (`crtezi.json`): 829, 832, 838, 839, 842, 843, 847, 851, 852,
858, 863, 864, 865, 866, 867, 868, 869, 870, 872, 873, 874, 876, 878, 883,
884, 885, 886, 892, 893.
25 translated and rebuilt with `darc-drawing.py` at DARC's default 9 cm,
4 with nothing to translate. Every rebuilt drawing was compared side by side
with its original PNG: same drawing, English text, nothing overlapping or
cut off. The untouched ones were rendered from their SVGs: no German
printed.

## Per drawing

- 829 — "HF (KW)" → "HF", "VHF (UKW)" → "VHF" (§14 row 749/829, as 749 in
  crtezi_08). "LW", "MF", the band values and wavelengths unchanged; they
  now print with a decimal point. The `----` line without `%` in the axis
  is DARC's and stays.
- 832 — decimal commas only: `\qty{9001,5}` → 9001.5, `\qty{8998,5}` →
  8998.5. f_OSZ (symbol), USB, LSB, DSB, SSB, G unchanged.
- 838, 839 — amplifier labels "HF" / "ZF" / "NF" → "RF" / "IF" / "AF"
  (abbreviation rule, as 803). VFO, BFO unchanged.
- 842, 843 — "HF" → "RF", "RX-Mischer" / "TX-Mischer" → "RX mixer" / "TX
  mixer", "Treiber" → "Driver" (§14 row 842/843), "38,666" → "38.666". RX,
  TX, PA, TRX, G, "1"/"3", "28-30", "MHz", the RX:/TX: sums unchanged.
- 847 — the eleven range names (§14 row 847): "Wechselströme" →
  "Alternating currents", "Funkwellen" → "Radio waves",
  "Mikrowellenstrahlung" → "Microwave radiation", "Terahertzstrahlung" →
  "Terahertz radiation", "Infrarot" → "Infrared", "Licht" → "Light",
  "Ultraviolett" → "Ultraviolet", "Röntgenstrahlung" → "X-ray radiation",
  "Gammastrahlung" → "Gamma radiation", "Höhenstrahlung" → "Cosmic
  radiation". "Radar", the scales and units unchanged; `% Beschriftung`
  comments kept.
- 851, 852 — "Anpass-" / "glied" → "Matching" / "network" (two lines, as
  615). U, λ/2, 2·λ unchanged; `% Anpassglied:` kept.
- 858 — "Schottkydiode" → "Schottky diode", "Silizium" → "Silicon",
  "Leuchtdiode" → "Light-emitting diode" (§14 row 858); "Germanium"
  unchanged. Collision fix, see below. The `use comma` option in
  `xticklabel style` stays: the tick labels are written out as
  `\qty{0.2}{\volt}` …, so it prints nothing (as 828).
- 863, 864 — nothing to translate: B, C, E, I_B/I_C/I_E, U_BE/U_CE/U_CB,
  NPN, PNP.
- 865 — "Bodenwelle" → "Ground wave", "Scheinbare Reflexion" → "Apparent
  reflection", "Refraktion" → "Refraction", "Tote Zone" → "Skip zone"
  (§10, §14 rows 741 and 865). D, E, F_1, F_2 and the heights unchanged.
- 866 — "Langwelle" → "Long wave", "Mittelwelle" → "Medium wave" (§10),
  "ca." → "c." (collision, see below; written `c.~` so the British setup
  does not set a sentence space after the point).
- 867 — "Kurzer Weg" → "Short path", "Langer Weg" → "Long path" (§2, §14
  row 865/867).
- 868, 869 — "Oberwellen (OW)" → "Harmonics (OW)" (§14 row *„1. OW“*, as
  the course caption). The numbered labels "f_0 / 1 Harm.", "1. OW / 2
  Harm." … "3. OW / 4 Harm." and "NA" stay as printed: the course captions
  explain the abbreviations ("Overtones (OW), harmonics (Harm.) and
  spurious emissions (NA)"), and the §14 row *„1 Harm.“ / „1. OW 2 Harm.“*
  keeps the labels with their meaning given in the description.
- 870 — "Refraktion" → "Refraction". α, φ, f_c unchanged.
- 872 — y-axis label "Distanz" → "Distance". The `use comma` option stays
  (tick labels written out, as 858).
- 873 — the path texts "Kurzer Weg" / "Langer Weg" → "Short path" / "Long
  path" (as 867). TX, RX unchanged.
- 874 — "Sommertag" → "Summer day", "Wintertag" → "Winter day", "Nacht" →
  "Night" (§14 row 865 …). D, E, F_1, F_2, F and the heights unchanged.
- 876 — "90° O" → "90° E", "90° Zenit" → "90° zenith" (§14 row 876/878).
  "0° N", "180° S", "270° W", "Elevation", "Azimuth" already English.
- 878 — "Zeit" → "Time", "Drehwinkel" → "Angle of rotation", "Bogenmaß" →
  "Radian measure" (§14 row 876/878). A–D, U, t, φ, the tick values
  unchanged.
- 883, 884, 885, 886 — "Erde" → "Earth" (§14 row *„Erde“ (Bodenfläche)*,
  as 192–194, 203, 204). H, E, S unchanged.
- 892, 893 — nothing to translate: "E", "H", "I", "+", "−" only; the
  `% Feldlinien …` comments stay.

Descriptions (`N.txt`): the German brackets dropped in 829, 838, 839, 842,
843, 847, 851, 852, 858, 865–870, 872–874, 876, 878 and 883–886 (in 870 the
non-German bracket `("f_c")` stays). In 866 the quoted labels now say "c."
as the drawing does ("10 m (c. 20 km)", "80 m (c. 200 km)", "Long wave (c.
1000 km)"); "Medium wave, 160 m (200 km)" had no "ca." in the German and is
left as written. 832 had no German brackets (values already with a point)
and is unchanged, as are the four drawings with nothing to translate.

## Collisions

- 858 — "Light-emitting diode", set vertically above the LED curve, ran off
  the top of the drawing. No shorter wording keeps the glossary term, so a
  line break: `node[rotate=90, anchor=west, align=left]{Light-emitting\\
  diode}` (`align=left` is what TikZ needs for a break). Both lines now end
  inside the drawing, as high as "Schottky diode".
- 866 — DARC's autoscale (`\DARCimageOnly`) fits the drawing to 9 cm with
  the label text at full size, so the longer "Long wave (approx. 1000 km)"
  shrank the arcs (82.3 → 69.2 pt high) and "80 m (approx. 100 km)" ran
  into "Medium wave, 160 m (approx. 200 km)". Tried in order: a line break
  in "Long wave" (the autoscale then overshoots to 316 pt wide, because at
  its first trial scale the medium-wave label is the widest object), line
  breaks in both labels (80 m still collides), moving the 80 m label up
  (then it hits the 10 m label). The fix kept is the shorter wording "c."
  (circa) for German "ca." in all four labels of this drawing: the drawing
  is back at its German proportions (255.6 × 82.3 → 255.6 × 81.2 pt), the
  four labels in their original places. Recorded as a glossary row;
  everywhere else *ca.* stays *approx.*

No other collisions. Size changes worth noting:
- 829 — 243.0 × 137.2 → 255.5 × 137.9 pt. Not the translation: DARC's own
  untranslated `829.tex`, built with today's setup, gives the same
  255.5 pt (checked, then the translated file restored and rebuilt).
- 878 — 266.3 × 126.7 → 275.2 × 120.2 pt: "Angle of rotation" is longer
  than "Drehwinkel", so the autoscale draws the axes slightly smaller; all
  labels clear, "Angle of rotation" ends inside the drawing.
- 865 — 3 pt taller ("Apparent reflection" at the top); nothing moves into
  anything.
All other widths and heights are within 0.5 pt of the originals.

## Glossary

One row added in §14, after the *„30 St.“ / … / „10 m (ca. 20 kilo
meter)“* row: *„ca.“ (Zeichnung 866)* → "c.", drawing 866 only, with the
reason above. Everything else is already in the glossary (§2 *kurzer /
langer Weg*; §5 *Treiber*, *Mischer*; §9 *Anpassglied*; §10 *Bodenwelle*,
*tote Zone*, *Refraktion*, *Mittelwelle / Langwelle*; §14 drawing-label
rows for 749/829, 842/843, 847, 858, 865–874, 876/878, 868/869, *„Erde“
(Bodenfläche)*). HF/ZF/NF → RF/IF/AF follows the abbreviation rule.

## Suspected errors

In the German drawings:
- 842.tex — the commented-out TX line reads "30 MHz − 116 MHz = 146 MHz"
  (should be "+"); it is a `%` comment and prints nothing (843 prints the
  correct "+"). Left as it is.

In DARC's German alt text (left as translated):
- 866.txt — the 80 m arrow is said to reach "200 km" (German „80 meter (ca.
  200 kilo meter)“); `866.tex` and the drawing say 100 km. The medium-wave
  label is quoted without "ca." („Mittelwelle, 160 meter (200 kilo
  meter)“), the drawing has it. Translated as written.
- 872.txt — the values are shifted by one tick: "at 10° about 4000 km, at
  20° about 2300 km …"; `872.tex` plots 4025 km at 0°, 2315 km at 10°,
  1475 km at 20°, … 10 km at 90°. Translated as written.
