# slike_08 — translation report

107 files in `contents/drawings/` (840–959 and 85, 86, 90, 93, 94, 96, as
listed in `serije.json`).

## Files translated (107)

- With a description (107): 85, 86, 90, 93, 94, 96, 840–847, 850–852,
  854–870, 872–886, 891–899, 903–911, 913–918, 922–930, 933, 935–946,
  948–959 (every file of the batch). Of these, 96 carry DARC's marker,
  translated; the 11 without it are 94, 96, 847, 866, 876, 879, 905, 906,
  936, 937, 952.

## Files left as they are (0)

- `TODO` only: none in this batch.

`alttext-check.py`: 107 files, 0 with findings. Line counts match the German.
No file ends in a newline, in German and English alike; the trailing spaces
of 924 (after "Detaillierte Beschreibung:" and the list items) are dropped,
as in slike_06/07.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

9 rows: the propagation labels of 865, 867, 870, 872–874 (*Refraktion,
Scheinbare Reflexion, Kurzer/Langer Weg, Sommertag/Wintertag/Nacht,
Distanz*); the spectrum ranges of 847; the block-diagram labels *RX-/TX-Mischer,
Treiber, Balance-modulator, 1./2. Filter, Digitale Signalverarbeitung* with
*Umschalter* → changeover switch; the semiconductor and component labels of
858, 922, 923, 958; *Senderausgangsleistung / Tiefpass / Messung von
unerwünschten Aussendungen / Leistungsoptimum / Eingangssignal /
Frequenzgemisch / Erde*; *Drehwinkel φ / Bogenmaß φ / Zeit / 90° O / 90°
Zenit*; the *1. OW 2 Harm.* labels; *30 St. / NF/BB / 70 cm Band / 10 m (ca.
20 kilo meter) / tech., phys.*; a descriptive row (grey gradient bar, cell
array, down-lead, mixer circle, pair of plates).

## Judgement calls

- Section labels as §14: *Kurzbeschreibung* → "Short description",
  *Ausführliche / Detaillierte Beschreibung, Detailbeschreibung* → "Detailed
  description", *Kurzfassung* → "Brief summary", *Kurze Zusammenfassung,
  Kurzzusammenfassung* → "Short summary", *Zusammenfassung* → "Summary",
  *Details* → "Details", *Kurz: / Detail:* (860) → "Short:" / "Detail:".
  Numbering `1)`, `1.` (941) or none kept as in each file.
- German-word labels: English, then the German in brackets at the first
  mention in a paragraph, as slike_05–07; a label already inside brackets
  gets a second bracket (874: ("Summer day" ("Sommertag"), …)). Labels that
  read the same in English keep no bracket: "Diffusion", "Germanium",
  "Radar", "Transceiver", "Amplitude", "Azimuth" and "Elevation" (876, printed
  in English), "tech." and "phys." (956), "MWS", "CO", "VFO", "BFO", "TRX",
  "PA", "ALC".
- *HF / ZF / NF* labels → "RF" ("HF"), "IF" ("ZF"), "AF" ("NF"); "1.ZF 50
  MHz" → "1st IF 50 MHz" ("1.ZF 50 MHz") (90), "1. ZF" → "1st IF" (93);
  "NF/BB" → "AF/BB" ("NF/BB") (951), as "NF/Basisband" in slike_02. In
  running text *HF-Verstärker* → RF amplifier. The symbols *fZF*, *fosz*,
  *f_T*, *U_HF*, *U_NF*, *U_th*, *U_Z*, *I_S* stay.
- 868, 869, 918: "1. OW 2 Harm." … kept as printed, with "(1st to 3rd
  overtone, 2nd to 4th harmonic)" after the list, and "1 Harm." (1st
  harmonic), following 1008 (slike_01). 869's "drei Oberwellen (2., 3. und
  4. Harmonische)" → "three overtones (2nd, 3rd and 4th harmonics)", the
  §5 trap; the unnumbered *Oberwellen* → harmonics; "NA" unglossed, as 1008.
- 866: the alt text spells the units out ("80 meter (ca. 200 kilo meter)");
  units after a number become symbols ("80 m (approx. 200 km)"), the German
  quote in brackets as the alt text gives it. *ca.* → approx.
- Numbers: decimal point throughout ("38.666 MHz", "4.7 kΩ", "0.6 V",
  "8998.5 kHz", "3.455–30.455 MHz", "≥ 0.05 · λ_max", "430.0075 MHz").
  "144.816.0" (915) is printed with points and kept. "Ohm" after a number →
  "Ω" (937), "R_L in Ohm" → "in ohms" (unit itself meant). Compounds
  *1-µF-Kondensator*, *50-Ω-Leitung* → "1 µF capacitor", "50 Ω line".
  Hyphens in "430 - 434 MHz", "3-30 MHz", "28-30" and the en dashes elsewhere
  kept as each file has them.
