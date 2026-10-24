# crtezi_12 — drawing translation report

29 drawings (`crtezi.json`): 1007, 1008, 1010, 1011, 1018, 1022, 1023,
1024, 1027, 1028, 1029, 1030, 1031, 1032, 1033, 1034, 1035, 1044, 1046,
1048, 1049, 1051, 1052, 1055, 1056, 1058, 1064, 1071, 1072.
26 translated and rebuilt with `darc-drawing.py` at DARC's default 9 cm,
3 with nothing to translate. Every rebuilt drawing was compared side by
side with its original PNG: same drawing, English text, nothing
overlapping or cut off. The three untouched ones were rendered from their
SVGs: no German printed.

## Per drawing

- 1007 — "Reales Strommessgerät" → "Real ammeter" (§14 *reales
  Strommessgerät*, as 1004 in crtezi_11). R_i, U_i, A unchanged.
- 1008 — "Oberwellen (OW)" → "Harmonics (OW)" (§14 row *„1. OW“ … „4. OW“
  (Zeichnung 1008)*, as 868/869 in crtezi_09). "1. OW" … "4. OW", "NA",
  f_0, A, f stay as printed, by the same row.
- 1010 — x-axis "Zeit [Stunden]" → "Time [hours]", y-axis "Dämpfung [dB]"
  → "Attenuation [dB]" (§14 row *„Zeit [Stunden]“*, §5 *Dämpfung*). The
  legend's `\qty{3.6}` … were already written with points (the German
  build printed commas, the British one points). The `%` comment "aus
  echten daten der NOAA" and the CSV data stay.
- 1011 — nothing to translate: the world map prints only the colour-bar
  ticks 0, 10, 20, 30; no words, no decimals.
- 1018 — "Reale Spannungsquelle" → "Real voltage source" (§14 *Reale
  Spannungsquelle*). R_i, U_q, U_k, R_L, I unchanged.
- 1022, 1024 — y-axis "$U_\text{A}$ bzw. Verstärkung" → "$U_\text{A}$ or
  gain" (*bzw.* as the §14 *„fc bzw. foF2“* row, §5 *Verstärkung*), the
  rotated "Grenzfrequenz" → "Cut-off frequency" (§5 *Grenzfrequenz*). U_A,
  f_g, f unchanged.
- 1023 — "ochpass" → "igh-pass": the drawing spells *Hochpass* with a red
  H drawn over the capacitor plus the word "ochpass"; "High-pass" starts
  with the same H, as the course tip says (*H*igh-pass, §5 *Hochpass*).
- 1027–1035 — "Zeit" → "Time" beside the t axis (§14 *„Zeit“* row). I, t
  unchanged; the commented-out `\only<…>` lines untouched.
- 1044 — "Bandbreite" → "Bandwidth" (§5 *Bandbreite*). P, f, "100 %",
  "50 %" unchanged; the `%` comments stay.
- 1046 — nothing to translate: antenna pattern with no text at all.
- 1048 — "Reflektor" / "Strahler" / "Direktor" → "Reflector" / "Radiator"
  / "Director" (§9 *Direktor / Reflektor*, *Strahler*, as the course text
  yagi_uda_2), the rotated "Strahlungsrichtung" → "Direction of radiation"
  (§14 *Strahlungsrichtung*).
- 1049 — nothing to translate: Yagi with its polar pattern, no text; the
  `use comma` option prints nothing (ticks off), so it stays, as in
  earlier batches.
- 1051, 1052 — the two-line "Antennen-" / "tuner" → "Antenna" / "tuner"
  (§9 *Antennentuner* → antenna tuner). TX, SWR, "15 m" unchanged.
- 1055 — "HF" / "ZF" / "NF" → "RF" / "IF" / "AF" (abbreviation rule),
  "1. Mischer" / "2. Mischer" → "1st mixer" / "2nd mixer" (§14 *„1.
  Mischer“* row). VFO, BFO, AGC unchanged.
- 1056 — "Leistung" (twice) → "Power" (§3, §14 *„Leistung“* row); decimal
  commas `\qty{7,101}`, `\qty{7,100}` (twice), `\qty{7,099}` → 7.101,
  7.100, 7.099. USB, LSB, f, f_T, "1 kHz" unchanged.
