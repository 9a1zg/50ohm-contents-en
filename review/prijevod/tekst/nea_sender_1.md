# nea_sender_1 — translation report

Chapter "Sender (1/2)" (Transmitters, part 1): 9 sections, each with its
slides, and 21 solutions. 39 files:

- `contents/sections/` and `contents/slides/`: `aufbau_sender.md`,
  `modulatoren.md`, `nicht_sinus_signale.md`, `leistungsvertaerker.md`,
  `parasitaere_schwingungen.md`, `alc.md`, `ausgangsleistung.md`,
  `senderausgangsleistung.md`, `sender_messungen.md`.
- `contents/solutions/`: `AB403.md`, `AD507.md`–`AD509.md`, `AF305.md`,
  `AF307.md`, `AF310.md`, `AF414.md`, `AF417.md`, `AF420.md`, `AF421.md`,
  `AF423.md`, `AF424.md`, `AI606.md`, `AI607.md`, `AI610.md`, `AI611.md`,
  `AJ201.md`, `AJ202.md`, `AJ205.md`, `AJ206.md`.

`revizija-guard.py --brojevi`: 39 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comments (`%[class:N]`, AB403
`% ggf. noch Verweis auf Fourier-Simulator?`, unchanged), idents
(`a_breitbandverstärker`), formula subscripts ($f_\mathrm{Oberwelle,N}$,
$f_\mathrm{OSZ}$, $\hat{U}_{\mathrm{Sender}}$, $U_\mathrm{SS}$), and the German
words named on purpose (*Oberwellen*, *Oberschwingungen*,
*Hüllkurvenspitzenleistung*, the Annex 1 column headings). Line counts,
leading and trailing whitespace (markdown line breaks in AB403, AF421,
AI610, AI611; the whitespace-only lines of slides/modulatoren.md — an EM
SPACE, U+2003, kept as such —, slides/nicht_sinus_signale.md,
slides/sender_messungen.md and AB403), the line wrapping of the solutions
AD508, AD509, AF305, AF310, and the final-newline state are the same as in
the German in every file.

Embedded questions looked up in English and the prose aligned with them:
NF102, NF401–NF403, VD106, VD727–VD737, EB501, EB502, EF305, EF401, EF402,
EJ209, AB401–AB403, AD503, AD507–AD510, AE206, AF302–AF310, AF401,
AF404–AF424, AF428, AI604–AI615, AJ201, AJ202, AJ205, AJ206, AJ212, AJ213,
AJ217 (e.g. VD106 "generally accepted rules of engineering", NF403 "AF
amplifier", AE206 "double-sideband suppressed-carrier signal", AF308 "AM
signals with suppressed carrier", AF309 "carrier suppression in magnitude
and phase", AF310 "in step with the AF voltage", AD509 "Deviation limiting
and deviation setting in FM transceivers", AF401 "DC input power supplied",
AF417 "low input impedance of the transistors", AF420/AF423/AF424 "turned
towards", AF421 "end stop 1", AJ217 "ferrite bead … emitter", EF305 "before
the power amplifier", EF402 "single-tone or two-tone drive", EB501
"resistive termination … highest crest of the modulation envelope", EB502
"lowest modulating frequency", AI608 "measuring head for RF power
measurement", AI605 "RF probe", AI613 "field-strength meter", AI614/AI615
"harmonics"; the answers quoted in solutions AB403, AD509 and AF414 are the
English answers verbatim).

## Added to `TRANSLATION_GLOSSARY.md` (§14)

