# nea_strom_spannungsversorgung_2 — translation report

Chapter "Strom- und Spannungsversorgung (2/2)" (Power supplies, part 2):
4 sections, each with its slides, and 7 solutions. 15 files:

- `contents/sections/` and `contents/slides/`: `schaltnetzteil_2.md`,
  `spannungsstabilisierung.md`, `fernspeiseweiche.md`, `sicherungen.md`.
- `contents/solutions/`: `AD315.md`–`AD321.md`.

`revizija-guard.py --brojevi`: 15 files checked, *struktura netaknuta*.
German-word grep: no hits outside picture and photo idents
(`a_Längstransistor 2N3055 auf Kühlkörper`, `a_Stabilisierung mit
Z-Diode`). Files without a final newline in the German keep it that way;
sections/spannungsstabilisierung.md keeps its trailing two spaces.

Embedded questions looked up in English and the prose aligned with them:
AD311–AD325, EK204 (e.g. AD311 "pulse-width modulator", AD313 "switch-mode
power supply", "poorly suppressed", AD316/AD319/AD320 "linear voltage
regulator", AD317 "12 V fixed voltage regulator", "almost zero volts",
AD321 "voltage stabiliser", AD322 "bias tee (remote DC feed)", AD325
"current rating", EK204 "same current rating and the same tripping
characteristic", "miniature fuse").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

14 rows: *Schaltzeit / Energietransport / Rückführung / Steuerblock*,
*Netzspannungspotentiale / Netztrennung*, *Störspektrum / (ungenügend)
entstört*, *EMV-Filter / Funkentstörfilter / leitungsgebundene Störungen*,
*Merke:*, *Referenzspannung / Spannungsreferenzquelle / Regelverhalten*,
*diskret aufgebaute Spannungsstabilisierung / linear geregelt*,
*systembedingt*, *Fernspeiseweiche oder englisch BIAS-T*, *abgesetzter
Vorverstärker / Empfangskonverter*, *Gleichspannungsversorgung(sleitung) /
Versorgungsgleichspannung / DC-Anschluss / DC-Seite*, *HF-Nutzfrequenz*,
*Feinsicherung / TR5 / Diazed / Neozed / Hochspannungssicherung*,
*kommerzielle Funkgeräte*.

## Added to `DECISIONS.md`

None. The one choice of note (the BIAS-T gloss) applies the existing
bracket rule and is recorded in the glossary row.

## Judgement calls

- All files: *Festspannungsregler* → fixed voltage regulator, *Linearspannungsregler / linearer Spannungsregler* → linear voltage regulator, *Längstransistor* → series pass transistor, *Z-Diode* → Zener diode, *Vorwiderstand* → series resistor, *Verlustleistung* → power dissipation (glossary §4, §5, AD315–AD321); *Spannungsstabilisierung* as a circuit → voltage stabiliser (AD321), as a technique → voltage stabilisation; *Lösungsweg / gegeben / gesucht* → "Solution / given / required", as in earlier units.
- schaltnetzteil_2: *Dies bedeutet, dass der leitende Zustand des Schalters verändert wird* → "the time for which the switch conducts is varied": a literal "the conducting state is varied" says nothing in English; the duty cycle is what the German means (pulse-width modulation, AD311).
- schaltnetzteil_2: *Das Schaltnetzteil wurde in Klasse N und E schon einführend erklärt* → "has already been introduced in Classes N and E", as earlier units write "Classes N and E".
- schaltnetzteil_2: *Merke:* → *Remember:*, as stromkreis and kondensator_2; *Die Drossel T darf keine Transformatorfunktion … bewirken* → "must not act as a transformer for the AC mains voltage"; margin note *EMV Filter = Funkentstörfilter gegen leitungsgebundene Störungen* → "EMC filter = radio interference suppression filter against conducted interference".
- schaltnetzteil_2 slides: *Elektronischer Schalter E regelt eine konstante Ausgangsspannung* → "regulates to a constant output voltage"; captions "230V" / "230 V  AC" → "230 V" / "230 V AC", the unit symbol spaced after the number, as in the previous unit's slides.
- spannungsstabilisierung: *systembedingt* → "by the very nature of the system"; *eine optimale elektronische Regelung* → "optimised electronic control"; *sonst kann es zu unerwünschten Schwingungen im Regelverhalten der Schaltung kommen* → "otherwise the regulation of the circuit can break into unwanted oscillation".
- spannungsstabilisierung tip: *Low-Drop-Spannungsregler* → low-dropout (LDO) regulators (glossary §14); *Masseleitung des Festspannungsreglers* → "chassis lead of the fixed voltage regulator" (glossary §13 *Masseleitung*), though an English data sheet would say "common" or "ground" pin.
- spannungsstabilisierung slides: *Ausgelegt als IC* → "Designed as an IC"; *Abhilfe* → "Remedy"; `\num{0,14}`, `\num{0,36}` → `\num{0.14}`, `\num{0.36}`.
- fernspeiseweiche: *eine Fernspeiseweiche oder englisch BIAS-T* → "a bias tee (remote DC feed)": the German gloss only gives the English term (bracket rule), and the bracket carries the descriptive name AD322 uses; the caption of picture 399 likewise; afterwards plain "bias tee" for both *Fernspeiseweiche* and *BIAS-T*.
- fernspeiseweiche slides: the bullet *Englisch: BIAS-T* → "Also called a remote DC feed": the bullet's job (naming the other-language term) has no English counterpart, and dropping it would leave an empty list item; the alternative English name keeps it useful. Captions *BIAS - T* → "Bias tee".
- fernspeiseweiche: *wirkt für Hochfrequenz hochohmig* → "presents a high impedance at RF" (glossary §14 *hochohmig*); *gegen Masse* → "to chassis" (glossary §14); *Blindwiderstand kleiner 1 Ohm* → "reactance is less than 1 Ω" (unit symbol after a number); *Gleichspannungsseite* (glossing *DC-Seite*) kept as "(the DC voltage side, e.g. 12 V)".
- fernspeiseweiche slides: *Gleichspannung wird über die Induktivität auf den Innenleiter geführt und koppelt HF ab* → "… through the inductor, which blocks RF": the subject of *koppelt HF ab* is the inductor, as the section says.
- fernspeiseweiche indepth: photo caption *BIAS - T Platine - mit KiCAD erstellt* → "Bias tee circuit board – designed with KiCad", the program's own spelling.
- sicherungen: *im Kapitel Netzgerät im Klasse N Kurs* → "in the chapter on the power supply unit in the Class N course" (chapter titles not yet translated; the reference stays descriptive); *defekte Sicherung* → "blown fuse"; *Schmelzsicherungen* → fuses (glossary §12, §14), so "miniature fuses, a subgroup of fuses"; *kommerzielle Funkgeräte* → "commercially made radios".
- sicherungen slides: wording and table aligned with the identical content of netzgeraet_1 (section and slides): "fast-acting / medium time-lag / time-lag", "Breaking time at ten times the rated current", "Characteristics of miniature fuses", "fuses of the same type".
- AD319: *die überschüssige Spannung in Wärme umgesetzt* → "the excess voltage is converted into heat", as written (see errors).
- AD320, AD321: `0{,}36`, `0{,}14` → `0{.}36`, `0{.}14`, as in earlier units.

## Suspected errors in the German original

- slides/spannungsstabilisierung.md (AD318 solution) — "$I = \frac{U_{\mathrm{in}}}{R_L} = \frac{\qty{5}{\volt}}{\qty{10}{\ohm}}$": the load current is $U_{\mathrm{out}}/R_L$; the value used (5 V) is the output voltage, so only the symbol is wrong. Kept.
- sections/schaltnetzteil_2.md — "Die Veränderung der Schaltzeit bewirkt zusätzliche Störsignale": the interference comes from the switching itself (the fast edges at the switching frequency and its harmonics, a line every 30 kHz, as the next sentences say), not from varying the switching time. Translated as written.
- slides/schaltnetzteil_2.md — under the heading "Galvanische Trennung" the bullets say the isolation keeps the circuit's interference away from the mains side; in the section that is the job of the mains low-pass filter, while galvanic isolation keeps mains potentials away from the output. Kept.
- sections/fernspeiseweiche.md — "Vorverstärkers (LNB)" calls an LNB (low-noise block downconverter) a preamplifier, and "Vorverstärker oder Empfangskonverter (LNA)" labels a converter as an LNA (low-noise amplifier). Kept.
- solutions/AD319.md — "die überschüssige Spannung in Wärme umgesetzt": it is power (the excess voltage times the current) that is converted into heat. Kept.
- Typos with no effect on the English: sections/schaltnetzteil_2.md "zum … Wechselspannungsnetzes", "Funkentstörfilter Filter" (photo 242), missing full stop after "[ref:a_EMV_Filter2]"; slides/schaltnetzteil_2.md "Netzspannungseite"; sections/spannungsstabilisierung.md "Kennline", "Festpannung", "bei Standard-Festspannungsregler", "eines Siliziumtransistor", "dadurch, indem", ident "a_diskrete_pannungsstabilisierung" (markup, kept); slides/spannungsstabilisierung.md "Linarer Spannungsregler", "linare"; sections/fernspeiseweiche.md "Spannungsverorgung" (caption), "Gleichspannungseite", "Versorgungstrom"; sections/sicherungen.md "zum auflöten".