- 1058 — "Reale Stromquelle" → "Real current source" (§3 *Stromquelle* →
  current source, as *Reale Spannungsquelle* in 1018). I_q, R_i, R_L, I
  unchanged.
- 1064 — "Phase wird um \qty{180}{\degree} gedreht" → "Phase is shifted
  by \qty{180}{\degree}" — as the figure's caption in
  sections/mehrwegeausbreitung (*Phasenverschiebung bei der Reflexion* →
  "phase shift on reflection").
- 1071, 1072 — "Basis" / "Kollektor" → "Base" / "Collector" (§4 *Basis /
  Emitter / Kollektor*); "Emitter", N, P, U_BE, U_CE, I_B, I_E, I_C
  unchanged. 1072's blue note "phys. Stromrichtung!" → "Electron flow!"
  (§3 *physikalische Stromrichtung*, as 1002 in crtezi_11).

Descriptions (`N.txt`): the German brackets dropped in 1007, 1008, 1010,
1018, 1023, 1044, 1048, 1051, 1052, 1055 and 1056. 1022 and 1024 quoted
the y-axis as "Power" ("Leistung") — DARC's German alt text says
„Leistung“, but the drawings print "$U_\text{A}$ bzw. Verstärkung"; they
now quote "U_A or gain", as the drawing. The other quoted labels already
matched the English drawings (1052's "Antenna" (top) and "tuner" (bottom)
read line by line). 1027–1035 have empty descriptions, 1058, 1064, 1071
and 1072 are "TODO" (DECISIONS.md), and 1011, 1046, 1049 had no German
bracket: all unchanged.

## Collisions

None. Clearances and size changes worth noting:
- 1022 — the rotated "Cut-off frequency" is longer than "Grenzfrequenz"
  and, centred where DARC put it (`near start` on the dashed line), ends
  about 1 pt above the x-axis; it does not touch it. No shorter wording
  of *Grenzfrequenz* exists in the glossary, so it was left as built. In
  1024 the same label, on the left of its dashed line, stays clear of the
  falling curve.
- 1018 — 255.1 × 174.4 → 255.1 × 180.0 pt, 1058 — 259.2 × 194.7 → 262.2 ×
  195.1 pt, 1007 — 257.9 × 125.0 → 252.1 × 121.2 pt: the build's
  autoscale to 9 cm lands differently with a label of another width
  ("Reale Spannungsquelle" stuck out left of the shaded box; "Real
  voltage source" does not), as 1004 in crtezi_11. Nothing overlaps.
- 1072 — 250.2 × 214.2 → 253.5 × 216.6 pt: "phys. Stromrichtung!" reached
  past the right-hand wire, "Electron flow!" does not, so 1072 now has
  exactly 1071's size.
- 1027–1035 — 2.6 pt lower ("Time" vs "Zeit" at the axis end).
- 1044 — 1.5 pt wider and higher.
All other widths and heights are within 1.1 pt of the originals.

## Glossary

One row added in §14 (after the *„ca.“ (Zeichnung 866)* row): *„$U_\text{A}$
bzw. Verstärkung“ / „H“ + „ochpass“ / „Reale Stromquelle“ / „Phase wird
um 180° gedreht“ / „phys. Stromrichtung!“* → "U_A or gain" / "H" +
"igh-pass" / "Real current source" / "Phase is shifted by 180°" /
"Electron flow!", with the note on DARC's „Leistung“ in the 1022/1024 alt
texts. The note of the §14 row *reales Spannungsmessgerät / reales
Strommessgerät* no longer says the drawings stay German (1004, 1007 now
print "Real voltmeter", "Real ammeter").

## Suspected errors

None in the German drawings. In DARC's descriptions (not the drawings):
- 1022.txt, 1024.txt — the y-axis is described as „Leistung“; the
  drawings print "$U_\text{A}$ bzw. Verstärkung" (the course captions
  speak of the voltage $U_\text{A}$). The English quotes the drawing.
- 1011.txt — describes "a completely black image with no content"; the
  drawing is a coloured world map with a colour bar (0–35). Left
  unchanged: only the brackets and quoted labels are this phase's to
  touch.
- 1056.txt — speaks of "four spectrum diagrams" that "all four" have a
  "Power" axis; only the two left-hand diagrams have that label. Left
  unchanged, as above.
