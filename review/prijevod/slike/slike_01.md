# slike_01 — translation report

107 files in `contents/drawings/` (100–110, 1000–1100 as listed in
`serije.json`).

## Files translated (65)

- With a description (55): 100, 102, 103, 104, 105, 106, 108, 109, 110,
  1000–1008, 1010–1026, 1036–1040, 1042–1056.
- DARC's marker only, nothing else in the file (9): 1027–1035 — the marker
  line translated, the empty rest kept.
- Marker followed by `TODO` (1): 1057 — marker translated, `TODO` kept.

## Files left as they are (42)

- `TODO` only (39): 1058–1095 and 1100.
- Empty files (3): 1096, 1097, 1098 — nothing to translate.

`alttext-check.py`: 107 files, 0 with findings. Line counts are the same as
in the German (178 lines changed, 178 replaced), and so is each file's final
newline or its absence.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

5 rows: the alt-text section labels; *Teilbild / Abbildung „a.“ /
Allgemein*; *offener Anschlusskreis / Anschlussklemme / Knoten*; *Wellenlinie
/ Doppelpfeil / Hilfslinie / Pfeilspitze*; the "1. OW" labels of 1008.

## Judgement calls

- Section labels: *Kurzbeschreibung* → Short description; *Ausführliche /
  Detaillierte Beschreibung, Detailbeschreibung* → Detailed description;
  *Zusammenfassung* → Summary; *Kurze Zusammenfassung, Kurzzusammenfassung,
  Kurz-Zusammenfassung* → Short summary; *Kurzfassung* → Brief summary;
  *Details* → Details. The German numbering style (`1)`, `1.`, none) kept per file.
- Quotation marks: straight "…", as the English course text uses throughout.
- German drawing labels: English first, capitalised as a label, then the
  German in brackets ("Short path" ("Kurzer Weg"), "Real voltmeter"
  ("Reales Spannungsmessgerät"), "Power" ("Leistung"), "Antenna tuner"
  ("Antennentuner"), "RF" ("HF"), "1st mixer" ("1. Mischer") …). Where a
  paragraph names the same label again, the bracket is not repeated
  (1048 last sentence, 1055 "RF", "IF").
- Labels with a decimal comma ("f = 3,5 MHz" in 1042, "f_T = 7,100 MHz",
  "7,101 MHz" in 1056, "–0,4 V" in 109, "31,7 MHz" in 102, legend of 1010)
  written with a decimal point, as the label will read once the drawing is
  translated (DECISIONS.md); 1010's legend already prints 3.6 / 7.1 / 14.15.
- 1002: *Physikalische / Technische Stromrichtung* → "Electron flow" /
  "Conventional current flow" (glossary), German in brackets.
- 1008: "1. OW" … "4. OW" kept as printed with "(1st to 4th overtone)"
  after them — *overtone* keeps the German numbering right (the 1st
  Oberwelle is the 2nd harmonic); the summary's *1.–4. Oberwelle (OW)* →
  "1st to 4th overtones (OW)". The unnumbered label "Oberwellen (OW)" →
  "Harmonics (OW)", matching the course caption of 1008. "NA" (spurious
  emissions) kept as printed, not expanded, as the German does not.
- 1003: "zum Netzteil" → "to power supply"; "zum TX" → "to TX", German in
  brackets since the drawing shows both.
- 1023: "Hochpass" → "High-pass" — the emphasised "H" still works in English.
- 1049: *Ausleger (Boom)* → "arm (boom)", later "arm".
- 1051: *Masse-/Erdungssymbol* → "chassis/earth symbol" (glossary *Masse*
  → chassis).
- 1016: *Spule (Induktivität)* → "coil (inductor)", to avoid "inductor
  (inductance)".
- 1020: *Teilbild* → "Panel".
- *Leitung* in a drawn circuit → "line"; *Leiter* → "conductor"; *Knoten*
  → "node".

## Suspected errors in the German descriptions

- 1011 — describes "a completely black image with no content", but
  `1011.tex` plots NOAA absorption data as a world map (caption: highest
  frequency affected by 1 dB of absorption) — the description was
  evidently made from a failed render. Translated faithfully.
- 1046 — "im Winkel vom 120°" (*von*) and "Ein nahezuförmiger Kreis" (word
  missing: *nahezu kreisförmiger*) — translated as meant ("A nearly circular
  outline").
- 1038 — the German contains the English word "unlabeled" ("ein unlabeled
  rechteckiger Block") — translated "unlabelled".
- 1022 — the short description ends "bis zum Ende der horizontalen Linie",
  the detailed one "der horizontalen Achse" — translated as written.
- 1020 — "nahe der rechten oberen Bereich" (grammar) — harmless.
- 1054 — not the description but the course caption: drawing 1054 shows a
  Π and a T attenuator, while the German caption in
  `vorverstaerker_daempfungsglied` reads "Vorverstärker im
  Überlagerungsempfänger" (English: "Preamplifier in a superhet").

## Provjera

Checked all 107 files against the German at `d0e7d7c~1`: 65 translated
files compared sentence by sentence (55 full descriptions, 9 marker-only,
1 marker + `TODO`), 42 `TODO`/empty files confirmed untouched. 5 files
changed, 7 lines. `alttext-check.py --rev d0e7d7c~1`: 107 files, 0 with
findings.

- 1050 — *für die Anregungen „f“, „2·f“ …* "for the excitations" → "for
  feeding at", as glossary §14 *Anregung (Dipol)* → "fed at".
- 1007, 1014, 1023 — *Anschlussklemme(n)* "connecting terminal(s)" →
  "terminal(s)", as the glossary row of this batch (§14) and 1003, 1017.
- 1003 — *Schematischer Plan* "Schematic plan" → "Schematic diagram"
  (natural English).

Left as translated: the 1008 "overtone"/"Harmonics (OW)" pair (follows
§14 and the course caption), 1049 "arm (boom)", 1053 "Π network", and the
suspected German errors listed above, which are reported, not fixed.
