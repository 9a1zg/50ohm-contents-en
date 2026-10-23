# slike_03 — translation report

107 files in `contents/drawings/` (21, 22, 24–29, 208, 214–323 as listed in
`serije.json`).

## Files translated (107)

- With a description (107): 21, 22, 24–29, 208, 214–223, 225–228, 230–253,
  255–266, 268, 271–276, 278–293, 295–301, 303–307, 309–320, 323. Of these,
  16 carry DARC's marker, translated: 260, 261, 266, 295–300, 303, 309,
  311–314, 323.

## Files left as they are (0)

- No `TODO` and no empty files in this batch.

`alttext-check.py`: 107 files, 0 with findings. Line counts are the same as
in the German (230 lines changed, 230 replaced); no file of the batch ends
in a newline, in German or English.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

6 rows: *Markierung (Achse) / Skalenmarke / parabelförmige Auslenkung / auf
gleicher Höhe in Bezug auf die t-Achse*; *Antennendiagramm / Kontur /
Schlaufe / sich verjüngen / Maßlinie / Maßpfeil*; *Messgerät „V“ / „A“ /
Spannungsquelle / Reihenschaltkreis*; *Zweileiterleitung / Doppelleitung,
Doppelader / Querstrebe, Querverbinder*; *große Spule mit „ü“ / Kennlinie
„1“ / Zener-Diode (Z-Diode)*; the drawing labels „Leistung“, „Dipol“,
„Richtantenne“, „l = 43,18 m für 7,1 MHz“.

## Judgement calls

- Section labels as glossary §14: *Kurzbeschreibung* → Short description,
  *Ausführliche / Detaillierte Beschreibung, Detailbeschreibung* → Detailed
  description, *Kurze Zusammenfassung* → Short summary, *Zusammenfassung* →
  Summary, *Kurzfassung* → Brief summary, *Details* → Details; 300's bare
  *Kurz:* → "Short:". Numbering and the line break after a label (264, 266)
  kept as in the German.
- *Die Abbildung zeigt* → "The figure shows", *Das Bild zeigt* → "The picture
  shows", as the glossary (§14 *Abbildung / Bild*). slike_02 wrote "The
  picture shows" for *Abbildung* in the sister files 19/20 of 21/22; the
  checker may want to align one way or the other.
- *Sinuskurve* → "sine curve", *sinusförmige Kurve* → "sinusoidal curve"
  (§14); *Nullpunkt* → "origin", *Nulllinie* → "zero line".
- *Markierung* on an axis → "tick mark"; *Skalenmarken* → "scale marks";
  *parabelförmige Auslenkung* → "parabola-shaped excursion" (*displacement*
  is kept for field lines).
- 218–221: *liegen auf gleicher Höhe in Bezug auf die „t“-Achse* → "line up
  with respect to the "t" axis" — the German means they sit at the same
  time, not at the same height.
- Labels that are German words: English, then the German in brackets —
  "Power" ("Leistung") in 250–253, 257–259, "Dipole" ("Dipol") and
  "Directional antenna" ("Richtantenne") in 264, "l = 43.18 m for 7.1 MHz"
  ("l = 43,18 m für 7,1 MHz") in 311. Labels that are only numbers, units or
  symbols get the decimal point and no bracket ("0.3", "3.0", "+5.6 V",
  "f_res = 7.05 MHz", "0.05·λ", "≥ 0.05·λ").
- "MWS" (260, 315) kept as printed, as glossary §9 *Mantelwellensperre*
  says; "ü = 1 : 7", "ü 1:4", "U_HF", "f/kHz", "E / E_max" and 323's
  `\( R_V \)` markup unchanged. The feed-point marks "X   X" keep their three
  spaces.
- *Spule* → "inductor"; the windings of a transformer (29, 303, 304) and the
  large winding with a ratio in 260/315 → "coil". *Drehkondensator* →
  "variable capacitor", *Parallelschwingkreis* → "parallel tuned circuit",
  *Schwingkreis* → "tuned circuit" (§5), *sog. Traps* → "so-called traps".
- *Messgerät „V“ / „A“* → meter "V" / "A"; *Masse* → "chassis",
  *Erdungssymbol* (222) → "earth symbol".
- 271–276: *Anschluss* of a circuit symbol → "connection" (the German uses
  it for the leads, not for drawn terminals).
- 312–314: *Doppelader / Doppelleitung* → "twin line", *Zweileiterleitung* →
  "two-wire line", *Leitungszug* → "line run"; *Querstreben / Querverbinder*
  → "crosspieces / cross-connections".
- 317–320: *Zener-Diode (Z-Diode)* → "Zener diode (Z diode)" and *Zener-Diode
  oder Z-Diode* → "Zener diode or Z diode", keeping the German's two names
  (glossary §4 maps both to *Zener diode*).