- *Spule* → inductor (also the drawn loops of 882, 891–899, 925–927), the
  windings of a transformer and the ratio coil "ü = 1 : 7" → coil (946, 954,
  955), as §14. *Induktivität* → inductance where the German uses it (926,
  and "(Induktivität)" glosses in 883, 884, 948, 954). *Drehkondensator* →
  variable capacitor (840). *Masse-Symbol* → chassis symbol,
  *Erdungssymbol* → earth symbol (851); *Masseanschluss* → chassis
  connection. *Sammelschiene* → busbar, *Strang* (solar cells) → string,
  *Trägerstange* → boom, *Bezugsleitung* → reference conductor (§14).
- 847: *10_–15*, *10_6* … kept in the alt text's notation; the stray spaces
  in '"1 fm" (unten) ,' and '" 1 km"' kept, like earlier batches.
- 878: *Drehwinkel φ* is the angle of a rotating phasor here, not the beam
  heading of §14 → "Angle of rotation φ"; *Bogenmaß φ* → "Radian measure φ",
  the summary's "im Bogenmaß" → "in radians". *Pfeile* stay arrows.
- 911: the two-line label "Digitale Signal-" / "verarbeitung" given line by
  line ("Digital signal" / "processing"), the summary quoting it as one
  label with its line-break hyphen in the bracket.
- 913: *Mischerkreis* → "mixer circle" (the circle symbol of the block
  diagram, as the blocks of 90 "mit Kreisen"). 954: *Abstieg* → down-lead.
- 916, 917: label *Tiefpass* → "Low-pass filter" ("Tiefpass"), the glossary
  term.
- Slips translated as meant: 863 *Basenanschluss* (base terminal); 946 "die
  oberen Leitungen hinter D1 und aus der unteren Leitung (hinter D2)
  treffen sich" → "the upper line after D1 and the lower line (after D2)
  meet"; 866's verbless "von der aus roter Pfeil mit … beschriftet" → "from
  which a red arrow is labelled …"; 892 "links ist mit „E“ beschriftet" →
  "the left-hand side is labelled "E""; 939 "jeweils … zwei Kondensatoren"
  (one capacitor at each of two nodes) → "two capacitors …, one at each";
  941 "unlabeled" (an English word in the German) → "unlabelled".
- These translations were briefly drafted in two scratch files before being
  written into the repository files, and the scratch files were deleted;
  nothing outside the repo remains.

## Suspected errors in the German descriptions

- 866 — the yellow arrow is given as "80 meter (ca. 200 kilo meter)", but
  `866.tex` prints "80 m (ca. 100 km)" and draws that arrow in DARCorange,
  not yellow; "Mittelwelle, 160 meter (200 kilo meter)" drops the "ca." the
  drawing has. Translated as written.
- 863 — "der interne Pfeil am Emitter zeigt zum Basenanschluss" describes a
  PNP symbol, but `863.tex` draws an `npn` transistor (arrow pointing away
  from the base); the current arrows are also drawn in DARCred, not orange.
  Translated as written.
- 90 — the block after "2.ZF 9 MHz" is described as "NF 455 kHz"; `90.tex`
  does label that filter "NF" with "455 kHz" beside it, so the alt text
  follows the drawing, but 455 kHz is a third IF, not AF (compare 913's
  "ZF 455 kHz"). Translated as written; a possible drawing error.

## Provjera

107 files compared with the German (`e8a5481~1`): 98 left as they are,
9 changed; glossary rows unchanged (the 9 new §14 rows checked against §2,
§3, §4, §5, §6, §7, §10 and the earlier §14 rows, no conflicts).
`alttext-check.py --rev e8a5481~1`: 107 files, 0 with findings. No numbers
missing; DARC's marker, section labels, bracketed German labels, decimal
points and units as symbols all as the brief and §14 have them. The
suspected errors in 866, 863 and 90 checked against the `.tex` files
(`80 m (ca. 100 km)` in DARCorange, `ca.` on the medium-wave label; `npn`
with DARCred current arrows; filter `l_=NF` with "455 kHz") and confirmed.

- 870, 918, 955: *doppelseitiger (Maß)pfeil* "double-sided … arrow" →
  "double-headed … arrow", as elsewhere in the batch (948, 954).
- 852: "horizontal black line (line)" (*Linie (Leitung)*) → "(transmission
  line)", §9.
- 874: "above a blue earth's surface" → "above the earth's surface, drawn in
  blue".
- 935: "The arrows standing orthogonally on the waves" → "The arrows
  perpendicular to the waves".
- 944: *mit den Legenden U (blau) …* "with the legends U (blue)" → "with the
  legend entries U (blue)".
- 951: "two capacitors … (small pairs of plates) to a short upper auxiliary
  line" → "…, connected to a short upper auxiliary line" (*gegen*).
- 958: "two black leads lead away" → "two black leads run away".
- Checked and kept: "Diagram of a block diagram" (913, 93) and "Shown is"
  as the German; 868/869/918's bracketed reading of the *OW / Harm.* labels
  (1008 precedent); 866's quotes with units as symbols and the German in
  brackets; "Azimuth"/"Elevation" unbracketed in 876 (printed in English).