33 rows: *Malkreuz*; *Mischer fügt … zusammen*; *Grundwelle /
Ordnungszahl*; *Oberwelle* (course text, against *Harmonische*) /
*Oberwellen* in general / *Oberwellenanteil*; *Sprungstellen / Über- und
Unterschwingen*; *Doppelseitenband-Signal mit unterdrücktem Träger*;
*Diodenring / Ringanordnung*; *ausbalanciert / Trägerabgleich /
Amplitudensymmetrie*; *Gegentaktanregung*; *Filtermethode*;
*Seitenbandfilter*; *Kapitel „Mischer II"*; *breitbandiger
Koppeltransformator*; *Auslegungsfrequenz*; *LDMOS*; *BIAS-Spannung /
Gate-Vorspannung*; *gleichspannungsmäßig / HF-mäßig*; *frei schwebendes Gate
/ unterer Zweig / Einstellwiderstand*; *Betriebsspannungszuführungen*;
*Kurzwellen-Verstärker / -Endstufe*; *TX-Anzeige / Parallel-Widerstand am
Transformator*; *ALC-Anzeige / Sendeleistungs-Anzeige / NF-Aussteuerung*;
*TUNE-Taste / PWR-Regler / Handbuch*; the Annex 1 column headings;
*Hüllkurvenspitzenleistung*; *effektive Wirkleistung … (PEP) / reeller
Abschlusswiderstand*; *HF-Tastkopf / HF-Messkopf*; *Forward-Spannung*;
*Senderabschluss*; *Spannungsverdoppler / Spitze-Spitze-Detektor / doppelte
Spitzenwertgleichrichtung*; *berechnet* in worked slides; *auf den Holzweg
geraten*; *(Emitter) unbeschaltet*.

## Added to `DECISIONS.md`

Two entries (Course text):

- *Oberwelle* against *Harmonische*: where the course text contrasts the
  two (nicht_sinus_signale), *Oberwelle* → *overtone*, with the German words
  named once; where *Oberwellen* just means unwanted multiples, *harmonics*.
- Column headings of Annex 1 to the AFuV: English, with the German heading
  in brackets, as the formula-sheet keywords.

## Judgement calls

