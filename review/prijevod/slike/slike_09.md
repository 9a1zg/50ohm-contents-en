# slike_09 — translation report

107 files: 40 in `contents/drawings/` (960–974, 976–989, 990–992, 994–999,
98, 99) and 67 in `contents/photos/` (2, 11, 12, 102–244 as listed in
`serije.json`).

## Files translated (107)

- With a description (107): every file of the batch. 69 carry DARC's
  marker, translated; the 38 without it are drawings 99, 988, 992, 994, 995,
  996 and photos 2, 11, 12, 102, 103, 104, 109, 117, 118, 123, 124, 125, 126,
  127, 135, 136, 143, 144, 145, 150, 167, 168, 190, 202–209, 216.

## Files left as they are (0)

- `TODO` only: none in this batch.

`alttext-check.py`: 107 files, 0 with findings. Line counts match the German.
No file ends in a newline except photo 168, which does in German too and keeps
it. The trailing spaces of 981 (after "Detaillierte Beschreibung:" and the
list items) and the trailing tab after the short description of photo 150
are dropped, as in slike_06–08.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

10 rows: the graph labels of 979–981, 988, 991, 994–999 (*Feldstärke,
Frequenz, Jahre, Sonnenflecken, Stunden, Zeit [Stunden], Distanz, Höhe, Winter
Tag … Sommer Nacht, fc bzw. foF2*); *Inversionsschicht / Duct / 3.ZF*; the
labels DARC set into photo 178; the headings of the German table in photo 145;
German printed on real objects (190, 212, 239); the Morse keys of 109
(*Handtaste, halbautomatische Taste, Squeeze-Taste, Tasthebel*); *Indianer*
(104); two rows of component and photo vocabulary (*Zeigermessgerät,
Drehwahlschalter, Drehgeber, Typenschild, Netzeinbaustecker, Schicht- /
Folienwiderstand, Spulenkörper, Grenzdaten, Akkupack, Schrumpfschlauch,
Mantelleitung, Ader, Luftfahrzeugkennzeichen, Hochdecker* …).

## Judgement calls

- Section labels as §14: *Kurzbeschreibung* → "Short description",
  *Ausführliche / Detaillierte Beschreibung, Detailbeschreibung* → "Detailed
  description", *Kurzfassung* → "Brief summary", *Kurze Zusammenfassung,
  Kurzzusammenfassung* → "Short summary", *Zusammenfassung* → "Summary",
  *Details* → "Details"; *Beschreibung* alone (175) → "Description".
  Numbering `1)`, `1.`, `-` (201) or none kept as in each file.
- Drawing labels that are German words: English, then the German in
  brackets, as slike_05–08 ("Mixer" ("Mischer"), "Driver" ("Treiber"),
  "Balanced modulator" ("Balance- modulator"), "1st filter" ("1. Filter"),
  "Inversion layer" ("Inversionsschicht")). Labels that read the same keep no
  bracket: "VFO", "XO", "BFO", "TCXO", "LNB", "PTT", "PA", "ALC", "TRX", "ANT",
  "RX", "MUF", "LUF", "Flux", "Duct", "Status". Value-only labels take a
  decimal point and no bracket ("2.4 GHz", "0.3 mW −5 dBm", "G 9.455 MHz",
  "4.7 nF", "5.6V", "2× 110 Ω 0.6 W", "13.2 V 4200 mAh", "AAA 1.5 V").
