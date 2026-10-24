# crtezi_10 — drawing translation report

29 drawings (`crtezi.json`): 894, 895, 896, 897, 898, 899, 903, 908, 909,
911, 913, 914, 916, 917, 918, 922, 923, 925, 926, 927, 928, 935, 936, 937,
940, 941, 942, 949, 950.
17 translated and rebuilt with `darc-drawing.py` at DARC's default 9 cm,
12 with nothing to translate. Every rebuilt drawing was compared side by
side with its original PNG: same drawing, English text, nothing overlapping
or cut off. The untouched ones were rendered from their SVGs: no German
printed.

## Per drawing

- 894, 895, 896, 897, 898, 899 — nothing to translate: "H", "E", "I", "+",
  "−" only; the `% Schwingkreis`, `% Feldlinien …` comments stay.
- 903 — "Eingangssignal" → "Input signal", "Frequenzgemisch" → "Frequency
  mixture" (§14 row 916/917/937/903, §5 *Eingangssignal*). The symbols
  f_e, f_z, f_o, G unchanged.
- 908 — "70 cm Band" → "70 cm band" (§14 row 949/908/909; house style band
  names). "430 MHz", f_T, f unchanged.
- 909 — as 908, and the decimal comma `\qty{430,0075}` → 430.0075.
- 911 — the two-line "Digitale Signal-" / "verarbeitung" → "Digital
  signal" / "processing" (§6 *Digitale Signalverarbeitung*, §14 row
  842/843/…/911/914; same split as 96). A/D, D/A unchanged.
- 913 — "HF" / "ZF" / "NF" → "RF" / "IF" / "AF" (abbreviation rule). VFO,
  BFO and the frequencies unchanged; "3.455–30.455 MHz" was already written
  with points in the `.tex` and now prints them.
- 914 — "NF" → "AF", "Balance-" / "modulator" → "Balanced" / "modulator"
  (two lines, as 98; §7 *Balancemodulator*), "Mischer" → "Mixer", "Treiber"
  → "Driver" (§5). CO, VFO, PA, ALC, G unchanged.
- 916 — "SWR-Meter" → "SWR meter" (§11), "Tiefpass" → "Low-pass filter"
  (§5), "Antenne" → "Antenna", "Senderausgangsleistung" → "Transmitter
  output power" (§1, §14 row 916/917). "Transceiver" unchanged.
- 917 — as 916, with "Messung von unerwünschten Aussendungen" →
  "Measurement of unwanted emissions" (§1 *unerwünschte Aussendungen*).
- 918 — nothing to translate: "f_0 / 1 Harm.", "1. OW / 2 Harm." … "3. OW /
  4 Harm.", "≥ 60 dB", A, f stay as printed, by the §14 row *„1 Harm.“ /
  „1. OW 2 Harm.“ … (Zeichnungen 868, 869, 918)* (as 868/869 in
  crtezi_09).
- 922 — "Dielektrikum" → "Dielectric", "Elektrode" → "Electrode" (twice)
  (§3 *Dielektrikum*, §14 row 858/922/923/958).
- 923 — "Plastik-Gehäuse" → "Plastic case", "Keramik-Dielektrikum" →
  "Ceramic dielectric", "Metalllegierung" → "Metal alloy" (§14
  *Plastikgehäuse / Metalllegierung / Keramikdielektrikum*).
- 925, 926, 927, 928 — nothing to translate: no printed text at all.
- 935, 936 — "Erde" → "Earth" (§14 row *„Erde“ (Bodenfläche)*). E, H, S
  unchanged.
- 937 — "Leistungsoptimum" → "Power optimum" (§14 row). P_L, P_max, R_L and
  the Ω ticks unchanged; the `use comma` option stays (the tick labels are
  written out as `\qty{…}{\ohm}`, so it prints nothing, as 858/872).
- 940 — y-axis "Leistung" → "Power" (§14 row *„Leistung“*); decimal commas
  8998,5 / 9001,2 / 9001,5 → points. LSB, f, 300 Hz, 3 kHz unchanged.
- 941 — as 940 (USB): "Leistung" → "Power"; 8998,8 / 9001,5 / 8998,5 →
  points.
- 942 — "Spule ohne Kern" / "Spule mit Eisenkern" / "Spule mit Ferritkern"
  / "Veränderliche Spule" → "Air-cored inductor" / "Iron-cored inductor" /
  "Ferrite-cored inductor" / "Variable inductor" (§14 symbol-chart row,
  §4 *Luftspule*).
- 949 — "30 St." → "30 pcs." (§14 row 949), `\qty{0,6}` → 0.6. "1 A", U, I
  unchanged.
- 950 — nothing to translate: the angle and dB tick labels are written out
  (`$-40^{\circ}$` …, `\qty{-6}{\dB}` …), no decimals, so the `use comma`
  option prints nothing; the coordinate names (`geschlechtsteil`, `hals`)
  are not printed.

Descriptions (`N.txt`): the German brackets dropped in 903, 908, 909, 911,
913, 914, 916, 917, 922, 923, 935–937, 940–942 and 949; the quoted labels
already matched the drawings. 918's `("1. OW")` is the label the drawing
prints, not a German bracket, and stays; 918 and the other drawings with
nothing to translate are unchanged.

## Collisions

None. Size changes worth noting:
- 917 — 293.5 × 119.9 → 255.1 × 106.8 pt. Not a scaling of the drawing:
  DARC's own untranslated `917.tex`, built with today's setup, comes out
  419.3 × 161.5 pt (the long German label anchored east pushes the
  autoscale over); the English label is shorter and the drawing fits the
  9 cm exactly (checked, then the translated file restored and rebuilt).
- 923 — 287.1 × 148.8 → 263.7 × 139.0 pt: "Metal alloy" and "Ceramic
  dielectric" are shorter than the German labels, so the label overhang
  shrinks (the untranslated file today gives 289.5 × 150.1 pt). All labels
  inside the drawing, the body at its German proportions.
- 942 — 1.7 pt lower; "Ferrite-cored inductor" ends inside the left half.
All other widths and heights are within 1.2 pt of the originals.

## Glossary

No rows added: every label is already in the glossary (§1
*Senderausgangsleistung*, *unerwünschte Aussendungen*; §3 *Dielektrikum*; §4
*Luftspule*; §5 *Tiefpass*, *Eingangssignal*, *Treiber*, *Mischer*; §6
*Digitale Signalverarbeitung*; §7 *Balancemodulator*; §11 *SWR-Meter*;
§14 drawing-label rows for 842/843/…/911/914, 858/922/923/958,
916/917/937/903 with *„Erde“ (Bodenfläche)*, 949/908/909, 868/869/918,
*„Leistung“*, the inductor symbol-chart row and *Plastikgehäuse /
Metalllegierung / Keramikdielektrikum*). HF/ZF/NF → RF/IF/AF follows the
abbreviation rule.

## Suspected errors

None in the German drawings. The SSB frequencies of 940 (LSB 8998.5–9001.2
kHz under the 9001.5 kHz carrier) and 941 (USB 8998.8–9001.5 kHz above the
8998.5 kHz carrier) agree with the 300 Hz–3 kHz baseband.