- aufbau_sender: *Niederfrequenz-Verstärker / Hochfrequenz-Verstärker*, written out in the German, → "Audio-frequency amplifier" / "Radio-frequency amplifier" (NF → AF, HF → RF); *Bandfilter* → band-pass filter; *Malkreuz* → "multiplication sign", as an earlier unit has it; *Inhalt des Kurses für die Klasse A* → "covered in the Class A course"; *allgemein anerkannten Regeln der Technik* → "generally accepted rules of engineering" (VD106); picture 735 caption identical in all nine places.
- modulatoren: *niederfrequentes Nutzsignal* → "audio-frequency information signal", and *Nutzsignal* in the in-depth box → information signal (glossary §14, the $m(t)$ sense); *im Takt* → "in step with" (AF310); *im Kapitel „Mischer II"* (section and slide) → "in the second chapter on mixers" (chapter titles not yet translated, descriptive as in earlier units); *symmetrische Schaltung* → balanced circuit, *symmetrisch, also ausbalanciert* → "symmetrical, that is, *balanced*", *symmetrischen Zweigen* (in-depth) → symmetrical branches; *Doppelseitenband-Signal mit unterdrücktem Träger (DSB)* → "*double-sideband suppressed-carrier signal* (DSB)" (AE206); *Kapazitätsdiode* → varactor diode, *Varicap* (captions) → varicap; *FM-„Hub"* → FM "deviation", keeping the quotation marks; *Antiparallel geschaltete Dioden* → "Diodes connected in inverse parallel" (glossary §14); *Ein auf die Trägerfrequenz abgestimmter Schwingkreis* → "A tuned circuit resonant at the carrier frequency" (not "tuned circuit tuned"); slides *Potis* → potentiometers, *C-Trimmern* → trimmer capacitors, *Brückenzweig* → bridge diagonal (glossary §5), *liegen … auf Masse* → "at chassis potential", *Elko* → electrolytic capacitor, caption 142 → "Circuit with an output for an AGC voltage" (AD503); AF307 working `\qty{9,0015}` etc. → decimal points.
- nicht_sinus_signale: see DECISIONS.md — *Oberwelle* → overtone, *Harmonische* → harmonic, the table column "Overtone"; the generic *Oberwellenanteile (bzw. Harmonische der Grundwelle)* → "significant overtones (or harmonics of the fundamental)", then "harmonic content" and "amplitudes of the individual harmonics" (AI614); *Frequenzbereich (Frequency-Domain)* → "frequency domain" (bracket rule); *Ordnungszahl* → ordinal number; *$N$-te* → "$N$th"; ordinals keep their digits ("1st overtone", "2nd harmonic"); caption 595 *Grundschwingung und Oberschwingungen* → "the fundamental and harmonics" (AB403 "harmonics"); worked slides *Lösungsweg / gegeben / gesucht* → "Solution / given / required", as in earlier units.
- leistungsvertaerker: *Kurzwellenbereich* → HF range, *Kurzwellen-Verstärker* → HF amplifier (AF420 "LDMOS HF PA"); *Gegentaktverstärker … in Push-Pull-Konfiguration* → "a push-pull amplifier, with two FETs working in push-pull configuration" (the German itself names it twice); *BIAS-Spannung* → bias voltage, lower case (glossary §14); *Trimmpotentiometer* → preset potentiometers (glossary §4 *preset (trimmer)*); *gleichspannungsmäßig betrachten* → "considered as far as DC is concerned" / "for DC", *HF-Mäßig entkoppeln* → "decouple … as far as RF is concerned" (as glossary *wechselspannungsmäßig*); *Pi-Filter / PI-Filter* → pi filter, caption "Pi filter"; *Übersetzungsverhältnis* → transformation ratio (glossary §4); *frei schwebendes Gate* → floating gate; *Abblockkondensatoren nach Masse* → decoupling capacitors to chassis; slide *Betriebsspannungseinstellung* translated as written ("Operating voltage set by potential dividers", see errors); AF421 working `1,77` → `1.77`, `\qty{2,516}{\mega\ohm}^2` → `\qty{2.516}{\mega\ohm}^2` (see errors); caption 780 *mit Kondensator als kapazitiver Spannungsteiler* → "with capacitors as a capacitive potential divider" (a capacitive divider is two capacitors, as the section says).
- parasitaere_schwingungen: *haben normalerweise keinen Bezug zur Betriebsfrequenz* → "normally bear no relation to the operating frequency" (AJ212 "no fixed relationship"); *TX-Anzeige* → TX indicator; *Parallel-Widerstand am Transformator zu dessen Bedämpfung* → "a resistor in parallel with the transformer … to damp it"; photo 351 caption *Ferrit-Perlen an einem IC* → "Ferrite beads on an IC".
- alc: *Automatic-Level-Control (ALC)* / *AGC (Automatic-Gain-Control)* → "automatic level control (ALC)" / "AGC (automatic gain control)", lower case as expansions; *Aussteuerung der Senderendstufe* → "the drive to the … transmitter power amplifier" (EF305 "power amplifier"); *Empfängerzweig / Sendezweig* → receive path / transmit path; *Regelspannung* → control voltage (it acts on an RF stage, not on receiver gain); *ALC-Anzeige* → ALC indicator; *grüner / roter Bereich* → green / red zone; *Handbuch der Software WSJTX* → "user guide of the WSJTX software" (name as the German writes it, link unchanged); *TUNE-Taste / PWR-Regler* → TUNE button / PWR control; *Wasserfall des TRX* → "waterfall display of the TRX".
- ausgangsleistung: first mention "Annex 1 to the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)" in the section and on the slides; Annex 1 column headings in English with the German in brackets (DECISIONS.md); *Zusatzgeräte* → accessory equipment (EB501, EF401); *Anpassgeräte* → matching units; the PEP definition quoted "in der Fachsprache" (*effektive Wirkleistung … während einer Periode … an der höchsten Spitze der Modulationshüllkurve*) → "the average real power … during one cycle of the RF oscillation at the highest crest of the modulation envelope", the wording of EB501 and RR 1.157, since English "effective power" or "RMS power" would not say what the definition means; *Der selten verwendete deutsche Begriff für PEP ist Hüllkurvenspitzenleistung* kept as information about German usage (DECISIONS.md *USB* entry), also in the slide note; *Punkt 11* → "point 11"; spaced hyphens used as dashes → en dashes.
- senderausgangsleistung: *maximale Senderausgangsleistung – auf Englisch Peak Envelope Power (kurz PEP)* → "the maximum transmitter output power, given as the peak envelope power (PEP)" (bracket rule: the gloss only gives the English term); *primär zugewiesen* → "allocated … on a primary basis" (glossary §1.1); *Zweitonaussteuerung* → two-tone drive (EF402); *im Mittel an einen reellen Abschlusswiderstand* → "the average power … into a resistive termination" (EB501); *mittlere Leistung* → mean power (EB502); the two consecutive blank lines in the section kept; slide *Hüllkurvenleistung* → envelope power.
- sender_messungen: *HF-Tastkopf* → RF probe, *HF-Messkopf* → RF measuring head (AI605, AI608); *Forward-Spannung* → forward voltage; *impedanzrichtig abgeschlossen* → "terminated with the correct impedance" (glossary §14); *belastbares Dämpfungsglied* → "an attenuator with a suitable power rating"; *in einer Tabelle wie in [ref:…]* → "in a table like Table [ref:…]"; table headings and caption translated, decimal commas → points throughout the table; *Probier aus, ob du auf die Lösung kommst!* → "See whether you can work out the solution!"; *Feldstärkeanzeiger* → field-strength meter, *Zeigerausschlag* → needle deflection (glossary §2); slides *berechnet* → calculated; *aus dem Messsystem* → "from the measuring system"; *doppelte Spitzenwertgleichrichtung* → double peak rectification; *beide Halbwellen* → both half cycles (glossary §3).
- Solutions: answers quoted as the English answers (AB403 "random frequency fluctuations", "with no other frequencies.", "harmonics"; AD509; AF414 with the bold kept on "**common-emitter**"); *Kapazitätsdiode* → varactor diode; *Z-Diode* → Zener diode; *Schleifer / Anschlag* → wiper / end stop; *Ersatzwiderstand nach Masse* → "equivalent resistance to chassis"; *Dummyload* → dummy load; *Spannungsverdoppler beziehungsweise Spitze-Spitze-Detektor* → "voltage doubler, or peak-to-peak detector"; *Laut Formelsammlung* → "According to the formula sheet"; *obere Halbwelle* → "positive half cycle"; *Holzweg* → "go astray"; *an ihrem Emitter unbeschaltet* → "no external circuitry at their emitters"; AI611's missing full stop at the end of its first paragraph added (the trailing space kept).

