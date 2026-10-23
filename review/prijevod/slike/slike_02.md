# slike_02 — translation report

107 files in `contents/drawings/` (12–20, 111–207 and 1113–1141 as listed in
`serije.json`).

## Files translated (83)

- With a description (83): 12, 13, 14, 15, 16, 17, 19, 20, 111–128,
  136–142, 144–147, 149, 153, 155, 158, 160–170, 172, 173, 175, 181, 182,
  184–204, 206, 207, 1122, 1123, 1124. Of these, 155, 161 and 202 carry
  DARC's marker, translated.

## Files left as they are (24)

- `TODO` only (21): 1113–1116, 1118, 1119, 1121, 1125, 1126, 1128–1139.
- Empty files (3): 1120, 1127, 1141 — nothing to translate.

`alttext-check.py`: 107 files, 0 with findings. Line counts are the same as
in the German (165 lines changed, 165 replaced), and so is each file's final
newline or its absence (only 1122–1124 end in one). The trailing space at
the end of the first paragraph of 206 is kept.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

7 rows: *Schaltplan in rechteckiger Leitungsführung / Anschlusspunkt / an
Masse*; *Ableitung / Abzweigung / Anzapfung*; *Halbbögen / Strich /
Querstrich / durchgestrichene Linie*; *Baustein / polarisierter /
verstellbarer Kondensator / Addierer*; *Nullpunkt / Grundlinie / Auslenkung
/ Bodenfläche*; *Grunddämpfung α0 je 100 m Leitungslänge*; the drawing
labels „ZF“, „NF“, „ZF-Amp.“, „NF/Basisband“, „zum Oszillator“.

## Judgement calls

- Section labels as glossary §14 (slike_01): *Kurzbeschreibung* → Short
  description, *Ausführliche / Detaillierte Beschreibung* → Detailed
  description, *Kurzfassung* (202) → Brief summary; numbering `1)` / `2)`
  kept as in the German.
- *Schaltplan in rechteckiger Leitungsführung* → "Circuit diagram drawn with
  right-angled wiring"; *Leiter* → "conductor"; *Anschlusspunkt* →
  "terminal"; *Masse* → "chassis" (§4 trap; *Erde* stays "earth").
- *Spule* → "inductor" for the component; the two windings of the
  transformer in 197 → "coils". *Halbbögen* → "semicircles", *durchgestrichene
  Linie* → "a line through it".
- *Hüllkurvendemodulator* (144–147) → "envelope detector" (§6); *Hüllform* →
  "envelope shape" (§11 *Hüllkurvenform*).
- *Ableitung* (160, 175, 195, 198) → "shunt path", to keep it apart from
  *Abzweigung* → "branch".
- *Mitte der Sekundär-/Primärwicklung* (153) → "centre of the … winding".
- Labels that are German words: English, then the German in brackets
  ("Earth" ("Erde"), "to oscillator" ("zum Oszillator"), "Frequency [MHz]"
  ("Frequenz [MHz]")). Where the German already puts the label in brackets,
  the German follows in a second bracket: ("AF" ("NF")), (labelled "IF"
  ("ZF")).
- "AF/BB" ("NF/BB") in 155: *BB* (Basisband) is "baseband" in English too,
  so only *NF* changes.
- The terminal letters "E" and "A" (136–140, *Eingang/Ausgang*) and the
  points "A"/"B" of 198 are kept as they are, like the symbols U_E / U_A —
  they are single-letter markings, not words.
- Labels with a decimal comma written with a decimal point ("1.6 V",
  "0.7", "+13.8 V", "IF=10.7 MHz" …), as in slike_01; in the brackets the
  German stays as printed ("ZF=10,7 MHz", "Voll‑PE 2,9 mm RG174").
- 202: *Voll-PE / PE-Schaum / Massivschirm* → "Solid PE / Foam PE / solid
  screen" (§9); "PTFE 1.8 mm RG178" has no German word, so no bracket. The
  non-breaking hyphen of "x‑Achse", "Voll‑PE" kept ("x‑axis").
  *Grunddämpfung* → "basic attenuation"; *Leitungslänge* → "cable length",
  as the course text of `kabeldaempfung_1`.
- 125/126: the symbol "ϑ" kept; the description does not name the component
  (a thermistor), so neither does the English.
- 16: *flacheres Maximum* → "flatter maximum" (15: *flacheres Minimum* →
  "shallower minimum").
- 1123/1124: *Leitungswege* → "current paths".
- 196: the doubled full stop at the end of the short description written as
  one.

## Suspected errors in the German descriptions

- 140 — "Der Kollektor ist über mit dem oberen Leiter verbunden": the word
  after *über* is missing; the drawing connects the collector directly
  (`140.tex`), so translated "The collector is connected to the upper
  conductor".
- 149 — the frame label is given as „f_res  ZF“ (two spaces), but
  `149.tex` prints `f_res ≠ ZF`: the ≠ was lost. Translated as written
  ("f_res  IF").
- 201 — "Rechts vom rechten Widerstand" (twice): there is no resistor at that
  point, the right-hand vertical connection holds a capacitor; translated as
  written ("right-hand resistor").
- 136–140 — "mit Masse vebunden" (*verbunden*), harmless typo.
- 13 — "getrichelte" (*gestrichelte*), harmless typo.
- 175, 195, 200 — "ein ein vertikaler Pfeil"; 175 also "rechts rechts" —
  doubled words, harmless.
- 184 — "die links mit „a“ … gekennzeichnet" lacks *sind*; harmless.
- 1122 — *Neutral dargestellter Ringmodulator* translated "shown in its
  neutral state"; no error, noted because the phrase is unusual.
