# nea_grundlegende_schaltungen_2 — translation report

Chapter "Grundlegende Schaltungen (2/3)" (Basic circuits, part 2): 12
sections, each with its slides, and 20 solutions. 44 files:

- `contents/sections/` and `contents/slides/`: `oszillator_spannungsstabilitaet.md`,
  `oszillator_schaltungen.md`, `oszillator_dds.md`, `oszillator_pll.md`,
  `frequenzvervielfacher_1.md`, `frequenzvervielfacher_2.md`, `mischer.md`,
  `transverter_1.md`, `transverter_2.md`, `verstaerker.md`,
  `kollektorschaltung.md`, `emitterschaltung.md`.
- `contents/solutions/`: `AD401.md`–`AD415.md`, `AD703.md`, `AD704.md`,
  `AF314.md`, `AF501.md`, `AF502.md`.

`revizija-guard.py --brojevi`: 44 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%TODO` comment in
sections/oszillator_schaltungen.md (left in German, as markup), idents, and
formula subscripts (`f_\mathrm{Takt}`, `f_\text{Sender}`, `f_\text{Grund}`,
`f_\mathrm{OSZ}`, `f_\mathrm{Quarz,1}`, `f_\mathrm{ZF}` …), which stay German
by the formula rule. Line counts, trailing spaces and final-newline state are
the same as in the German (also the ten empty lines at the end of
sections/oszillator_schaltungen.md).

Embedded questions looked up in English and the prose aligned with them:
AD401–AD415, AD607–AD610, AD612–AD620, AD701–AD705, AF301, AF311–AF314,
AF501, AF502, ED401–ED403, EF201–EF206, EF301–EF303, EF307, EF308, EF403,
EF405, EF501–EF505 (e.g. AD613 "sustained (undamped) oscillations", "fed
back … in phase", AD614/AD617 "capacitive-feedback (three-point / crystal)
oscillator", "common-collector configuration", "on its third overtone",
AD615 "coupled out", AD612 "well filtered and decoupled", AD701 "phase
detector", AD702 "stable state", AD704 "division ratio", AF311 "non-linear
distorting stage", AF313 "well screened", AF314 "sequence of multipliers",
"Fundamental frequency $\cdot 2 \cdot 2 \cdot 3 \cdot 3$", EF203/EF205
"wanted products", EF206 "well screened", EF308 "Approx. 2.5 kHz", EF405
"power feed … RF pick-up", EF505 "frequency error", AD411 "base bias",
AD412 "AC coupling and DC blocking", AD413 "maximising the AC voltage gain").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

36 rows: the *Chirp* gloss, *Verstärkerelement / Selbsterregung*,
*kapazitiv rückgekoppelt / kapazitiver Spannungsteiler*, *Oszillator /
Verstärker in Kollektorschaltung (Emitterschaltung)*, *wechselspannungsmäßig
/ signalmäßig*, *Oberschwingungen / Obertöne (Quarz)* (overtones),
*auskoppeln / Auskopplung*, *Phaseninkrement / Adresszähler / Wertetabelle*,
*D/A-Wandler*, *Phasendetektor*, *eingerastet (locked)*, *Teilverhältnis /
Teilerfaktor / Teilfaktor*, *Vergleichsfrequenz*, *Verzerrerstufe*,
*Verdoppelung / Verdreifachung / Verneunfachung*, *Zwischenstufe /
Zwischenfrequenzen* (slide), *Gegenprobe*, *Lösung* under *Lösungsweg*,
*Hoch- / Heruntermischung*, *Betragsstriche / Fallunterscheidung*,
*balancierter Ringmischer (Balance-Mixer)*, *Mischprodukte höherer
Ordnung*, *Sende-/Empfangsumschaltung*, *quarzstabilisierter Oszillator*,
*Up-Konverter*, *Linearitätsabweichungen / Bandpasscharakteristik*,
*Strom- / Spannungs-Verstärker*, *Arbeitspunkt (engl. bias, Vorspannung) /
BIAS*, *Eingangskennlinie*, *Kollektor-Emitter- / Basis-Emitter-Strecke*,
*Abblockkondensator in der Betriebsspannung*, *ausregeln*,
*Emitterkondensator / überbrücken*, *ohne Arbeitspunktvoreinstellung*,
*gesperrter Transistor*, *Zur Erinnerung:*.

## Added to `DECISIONS.md`

None. The choices of note (the *Chirp* gloss, *engl. bias*, *eingerastet
(locked)*, *Balance-Mixer*) apply the existing bracket rule and the
*Ducting* gloss rule, and are recorded in their glossary rows.

## Judgement calls

- All files: *Kollektorschaltung / Emitterschaltung* → common-collector / common-emitter circuit, *in Kollektorschaltung* → "in common-collector configuration" or "common-collector oscillator / amplifier" (AD401, AD409, AD617); *Emitterfolger* → emitter follower; *Pufferstufe* → buffer stage; *Spannungsteiler* → potential divider; *Basisvorspannung* → base bias; *Gegenkopplung* → negative feedback; *Koppelkondensator* → coupling capacitor; *Abblockkondensator* → decoupling capacitor; *gegen / auf Masse* → to chassis; *Halbwelle* → half cycle; *NF / HF* → AF / RF (glossary §3–§5, §14).
- oszillator_spannungsstabilitaet: *Das englische Wort „Chirp" bedeutet wörtlich übersetzt „Zwitschern"* → "The English word "chirp" means the short, high call of a small bird": the German translates the English word into German; the English explains it instead, as the *Ducting* gloss does, so the next sentence ("has something of a bird's chirp about it") still follows. *Druchgang* (= *Durchgang*) → "over" (glossary §2).
- oszillator_schaltungen: *Oberschwingungen/Obertöne* of a crystal → "harmonic frequencies (overtones)", *auf einer Oberschwingung betrieben* → "operated on an overtone", as AD617 b; *Oberwelle* of a signal stays *harmonic*. *kapazitiver Spannungsteiler* → "capacitive potential divider", as AD616 a.
- oszillator_schaltungen: *da der Kollektor wechselspannungsmäßig auf Masse liegt* → "since the collector is connected to chassis as far as AC is concerned".
- oszillator_dds: *Direkte Digitale Synthese, englisch Direct Digital Synthesis* → "*Direct digital synthesis*" (bracket rule); index terms translated (*Direct digital synthesis*, *DDS:Phase accumulator*); caption *DDS (Direct Digital Synthesizer)* → "DDS (direct digital synthesiser)", British *-ise* as §5 *frequency synthesiser*. "in [ref:a_dds_aufbau] dargestellt" (no *Abbildung*) → "shown in Figure [ref:…]", as in the previous unit. Caption *Vergleichssignal* → "Comparison signal" (the K = 1 signal the K = 2 figure is compared with).
- oszillator_pll: *„eingerastet" (locked)* → ""locked"", the bracket only gives the English word; *Phasenvergleicher* → phase detector (AD701); *Teilverhältnis / Teilerverhältnis / Teilfaktor* → division ratio throughout; *Frequenzintervall* → "frequency step"; *Vergleichsfrequenz* → comparison frequency.
- frequenzvervielfacher_1 slides: *Kreuzung beachten* → "Note where the lines cross" (the crossing in the EF302 block diagram).
- frequenzvervielfacher_2 slides: *Es werden Zwischenfrequenzen erzeugt* → "Frequencies are produced at the intermediate stages": the section speaks of frequencies between the multiplier stages; "intermediate frequencies" would read as the IF. *Gegenprobe* → "Check". `$\textrm{Grundfrequenz}\,\cdot 2…$` → `$\textrm{Fundamental frequency}\,\cdot 2…$` and in AF314 `$\text{Grundfrequenz}…$` → `$\text{Fundamental frequency}…$`: running words in a formula, not a subscript, and the wording of AF314's answers.
- frequenzvervielfacher_2: *Klasse-C-Verstärker* → "class C amplifier" (glossary §5, lower case); *2. Harmonische* → "2nd harmonic" (keeps the digit).
- mischer: *siehe Vertiefung* → "see the in-depth section"; *balancierter Ringmischer (Balance-Mixer)* → "balanced ring mixer", the bracket only repeats the name; *Fallunterscheidung* → "two cases have to be distinguished"; slides *Lösungsweg* / *Lösung:* → "Solution" / "Working:", so the bullet does not repeat the heading.
- transverter_1: *Kurzwellen-Transceiver* → HF transceiver; *Sende-/Empfangsumschaltung* → transmit/receive switching; *quarzstabilisierte Oszillator* → crystal-controlled oscillator (as AF314); *Abweichungen in der Zielfrequenz* → errors in the target frequency (EF505 "frequency error"). Slide *wird ver-3-facht* → "is multiplied by 3", keeping the digit; *daneben* → "off".
- transverter_2: *Teilbereich* → sub-band (glossary §1.3), also in AF501/AF502; *logischerweise* → "Not surprisingly"; *Verneunfachung* → "multiplying … by nine"; *Bandfilter* → band-pass filter (glossary §5).
- verstaerker: *entsprechend belastbare Spannungsquelle* → "a voltage source with a suitable rating"; *(sog. Splatter)* → "(known as splatter)"; *NF-Bandbreite* → audio bandwidth (glossary §13); *Stromzufuhr* → power feed and *HF-Einstrahlung* → RF pick-up (EF405); *Einströmen von Hochfrequenz in das Stromnetz* → "RF from being conducted into the mains". Slide notes *im Abschnitt Unerwünschte Ausstrahlungen im Kapitel Sender* → "in the section on unwanted emissions in the chapter on transmitters" (chapter titles not yet translated; descriptive, as in sicherungen). EF308 note *Erkennbar am Mikrofon vorher* → "Recognisable from the microphone before it" (in the block diagram).
- kollektorschaltung, emitterschaltung: *Arbeitspunkt (engl. bias, Vorspannung)* → "operating point (bias)": the gloss names the English word and its German equivalent; the English keeps "bias" as the established term. Slides *BIAS* → "bias".
- kollektorschaltung: *wird dieses Signal durch die Eingangskennlinie verstärkt* → "this signal is amplified according to the input characteristic"; *Zudem wird der Kollektor durch den Abblockkondensator signalmäßig (für Wechselspannung) auf Ein- und Ausgang gelegt* → "the decoupling capacitor connects the collector, as far as the signal is concerned (for AC), to both the input and the output" (see errors); the missing full stop after "abgelesen werden " kept, with its trailing space.
- emitterschaltung: *ohne Arbeitspunktvoreinstellung durch einen Spannungsteiler* → "without its operating point being preset by a potential divider"; caption → "without a preset operating point"; *So erklärt sich das entsprechende Ausgangssignal* → "This explains the output signal in question".
- Tables (emitterschaltung, AD402, AD403, AD405): `l:` / `X:` column markers kept; *Eigenschaft* → Property, *hoch / niedrig* → high / low; `\num{0,9}` → `\num{0.9}`.
- AD703: the German ends "muss die Frequenz an Punkt A ebenfalls [formula] betragen."; English "the frequency [formula] must also be present at point A." so the sentence closes after the formula on its own line, as in the German.
- AD406, AD407: *gesperrt / sperrt* → "cut off"; *gegenphasig* → "in antiphase" (glossary §3).

## Suspected errors in the German original

- slides/transverter_2.md — third bullet "Liegt die Oszillatorfrequenz darunter, wird ein SSB-Signal invertiert": the sideband is inverted when the oscillator is *above* the wanted signal; the bullet before has just covered the "below" case (no inversion). Translated as written ("below it").
- slides/transverter_2.md — first bullet "Umsetzer von einer Frequenz auf eine andere durch Frequenzvervielfacher": converters and transverters convert by mixing (EF502, transverter_1); a multiplier at most produces the oscillator frequency. Kept.
- slides/kollektorschaltung.md — "Ausgangsignal: Kollektor → Last → Versorgungsspannung → Kollektor": in the common-collector circuit the output is taken at the emitter, so the path should run emitter → load → … → collector → emitter. Kept.
- slides/kollektorschaltung.md — "Kollektor wird auf Masse gelegt → Ausgang ist auf gleichem Potenzial wie Eingang" (and in the section "Kollektor … signalmäßig … auf Ein- und Ausgang gelegt"): what is meant is that the collector, at AC earth through the decoupling capacitor, is the common reference of input and output; input and output are not at the same potential. Kept.
- slides/emitterschaltung.md — "Basis-Emitter-Strecke leitet erst, wenn ca. 0,5 V überschritten werden": the section and AD406 say approx. 0.6 V. Kept.
- slides/emitterschaltung.md — "Halten Gleichspannungsanteile aus der Netzspannung vom Arbeitspunkt fern": there is no mains voltage in the circuit; the section says the coupling capacitors keep DC components away from the amplifier stage. Translated as written ("from the mains voltage").
- slides/oszillator_pll.md — "Kleinste wählbare Frequenz entspricht dem Referenzoszillator": the section says the smallest selectable frequency *step* (*Frequenzintervall*). Kept.
- slides/transverter_1.md — "z.B. wird ein 2 m-Signal im Empfang als ein 70 cm-Signal ausgesendet": a converter works in one direction only; "received … transmitted" describes something else (a cross-band repeater). Kept.
- sections/emitterschaltung.md table (also AD402, AD403, AD405) — the input impedance of the common-emitter circuit is given as "hoch", the same as the common collector's; it is usually described as medium (a few kΩ) and well below that of the common collector. Kept.
- slides/transverter_2.md (AF502 solution) — "44,6667 MHz" where the question, AF502 and the section have 44.667 (rounding only). Kept.
- Typos with no effect on the English: sections/oszillator_spannungsstabilitaet.md "Druchgang"; slides/oszillator_schaltungen.md "Eines der wichtigsten Schaltungen"; sections/frequenzvervielfacher_2.md missing full stop after "wie sie funktionieren", "im laufe"; sections/mischer.md "Multipliziert", "Oszilatorfrequenz"; sections/transverter_1.md caption "z. B. Für"; sections/verstaerker.md "Leicht", "i.d.R", "Sprachkommunkation"; slides/verstaerker.md caption "Amateurfunk Mikrofonverstärker"; sections/kollektorschaltung.md and emitterschaltung.md caption "Bezeichnugnen"; slides/kollektorschaltung.md "Versorgungspannung", "Ausgangsignal", "Versorungsspannung"; sections/emitterschaltung.md "Kollektor und Emitterschaltung", "zuammen", "Kollerktorwiderstand", "Kollektor-Emitter-Strecke, fließt"; slides/emitterschaltung.md "Bipoltransistor" (captions), "Ausgangsignal", "Verstärkungfaktor"; slides/transverter_2.md `f_{Osc,2}` without `\text` (markup, kept).