## Suspected errors in the German original

- sections/nicht_sinus_signale.md (in-depth box) and slides/nicht_sinus_signale.md (note) — "Sägezahnförmige Signale enthalten überwiegend geradzahlige Harmonische bzw. ungeradzahlige Oberwellen": a sawtooth contains all integer harmonics, odd and even alike (amplitudes falling as 1/n), not mainly even ones. Kept.
- slides/leistungsvertaerker.md (AF421 working) — "$\frac{\qty{2,516}{\mega\ohm}^2}{\qty{7170}{\ohm}}$": $(\qty{370}{\ohm})\cdot(\qty{6,8}{\kilo\ohm}) = 2.516\cdot 10^6\,\Omega^2$, not $\qty{2,516}{\mega\ohm}^2$ ($2.516\cdot 10^{12}\,\Omega^2$); the result, 351 Ω, is right. Kept.
- slides/sender_messungen.md (AI610 working) — "$U_S = U_{E,eff}\cdot\sqrt{2} = \qty{7,071}{\volt}\cdot 1,414 = \qty{10,07}{\volt}$": the slide before gives $U_{E,eff} = \qty{7,125}{\volt}$; $7.071 \cdot 1.414 = 10.0$, $7.125 \cdot 1.414 = 10.07$. Kept.
- slides/leistungsvertaerker.md — under the heading "BIAS-Spannung in Leistungsverstärkern", "Betriebsspannungseinstellung durch Spannungsteiler": the potential dividers set the bias (operating point), not the supply voltage, as the section says. Kept ("Operating voltage set by potential dividers").
- solutions/AF417.md — "an die $\qty{50}{\ohm}$ des nachfolgenden Senders": $T_2$ matches the transistors to the 50 Ω of what follows the amplifier (filter, antenna), not to a following transmitter. Kept ("of the transmitter that follows").
- slides/alc.md — "Wenn ALC-Anzeige anspricht, ist Sender durch zu starkes NF-Signal übersteuert" and "Bei SSB ist ein geringfügiges Übersteuern erwünscht": the section says that when the ALC indicator reacts the control is becoming active, and that with SSB a slight *response of the ALC* is desirable, not overdriving. Kept.
- Typos with no effect on the English: sections/leistungsvertaerker.md "Kondenstatoren", "Der untere Teil der Schaltung, ist", "wird hier nur die über einen Spannungsteiler die BIAS-Spannung", "Der Rest ist der Schaltung ist", "Ein ähnliche Funktion"; sections/parasitaere_schwingungen.md "Leistungsversträrker", "parisitäre"; slides/parasitaere_schwingungen.md caption "Transformatur"; sections/alc.md "grade" (twice, for "gerade"); sections/senderausgangsleistung.md "Wie die PEP exakt misst" (no subject); sections/ausgangsleistung.md "wenn wir uns … die Strahlungsleistung … besprechen"; solutions AB403 "die niedrigsten Frequenz", AD508 "Schwinkreises", AD509 "Maximum, dass sich", AF305 "in der zweite Stufe", AI611 "ingesamt"; the idents `e_senderausgangsleisung` (idents never change).

