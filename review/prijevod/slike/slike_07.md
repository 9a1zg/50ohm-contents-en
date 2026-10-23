# slike_07 — translation report

107 files in `contents/drawings/` (734–839 and 74–84, as listed in
`serije.json`).

## Files translated (107)

- With a description (107): 74, 75, 77, 78, 80, 82, 83, 84, 734–773, 776–788,
  790, 791, 793, 795–820, 822–824, 826–839 (every file of the batch). Of
  these, 51 carry DARC's marker, translated: 82, 748, 763, 770, 771, 787, 791,
  793, 795–820, 822–824, 826–839.

## Files left as they are (0)

- `TODO` only: none in this batch.

`alttext-check.py`: 107 files, 0 with findings. Line counts match the German.
No file ends in a newline, in German and English alike; the trailing spaces
of 750, 828 and 834 are dropped, as in slike_06.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

13 rows: the air-layer labels of 734; the squelch labels of 737; the PSU
front-panel labels of 740; *Tote Zone / Sender / Empfänger* (741); *Frequenz
[Hz] / DVB-T2 Kanal 35 / 9 V Block*; the band-name labels *HF (KW)*, *VHF
(UKW)* (749, 829); *Isotroper Strahler / Pufferstufe / Eingangs- /
Ausgangsanpassung*; *HF_IN / HF_OUT*; *Biasversorgung / Leistungsversorgung /
Verknüpfungspunkt / Verzweigungspunkt / Verbindungspunkt*; the mixer and IF
labels of 80–84, 807, 808, 810; the limiter headings of 828; *Durchgang* →
cycle (738); the water-analogy parts of 835–837.

## Judgement calls

- Section labels as glossary §14: *Kurzbeschreibung* → "Short description",
  *Ausführliche / Detaillierte Beschreibung, Detailbeschreibung* → "Detailed
  description", *Kurzfassung* → "Brief summary", *Kurze Zusammenfassung,
  Kurzzusammenfassung, Kurz-Zusammenfassung* (831) → "Short summary",
  *Zusammenfassung* → "Summary", *Details* (838) → "Details", *Kurz: /
  Detail:* (807, 836) → "Short:" / "Detail:". Numbering `1)`, `1.`, `-` or
  none kept as in each file; 788's "DAusführliche Beschreibung" (typo) →
  "Detailed description".
- Labels that are German words: English, then the German in brackets, the
  bracket at the first mention in a paragraph and not repeated when the same
  paragraph names the label again (803, 810, 84: "RF", "1st IF" in the closing
  summary sentences), as in slike_05/06. A label already in brackets keeps the
  German in a second bracket: ("Mixer" ("Mischer")) (80). Labels that read the
  same in English keep no bracket: "Squelch", "Amplitude", "ON", "OFF", "VCO",
  "VFO", "BFO", "CO", "AGC", "DSB", "SSB", "LSB", "USB", "LW", "MF", "UHF" …
- *HF / ZF / NF* as labels → "RF" ("HF"), "IF" ("ZF"), "AF" ("NF"); "1.ZF",
  "1. ZF" → "1st IF" with the printed form in brackets. In running text
  *HF-Verstärker*, *ZF-Ausgang*, *NF-Stufe* → "RF amplifier", "IF output",
  "AF stage". *HF_IN / HF_OUT* (782–786) → "RF_IN" ("HF_IN"), as *NF_IN* in
  slike_05; 773 prints "RF_IN" already.
- 749, 829: the band names "HF (KW)" and "VHF (UKW)" → "HF" ("HF (KW)"),
  "VHF" ("VHF (UKW)"): the German everyday name only repeats the English one
  (bracket rule, as the frequency-range table of the course text); the bracket
  shows what is printed. In 829 the names are unquoted in the German and are
  treated the same way.
- Symbols and quantities stay: *f_OSZ*, *fosz*, *fZF*, *f_ZF*, *fe1*, *f_e1*,
  *U_HF*, *U_NF*, *U_BIAS*, *U_ss*, *U_eff*, *U_g*, *R_V*, *K_1*; "f_e1 und
  f_e2" (807) is a phrase label and becomes "f_e1 and f_e2" ("f_e1 und
  f_e2"); "Filtert fe2 raus" (808) → "Filters out fe2" ("Filtert fe2 raus").
