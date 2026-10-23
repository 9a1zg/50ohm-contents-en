# slike_05 — translation report

107 files in `contents/drawings/` (479–617 and 48–61, as listed in
`serije.json`).

## Files translated (107)

- With a description (107): 48–53, 55–57, 61, 479–484, 486, 488–491,
  495–527, 529, 531, 535–538, 541–546, 549, 554–563, 576–580, 586–595,
  597–599, 601, 607–617 (every file of the batch). Of these, 11 carry
  DARC's marker, translated: 486, 488, 489, 490, 491, 496, 497, 498, 499,
  501, 577.

## Files left as they are (0)

- `TODO` only: none in this batch.

`alttext-check.py`: 107 files, 1 with findings — 501, "German words: und".
The word is inside the quoted German label in brackets, "Control and
monitoring signals" ("Steuer- und Kontrollsignale"); the checker strips
the bracket `("Audio (NF) RX")` only up to the inner `)`, so its quote
pairing slips and the bracketed label is counted as running text. Not a
real finding. No numbers missing. Line counts are the same as in the
German (233 lines replaced); no file of the batch ends in a newline, in
German or English.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

7 rows: the labels of drawing 49 (*Wickel / Metallbeläge / Dielektrikum*,
*Lage / Schicht*); the labels of 488, 496, 541, 591–594, 615
(*Audioverstärker, NF_IN, HF-Diode, Anpassglied, Leistung, Lampe_1*); the
labels of 501; *Anschlussmarke / Lötöse / Zellensymbol / Kontaktbrücke /
Sammelleitung / Bezugsschiene / Masse-Schiene*; the connector parts of
608–611; the radio display of 578–588; *Träger / Trägerstab /
Querelemente / Schleifenelement* of the Yagi-Uda drawings.

## Judgement calls

- Section labels as glossary §14: *Kurzbeschreibung* → "Short
  description", *Ausführliche / Detaillierte Beschreibung,
  Detailbeschreibung* → "Detailed description", *Kurzfassung* → "Brief
  summary", *Kurzzusammenfassung / Kurze Zusammenfassung* → "Short
  summary", *Zusammenfassung* → "Summary". Numbering `1)` / `2)` or none
  kept per file; 517's unlabelled "2)" and 563's ") Ausführliche
  Beschreibung" (digit missing) kept as they are; the line breaks after the
  labels in 498 and the bullet lists of 490 and 498 kept.
- 488: the net labels $\mathrm{NF}_\mathrm{IN}$ / $\mathrm{NF}_\mathrm{OUT}$
  are typeset as symbols in `488.tex`, but *NF* is the German abbreviation
  that the house style turns into AF, so they are treated as labels:
  "AF_IN" ("NF_IN"). "f_OSZ" (500), "f_T", "U_BE", "V_S", "E_1"…, "R_1"…
  stay as symbols.