## Provjera

Checked all 39 files line by line against `f5c26e7~1` (German), with every
embedded question looked up in `contents/questions/fragenkatalog3b.json`.
Nothing dropped or added; numbers, formulas and markup intact;
`revizija-guard.py --rev f5c26e7~1 --brojevi`: 39 files, *struktura
netaknuta*. The two DECISIONS.md entries (*Oberwelle* → overtone where the text
sets it against *Harmonische*, as AB402 already does; Annex 1 column headings
in English with the German in brackets) and the 33 glossary rows are kept. They
are correct and consistent with the questions. All judgement calls are kept. The
suspected German slips are confirmed (sawtooth: all harmonics; MΩ² in AF421;
7.071 for 7.125 V in AI610; *Betriebsspannungseinstellung*; AF417 "following
transmitter"; the ALC slides) and stay translated faithfully.

Changes: omission 1, meaning 1, technical 0, style 6, glossary 0.

- sections/alc.md (digital modes): "is too strong and is overdriving the
  transmitter" → "is too strong and is being overdriven". In the German
  (*übersteuert wird*), the audio signal is what gets overdriven. The
  transmitter was not named. (meaning)
- sections/ausgangsleistung.md: *haben wir bereits gelernt* → "we have already
  learnt" ("already" was dropped). (omission)
- sections/alc.md (tip): "the ALC only just no longer responds" → "the ALC just
  stops responding". (style)
- sections/senderausgangsleistung.md: "the maximum transmitter output power,
  given as the peak envelope power (PEP)" → "– the peak envelope power (PEP) –".
  This keeps the German apposition without adding "given as". (style)
- sections/sender_messungen.md: "connected ahead of it" → "ahead of the
  measuring circuit", because "it" had no antecedent (wording as AI609). The
  two "rectified by a diode, whose output voltage … and which is held …"
  sentences are recast so that "held" clearly refers to the voltage, not the
  diode. (style ×2)
- sections/ and slides/aufbau_sender.md: *ganz besonders* "very particularly" →
  "especially". (style)
- sections/leistungsvertaerker.md: "is also found again in" → "is also found
  in" (*wiederfinden*). (style)
