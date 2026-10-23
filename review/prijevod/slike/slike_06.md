# slike_06 — translation report

107 files in `contents/drawings/` (618–733 and 62–73, as listed in
`serije.json`).

## Files translated (107)

- With a description (107): 62–73, 618–628, 630–633, 635–639, 641–648,
  650–659, 662–687, 689–694, 697, 699–706, 710, 711, 713, 714, 716, 718, 720,
  725–733 (every file of the batch). Of these, 30 carry DARC's marker,
  translated: 64, 671, 674–679, 682–687, 689–693, 697, 699–706, 718, 720.

## Files left as they are (0)

- `TODO` only: none in this batch.

`alttext-check.py`: 107 files, 1 with findings: 680, "German words: und".
The word is inside the quoted German label in brackets, "Risk of short
circuit and reverse polarity" ("Kurzschluss- und Verpolungsgefahr"). The same
paragraph has the label ("Gleichstrom (I)"), and the checker strips a bracket
only up to its inner `)`, so its quote pairing slips, as with 501 in slike_05.
Not a real finding. No numbers are missing. Line counts match the German
(287 lines replaced). Only 690 ends in a newline (two, in fact), in German
and English alike.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

12 rows: the split-operation labels of 672/673; *Vorlaufend / Reflektiert /
SWR-Meter / Kabel / Dipolschenkel*; the colour-code labels of 665 and
*Hinweislinie*; the labels of 680/681 (*Hohe Spannung, Gleichstrom (I),
Lebensgefahr*, *Massesymbol*, *Strichmännchenfigur*); *Phasenwechsel /
Symbolzeit / Nebenausläufer / glockenförmige Kurve*; the network labels of
699/706; the speech-spectrum labels of 730; the ionosphere labels of 731–733;
*Positive Halbwelle / Periode / Jahre / Sonnenflecken im Mittel pro Monat*;
the symbol names of 694; the water-circuit parts of 667; *FPGA oder Software
/ De-Mapper / Präfix / Numeral / Suffix*.

## Judgement calls

- Section labels as glossary §14 and slike_05: *Kurz-Zusammenfassung* (64,
  677) → "Short summary", like *Kurzzusammenfassung*; *Kurz:* / *Detail:*
  (705) → "Short:" / "Detail:", as the earlier batches did (447). Numbering
  `1)`, `1.` or none kept as in each file.
- *Leuchtdiode* → "light-emitting diode" throughout (§4); *Amperemeter* →
  "ammeter"; *Spannungsmesser mit Wechselstromsymbol* (633) → "voltmeter with
  an AC symbol"; *Anschlusspunkt* → "terminal" (§14, slike_02); *Strahler* →
  "radiator", *Fußpunkt* → "base" (as 614); *Masse* → "chassis", *geerdet* /
  *Erde* → "earthed" / "earth".
- Labels that are German words: English, then the German in brackets, the
  bracket given at the first mention in a paragraph and not repeated when the
  same paragraph names the label again, as in slike_05 (e.g. "Channel decoder"
  ("Kanaldecodierer"), "Output" ("Ausgang"), "Transmitter" ("Sender")). Labels
  that read the same in English get no bracket: "Transceiver", "Remote",
  "Internet", "Router", "Mapper", "De-Mapper", "Numeral", "Suffix", "Anode",
  "Amplitude", "Diode", "LED", "Transistor", "Sporadic-E", "Region 1",
  "mech. 5/8 λ", "Ext. GPSDO", "ASK", "8QAM". "SWR meter" ("SWR-Meter") takes
  the bracket because the German spelling differs.
- 706: the labels "Server-netz", "internes Netz", "Internet-anschluss" are
  printed hyphenated and in lower case; the English keeps the lower case of
  "internal network" and the German in brackets as printed.
- 666: the letters "node" and "athode" are printed in the drawing to complete
  "A"/"K" into *Anode* / *Kathode*; kept exactly as printed, and "Kathode"
  itself → "Cathode" ("Kathode"). The large "K" stays a "K".
- Text printed on components and photos kept exactly, including the comma in
  "WIMA FKP 3 0,01/100-" and "WIMA 0,22 MKS 4 630-" (691), "21Ω-33Ω 22 kΩ
  10%", "50V / 1A" without a space. Drawing values that are only a number and
  unit take a decimal point and no bracket: "1.5 V" (626), "2.4 GHz",
  "2.256 GHz" (651), "⎓ 13.8 V" (680), "0.5 | 45°" (697, 702), "14074.3 kHz"
  etc. (718), "6.5 s" (720), 28.410/28.415/28.420/28.430 MHz (672, 673).
  "0.02 s" … "0.1 s" in 725 are already written with a decimal point.
- 694's "jeweils mit deutscher Beschriftung darunter" kept: "each with a
  German label below it" (true while the drawing is untranslated).
- 705: the quoted digit string "0  0  1  0  1  1" keeps its double spaces;
  the non-breaking hyphens of 702 ("Amplituden‑/Phasenangaben") and 705
  ("y‑Achse") are not reproduced, as in slike_05. The trailing spaces in 666,
  687 and 690 are dropped.
- 652: the short description ends "Anzeige,." (stray comma); kept as
  "display,.".
- 618, 621: "Parallel zur Leuchtdiode Widerstand" has a stray word; kept
  ("In parallel with the light-emitting diode resistor"). The `.tex` puts the
  meter across the LED.
- 731: "bis 10" → "up to 10" ("bis 10"); *Kennzeichnung* → "marking".
- 667: *Aggregat* → "unit", *Absperrhahn* → "stopcock", *Schaufelrad* →
  "paddle wheel".
- 633: the short description's "„I_2“ auf der Innenseite des Außenleiters
  („I_2“)" names I_2 twice; kept.
- Typos translated as meant: 635 *Antennensymboi*, 641/653 *zuammengeführt*,
  690 *bauteil*; 733 "führen zwei … Linien … und endet" (number slip) → "lead
  … and end".

## Suspected errors in the German descriptions

- 620 — the short description says voltmeter; the detailed description says
  a circuit symbol labelled „A“ for an ammeter. `620.tex` draws `rmeter, t=V`,
  a voltmeter. Translated as written.
- 646 — the short description has the arrow in the lower conductor pointing
  to the left, the detailed description pointing to the right. Translated as
  written.
- 635 — the detailed description calls the last block before the loudspeaker
  "ein nach rechts zeigendes Dreieck (Filter)". A triangle is the amplifier,
  and the short description and `635.tex` (`ampshape`) have an amplifier
  there. Translated as written.
- 642–645 — the descriptions name the blocks „Quellendecodierer“ and
  „Kanaldecodierer“, but in these transmit chains (a "Mapper" with two
  outputs) the drawings (`642.tex`–`645.tex`) say *Quellencodierer* and
  *Kanalcodierer*. Translated as written ("Source decoder" ("Quellendecodierer")
  …), so the bracket shows the description's word, not the drawing's.
- 729 — "spitzen Maxima und tiefen Minima im Abstand von etwa 1 Jahr": the
  cycle shown is the roughly eleven-year solar cycle, which the course
  captions also name. Translated as written ("about 1 year").
- 73 — the minus terminal is written „—“ (em dash) in the detailed
  description and "–" in the short one. Kept as written.
- 67, 68, 69, 70 — the short description writes "−" (minus sign) and the
  detailed description "–" (en dash). Kept as written.