- Labels that are German words: English, then the German in brackets, the
  bracket not repeated when the same paragraph names the label again:
  "Audio amplifier" ("Audioverstärker"), "RF diode" ("HF-Diode"),
  "Antenna" ("Antenne"), "Network" ("Netzwerk"), "Power" ("Leistung"),
  "Matching network" ("Anpassglied"), "Roll" ("Wickel"), "Metal foils"
  ("Metallbeläge"), "Dielectric" ("Dielektrikum"), "Lamp_1" ("Lampe_1"),
  "RF" ("HF"), "IF" ("ZF"), "AF" ("NF"). 501's labels that already contain
  a bracket take the German in a second bracket: "Audio (AF) RX" ("Audio
  (NF) RX"), as glossary §14 ("AF" ("NF")). Labels that read the same in
  English get no bracket: "Demodulator" (590), "Internet" (542), "mech. >
  λ/4" (563), "SWR", "MHz:", "SWR:".
- 501: *Steuer- und Kontrollsignale* → "Control and monitoring signals"
  (*Steuer-* = control, *Kontroll-* = the feedback the remote_station text
  describes).
- Decimal point in labels and values without a bracket (a label that is
  only a number and unit): "6.9 pF", "3.3 kΩ", "5.6 V", "0.3 A", "2.7 kΩ",
  "0.03 µs/Div.", "2× 110 Ω 0.6 W", "4.7 nF", the SWR scale "2.5, 3.0 …
  5.5 MHz", "approx. 1.3". 577's "330 Ohm" / "10 kOhm" → "330 Ω" /
  "10 kΩ". The display reading "144.315.0" kept exactly as printed.
- *Masse* → "chassis" (chassis symbol, chassis rail, chassis node, chassis
  point); *Erdungssymbol* → "earth symbol", *geerdet* → "earthed" (615).
- *Spule* → "inductor"; *Spule (Induktivität)* (491, 497) → "coil
  (inductor)", as slike_04; the windings of 489's transformer → "coils",
  as glossary §14 (slike_02); 50's physical coil → "coil".
- *Reihenschaltkreis / Schaltplan in rechteckiger Leitungsführung* →
  "series circuit / circuit diagram drawn with right-angled wiring", and
  *Gezeigt ist ein Blockschaltbild …* → "Shown is a block diagram …", as
  slike_02/03/04; *Baugruppen* → "modules"; *Generator* (500, 524) →
  "generator", *(Oszillator)* → "(oscillator)", each as the German has it.
- *Leiterbahn* (489, 498) → "conductor track" (§14, slike_04);
  *Sammelschiene* (499) → "busbar"; *Sammelleitung* → "common line";
  *Schiene* → "rail"; *„+“-Bus* → "+" bus.
- 51, 613: *Träger / Trägerstab* of the Yagi-Uda → "boom" (§9), the
  technical term for what the German calls the support.
- *Flanken*: 57 (a pulse on the scope) → "edges" (§14 *Flanke (Rechteck)*),
  612 (an emission spectrum) → "slopes" (§14 *Flanken (Filter)*).
- *spiegelbildlicher Verlauf nach unten* (597–601) → "its mirror image
  below"; *an- und abschwellende Amplitude* (607) → "rising and falling
  amplitude"; *Fußpunkt* (614) → "base".
- 607 begins its short description with lower-case "oberer Teil:"; kept
  ("upper part:").
- 48: the short description has no closing full stop; none added.
- Not reproduced: the trailing spaces at the end of 483 and after
  "Detailbeschreibung:" in 490, the double spaces in 483, 484, 502, 546,
  559, and the non-breaking hyphens in 486 ("P‑N") and 608
  ("Bajonett‑Nuten"). 497's English-style quotes “+” → "+".
- Typos translated as meant: 483/484 *zugeodneten*, 506 *verikalen*,
  525 *aus aus*, 597–601 *spiegeldbildlichem*, 615 *dieser Leiters*.

## Suspected errors in the German descriptions

- 482 — "eine nicht näher bezeichnete horizontale Achse": the second axis
  is the vertical one (the short description, and 479–481, say so).
  Translated as written ("a horizontal axis that is not labelled further").
- 523 — "alle Bauteile sind in Reihe miteinander verbunden", although the
  same description puts the inductor and the variable capacitor in
  parallel. Translated as written.
- 535–538 — "Darüber steht der Buchstabe "I"", then "es sind keine Zahlen-
  oder Textbeschriftungen vorhanden"; the letter is a label. Translated as
  written.
- 562 — "eine Verbindung zum Außenmantel des abgehenden Koaxialkabels":
  the sheath is the insulating jacket; electrically the connection is to
  the outer conductor (screen), as the same description says a sentence
  later. Translated literally ("outer sheath").
- 614 — "eine durchgehende gestrichelte vertikale Linie": continuous and
  dashed at once. Translated as written.
- 49 — "zwei mit „Metallbeläge“ beschriftete Schichten …, die jeweils auf
  diese Schichten überragende Lagen aufgebracht sind. Diese an den Seiten
  überragenden Schichten sind mit „Dielektrikum“ beschriftet": *Schichten*
  is used both for the metal foils and for the projecting dielectric
  layers, so the sentence is hard to follow. Translated as closely as
  English allows.
- 479 — "einem dachförmigen Bereichen" (case slip, as 477); 576 "verbunden
  über zwei parallel geschalteten 110-Ω-Widerständen" (case slip);
  harmless.
- 563 — the second label lacks its digit (") Ausführliche Beschreibung").