- 307: *Kennlinie „1“* → characteristic "1" (§5 *Kennlinie*).
- 260: the non-word *Umwicklungsverhältnis* → "winding ratio" (literal; 315
  calls the same label *Übersetzungsverhältnis* → "transformation ratio").
  *Leitung mit 50 Ohm* → "a line of 50 Ω".
- 268 is word for word the German of 1046 (slike_01), so it takes 1046's
  English unchanged.
- 275, 289: the label ") Ausführliche Beschreibung" lost its "2"; written
  "2) Detailed description", like the other files.
- 208: a stray closing bracket after "fünften Markierung)" dropped.
- 227: the double space in "einen  Anschlusspunkt" not reproduced.
- 297: *Diagramm zeigt* (no article) kept as "Diagram shows"; 323 likewise
  "Circuit diagram shows".

## Suspected errors in the German descriptions

- 223 — the short description gives the curve "in Höhe von „+10 V“ parallel
  zur horizontalen Achse", the detailed description has no sentence on
  where the curve runs at all (225, 226, 228 have "Eine Kurve verläuft auf
  der Nulllinie"). Translated as written.
- 257 — the short description says vertical axis "U" and a line "im
  mittleren Teil", the detailed one says axis „Leistung“ and line "im
  rechten Teil"; `257.tex` labels the axis `$U$`. It also ends "bis zum Ende
  der horizontalen Linie" where the short one says *Achse* (as 1022 in
  slike_01). Translated as written.
- 278 — the short description gives the base label as „+2,0“ without "V";
  the detailed one and `278.tex` have "+2,0 V". Translated as written.
- 263 — says "Es gibt keine Beschriftungen oder Maße" although it has just
  named the labels „a“ and „b“; also "verikalen" (*vertikalen*).
- 248 — "beginnt bei einem höheren Wert auf der Nulllinie": copied from 249
  ("niedrigen Wert"), meaning a higher frequency; translated as written.
- 266 — the summary calls the small lobe at 180° a *Rückkeule*, the detailed
  description a *Nebenkeule*; translated "back lobe" and "side lobe" as
  written.
- 268 — same German as 1046: "im Winkel vom 120°" and "nahezuförmiger Kreis"
  (see slike_01).
- 271 — "Zwei Schaltzeichen /“1“ und „2“)": a slash for the opening bracket;
  harmless.
- 29 — "Litern" (*Leitern*); 264 — "horiztontalen" (twice); 305 — "Leitern
  Leitern"; 323 — "Ein Zener-Diode" (*Eine*). Harmless typos.
- 304 — says "keine weiteren … Textbeschriftungen" after naming the label
  „U“; *weiteren* covers it, noted only for DARC.

## Provjera

Checked all 107 files against the German at `cbc5d5e~1`, sentence by
sentence: 107 full descriptions (16 with DARC's marker), no `TODO` or
empty files. 6 files changed, 6 lines. `alttext-check.py --rev cbc5d5e~1`:
107 files, 0 with findings.

- 227 — *Im mittleren Leiter folgt nach rechts ein weiterer Widerstand* "In
  the middle conductor, further to the right, follows another resistor" →
  "Further to the right in the middle conductor there is another resistor"
  (natural English).
- 260 — *Leitung mit 50 Ohm* "a line of 50 Ω" → "a 50 Ω line" (natural
  English).
- 297 — *zeigt einen symmetrischen Verlauf* "shows a symmetrical course" →
  "runs symmetrically" (natural English).
- 313 — *Maßpfeil mit der Aufschrift „31,2 m“* "inscribed" → "labelled", as
  slike_02 did for *Aufschrift*.
- 315 — *mit Begrenzungspfeilen nach links und rechts* "with limit arrows to
  the left and right" → "with arrowheads at its left and right ends" (not an
  English term).
- 316 — *ein Block mit der Aufschrift „G“, drei wellenförmigen Linien und …*
  "a block labelled "G", three wavy lines and …" → "a block with the label
  "G", three wavy lines and …", so the wavy lines and the rectangle read as
  part of the block, as in the German.

Left as translated: *Die Abbildung zeigt* → "The figure shows", *Das Bild
zeigt* → "The picture shows", which is what the glossary says (§13
*Darstellung / Abbildung / Bild*). slike_01 and slike_02 wrote "The picture
shows" for *Abbildung* in 18 files (19 and 20 among them); that is for a
later consistency pass over all batches, not changed here. Also left:
*Anschluss* of a circuit symbol → "connection" (271–293), the two names
"Zener diode (Z diode)", "MWS" unquoted in 260 as in the German, the
corrected label "2) Detailed description" in 275/289, and the suspected
German errors listed above, which are reported, not fixed.