- Numbers: decimal point throughout, also in the band tables of 749 and 750
  and the frequency lists of 831/832. Text already printed with a point is
  kept as printed: "13.8", "00.0" (740), "433.075000" (793), "0.4λ" … (788),
  and 830's "433.000 MHz", "1.240 GHz", "2.300 GHz", "955.000 GHz", which the
  German writes with a point. "73Ω" (788) keeps its missing space as quoted.
  "R3,6", "R5,7", "R2,3,6", "R5,7,8" (816, 817) are lists of resistor numbers,
  not decimals, and stay exactly. Units as symbols: "56 Ohm", "200 Ohm",
  "100 kOhm" → "56 Ω", "200 Ω", "100 kΩ" (771, 815). Compound values
  *0,1-μF-Kondensator*, *+13-V-Stromversorgung* → "0.1 μF capacitor", "+13 V
  power supply"; µ and μ kept as each file has them.
- *Spule* → inductor; the windings of a transformer and the coils of 797's
  transformer symbol → coils (§14). *Masse* / *an Masse* / *gegen Masse* →
  chassis / connected to chassis / to chassis; *Massezeichen* → chassis
  symbol; *Erdungssymbol* → earth symbol. *Schleifkontakt* → wiper.
  *Anschluss* of a component → lead, of a circuit → terminal or connection.
- 828: the heading *Verstärkung* over an amplified waveform → "Amplification"
  ("Verstärkung"), not "Gain"; *Begrenzung* → "Limiting" (§5).
- 748: "9 V Block" → "9 V block" ("9 V Block"), the label's own word; the
  running text's "9V" is kept as written.
- 773: the MMIC pins are called *Eingang 1* and *Ausgang 2/3/4* although 2
  and 4 go to chassis; translated as written ("output 2" …).
- 835–837 (water analogy): *Trog* → trough, *Rinne* → gutter, *Kanal* →
  channel, *Klappe* → flap, *Lager* → bearing, *Bügel/Steg* → bracket/web,
  *gebördelt* → beaded outwards, *Band-/Schellenbefestigung* → strap/clamp
  fixing (glossary §14).
- Slips translated as meant: 741 *merkierten*, 743 *spiegeldbildliche*, 77
  *mit zwei horizontalen Leiter*, 782–784 "rechts„Ausgangsanpassung“"
  (missing space), 788 "eine horizontale graue Linien, mittig die Aufschrift
  … trägt", 761 a missing full stop before "Parallel zu diesem Kondensator",
  786 a stray "v" after *Primärwicklung* and the space in "(R_2 )". 743's
  stray space before the final full stop of the short description is kept
  (" ."), like 652's "display,." in slike_06. 762 has no blank line between
  its two sections; kept.
- 735: the short description writes the antenna as "(8)" without quotes,
  unlike "("1")" … "("7")"; kept.

## Suspected errors in the German descriptions

- 748 — "Fünf Batterien" but only four sizes are named (LR41, AAA, AA, 9V),
  four labels are given, and the photo (`photos/168.png`, included by
  `748.tex`) shows four batteries. Translated as written ("Five batteries").
- 830 — the frequencies named do not match the drawing: "433.000 MHz" (the
  `830.tex` band edge is 430.000), "2.300 GHz" (2.320) and "up to 955.000
  GHz" (the highest value in the drawing is 951.000). Translated as written.
- 83 — the blocks with triangles are introduced as amplifiers (short
  description, and "(HF-Verstärker)", "(1. ZF-Verstärker)" in the detailed
  one), but later called "(2. ZF-Filter)", "zum 2. ZF-Filter, zum 1.
  ZF-Filter und zum HF-Filter" and "(NF-Filter)". Translated as written.
- 82 — the list names only two mixers (modules X and Y), and the last
  sentence then says "unter Z „BFO“" although no Z has been introduced;
  `82.tex` has three mixers labelled X, Y and Z. Translated as written.
- 77 — the short description speaks of "einem parallelen horizontalen
  Leiter", the detailed description of two horizontal conductors. Translated
  as written ("one parallel horizontal conductor").