- *HF / ZF / NF* labels → "RF" ("HF"), "1st IF" ("1.ZF"), "2nd IF" ("2.ZF"),
  "3rd IF" ("3.ZF"), "AF" ("NF"); in a short summary that lists them
  unquoted (968) each gets its bracket; in running text (970 "HF-, 1.ZF-,
  2.ZF- und NF-Verstärker", 972 "NF‑Eingang", 98 "NF-Verstärker") the
  English abbreviation alone. The symbols *fosz*, *Ue*, *Us*, *Ua*, *UCE*,
  *Uq*, *Ri*, *Ik*, *Uk* stay.
- Photos: text printed on an object (makers' markings, type numbers, display
  readings, scale figures) kept exactly as printed, including the commas of
  "0,47 µF (X2) SH", "2 x 1,8 mH", "2 x 4,7 nF (Y2)" (242), "0,015 µF (X2)"
  (243), "1,5" (196) and the calculator display "0,007" (172, checked against
  `172.png`, which shows a comma); unquoted numbers take the decimal point
  (172's summary "0.007", 196's kΩ scale "0.5k", 143's "1.3, 1.5 … 2.5").
  English printed text ("Frequency Segment", "Full-scale model", "WORKING
  SIGN" …) unchanged. German words printed on a real object are kept with
  the meaning in brackets: "Sportgerät" (sports equipment) (190), "Rückkehr"
  (back) and "abbrechen" (cancel) (212, where the German itself calls them
  German labels); the label "Trafo  SU 60 b" / "Material-Nr. 31-024" (239)
  is a type marking and is kept unglossed. The labels DARC set into photo 178
  and the headings of the German table in photo 145 are treated like drawing
  labels (English, German in brackets).
- 244: the German quotes the temperature range as "−25 bis +85°C", but the
  label (`244.png`) prints "-25/+85°C"; the German *bis* is the describer's
  word, so the English quotes "−25 to +85°C" without a bracket.
- 996: the whole German text is wrapped in quotation marks; kept. Its axis
  labels "Distanz in kilo meter" / "Höhe in kilo meter" → "Distance in
  kilometres" / "Height in kilometres" with the German in brackets (no number
  before the unit, so the unit name stays). 994's ‚…‘ quotes → "…"; 995
  gives its labels unquoted and keeps them so, the German in brackets.
- 979, 980, 981: axis labels with units ("Field strength in V/m",
  "Frequency in Hz"); 981's "Feldstärke in V m" with the note that the "m"
  is under the "V" kept as written. Tick labels already written with a
  point ("0.1", "0.01", "1 000", "1,000" in 998) kept as the German has them;
  997's coordinate "(0,0)" kept.
- *Masse-Symbol / Massesymbol* → chassis symbol (966, 984, 989), *Masse‑/
  Erdungssymbol* → chassis/earth symbol (967), *Erdungssymbol / Erde-Symbol*
  on the filter labels → earth symbol (242, 244), as §14 and slike_08. 989
  "über ein Masse-Symbol geerdet" → "earthed via a chassis symbol", as
  written.
- *Spule* → inductor (966, 971), the windings of the transformer of 965 →
  coil, the air-wound coils of 171 → air-cored inductors (§4 *Luftspule*),
  photo 207's *Spulen* → inductors; *Ringspule* (193, a loop on an old
  instrument) → ring coil.
- *Zeigermessgerät* → analogue meter (967), §14 *Zeigerinstrument*;
  *Spannungsteiler* → potential divider (984, 986, 990), §5.
- 104: *Indianer* → "Native American", the neutral English term.
- 109: *Handtaste* → straight key, *halbautomatische Taste* → semi-automatic
  key, *Squeeze-Taste* → squeeze key, as amateurs name them in English.
- 190: *ARDF-Fuchs* → "ARDF fox", *Fuchsjagdsender* → foxhunt transmitter,
  *Wimpel* → pennant, *Zeitnehmer* → timing unit (§14 ardf).
- 167: "Luftfahrzeugkennzeichen (Rufzeichen)" → "aircraft registration
  (call sign)", as written.
- Slips translated as meant: 972 "links ein kleiner offener Kreis" (lower
  case, verbless) → "On the left a small open circle as the input"; 191
  "sternförfer Antrieb" (typo for *sternförmiger*) → "star-shaped drive";
  223 "hier ist eine … Metallspitze freiliegt" → "is exposed"; 208 "ein große
  Leistungstransistor" → "a large power transistor"; 999 "mit einem kleinen
  Abwärtsspitzen" → "with a small downward spike".
- All files were written in place in the repository; no drafts outside it.

## Suspected errors in the German descriptions

- 960 — "Zwei Dioden, D1 und D2, sind … in einer Brückenschaltung
  angeordnet", but `960.tex` draws a full-wave centre-tap rectifier (two
  diodes from the two ends of the secondary to a common node, the centre tap
  as return), not a bridge. Translated as written ("in a bridge circuit").
- 996 — the axis labels are given as "Distanz in kilo meter" and "Höhe in
  kilo meter", but `996.tex` prints "Distanz [km]" and "Höhe [km]".
  Translated as written.
- 244 — "−25 bis +85°C" is quoted as printed text, but the label prints
  "-25/+85°C" (see judgement calls).
- 98 — the description omits the "?" block and the VFO that feeds the
  (second) mixer in `98.tex`, and says the lines go "from the balanced
  modulator" to the CO and to the mixer; the CO feeds the balanced modulator.
  Translated as written.
