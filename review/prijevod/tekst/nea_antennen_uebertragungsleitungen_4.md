# nea_antennen_uebertragungsleitungen_4 — translation report

Chapter "Antennen und Übertragungsleitungen (4/4)" (Antennas and
transmission lines, part 4): 8 sections, each with its slides, no
solutions. 16 files:

- `contents/sections/` and `contents/slides/`: `vna_1.md`, `vna_2.md`,
  `leitung_phasenverschiebung.md`, `lecherleitung.md`,
  `impedanztransformation.md`, `mantelwellen_1.md`, `mantelwellen_2.md`,
  `umwegleitung.md`.

`revizija-guard.py --brojevi`: 16 files checked, *struktura netaknuta*.
German-word grep: no hits; the only German left is the `%` comment in
mantelwellen_2 (`% TODO: Bild Spannungsbalun / Spartransformator`), which
stays, the idents, the symbol $ü$, and the German word named once in
mantelwellen_1 (DECISIONS.md). Line counts, trailing spaces (slides vna_2,
leitung_phasenverschiebung, impedanztransformation, mantelwellen_1; the
blank lines with spaces around the list in sections/mantelwellen_1) and the
presence or absence of a final newline are as in the German.

Embedded questions looked up in English and the prose aligned with them:
EI201–EI206, AI201–AI208, AG320, AG406–AG418, AG420–AG429, EG404–EG408,
AJ115 (EI206 "short-circuit, open-circuit and matched conditions", "test
port", "terminating resistor"; AI201 "device under test", "resistive and
reactive part"; AI204–AI206 "resistive part", "reactive part … inductive /
capacitive"; AI207/AI208 "resonance curve"; AG320 "two parallel
conductors", "mainly depend on … the length of the line"; AG409–AG412
"electrical length", "Nearly 0 Ω", "Very high"; AG413–AG415 "tuned
$\lambda$/2 feeder", "start of the feeder"; AG417/AG418 "transformer
section"; AG406 "pi filter"; EG404/AG428 "sheath current"; EG405 "cause
interference to other equipment and to your own reception"; EG406 "radiation
pattern … distorted"; EG408 "common-mode currents can be attenuated"; AG420
"balancing devices such as a half-wave delay line or a balun"; AG423/AG424
"delay line", "at each of its terminals"; AG425/AG426 "sheath currents",
"common-mode components", "current-compensated choke", "differential-mode";
AG427/AG429 "poor earthing of unbalanced antennas", "coupling into the coax
screen", "uneven loading … from its surroundings"; AJ115 "RF isolating
transformer").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

19 rows: *Mantelwellen (Definition im Kurstext) / Mantelstrom /
Mantelwelle*; *stromkompensierte Drossel neben Mantelwellensperre*;
*Symmetrierglied (Kurstext)*; *Gegentaktsignal / Gleichtaktsignal*;
*Spannungsbalun / Spartransformator*; *(HF-)Trenntrafo / Pol*;
*Dreileitersystem / Außenseite des Innenleiters / …*; *kontaktlose
Einkopplung*; *Umwegleitung / Umwegeleitung / λ/2-Umwegleitung*;
*Anschlusspunkte (Antenne)*; *betragsgleich, 180° phasenverschoben*;
*Frequenz-Sweep / Wobbeln*; *Startfrequenz / Stoppfrequenz /
Frequenzpunkt*; *imaginäre Einheit / imaginäre Zahl / reelle Zahl /
komplexe Zahl*; *Zustände "offen" / "Kurzschluss" / "angepasst" (VNA)*;
*Leitungsabschluss*; *Zweidrahtleitung (Lecherleitung)*; *gewünschter
Speisewiderstand $Z_\mathrm{E}$ / geometrisches Mittel*; *Kreiszahl*.

## Added to `DECISIONS.md`

1 entry (Course text): *Mantelwellen* → common-mode currents, *Mantelstrom*
→ sheath current, with the German word named once where mantelwellen_1
defines the effect ("*common-mode currents* (in German *Mantelwellen*,
literally "sheath waves")"), because the text and the embedded questions
(EG404, AG425, AG426, AG428) also say *sheath current(s)*;
*stromkompensierte Drossel* beside *Mantelwellensperre* → "current-compensated
choke" / "common-mode choke" (AG426); *Umwegleitung* → delay line
throughout (AG420, AG423, AG424).

## Judgement calls

- vna_1: *frequenzabhängige Widerstände* → "frequency-dependent resistances", kept close to the German, which goes on to say "Widerstand (bzw. Impedanz)" → "resistance (or impedance)"; slide *Große und kleine Widerstände eines Schwingkreis* → "High and low resistances of a tuned circuit".
- vna_1: *Zustände "offen" …, "Kurzschluss" …, "angepasst"* → 'the "open" condition, the "short circuit" and the "matched" condition' (EI206); *Lastwiderstand entsprechend des Ausgangswiderstands* → "load resistance equal to the output resistance of the instrument"; *Leitungsabschluss* → "line termination", *Abschlusswiderstand* → "terminating resistor", *Messanschluss* → "test port" (glossary §11, EI206).
- vna_1: caption of photo 201 reordered to "Measurement from 0 MHz to 100 MHz of a low-pass filter with its cut-off frequency at 30 MHz", so that the range does not attach to the cut-off frequency; slide note *der Durchgang bis ca. 30 MHz* → "the passband up to approx. 30 MHz" (not the glossary's operating *Durchgang* → over).
- vna_1/vna_2: *Endgespeisten Drahtantenne* (caption) → "end-fed wire antenna"; *Kalibrierkit* → "calibration kit"; the standards "Load, Open, Closed" kept as written (see below).
- vna_2: *Frequenz-Sweep, oder früher gelegentlich auch als Wobbeln* → "*frequency sweep*, or formerly, now and then, *wobbulation*" — the English counterpart of the older German word (wobbulator), not dropped; *Messobjekt* → "device under test" (AI201); *um den Einfluss von Störungen zu verringern* → "to reduce the effect of interference".
- vna_2: *Wirk- und Blindanteil (Wirkwiderstand R und Blindwiderstand X)* → "resistive and reactive parts (resistance $R$ and reactance $X$)" (glossary §5, AI204–AI206); indepth *einen Wirk- und Blindanteil eines Widerstands* → "the resistive and reactive parts of an impedance", since a resistance in the English sense has no reactive part; *Formelzeichen $i$ (für Ströme)* → "the symbol $i$ (for currents)"; slide note *bewährtes Hilfsmittel* → "well-proven tool" (the section's *beliebtes* → "popular").
- leitung_phasenverschiebung: *im Leiter müssen wir den Verkürzungsfaktor berücksichtigen* → "in a conductor we have to take the velocity factor into account" (a line, so *velocity factor*, DECISIONS.md); table header cells "X: Line length", "X: Phase shift" with the `X:` markers unchanged; *mechanisch länger* → "mechanically longer" (glossary §14 *mechanische Länge*; see below).
- lecherleitung: *hin- und rücklaufender Welle* → "the forward and reflected waves" (glossary §9); *Reihen- / Parallelschwingkreis in Resonanz* → "series / parallel tuned circuit at resonance"; *Leerlauf* → "open circuit"; slide *am Ende offene Zweidrahtleitung* → "two-wire line open at the end", not §9's *twin feeder*, since a Lecher line is not a feeder (AG320 "two parallel conductors").
- impedanztransformation: *Transformationsleitungen* → "transformer sections" (glossary §9, AG417, AG418); *mit 1:49 Unun* → "and its 1:49 unun"; *Speisewiderstand $Z_\mathrm{E}$ am anderen Ende des Kabels* → "the desired input impedance $Z_\mathrm{E}$ at the other end of the cable", and on the slide *Speise- und Lastwiderstand* → "the input impedance and the load resistance": $Z_\mathrm{E}$ is the input end of the line, the antenna is $Z_\mathrm{A}$ (AG417), so the glossary's *feed-point impedance* would point at the wrong end; *Pi-Filter* → "pi filter" (AG406, leistungsvertaerker); *Kreiszahl $\pi$* → "the number $\pi$", slide *der Kreiszahl* (no symbol) → "the mathematical constant"; *das sogenannte Pi-Filter* → "what is called the pi filter", without italics, as the German.
- impedanztransformation slides: *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", as earlier units; *Wellenwiderstand ungleich Lastwiderstand führt neben Stehwellen zu Impedanztransformation* → "A characteristic impedance that differs from the load resistance leads to impedance transformation as well as to standing waves".
- mantelwellen_1: *Diesen Effekt bezeichnen wir als Mantelwellen* → "We call this effect *common-mode currents* (in German *Mantelwellen*, literally "sheath waves")" (DECISIONS.md); the long German sentence that follows split in two; *Mantelströme* → "sheath currents" (EG404); *Richtcharakteristik* → "radiation pattern" (EG406); *Hauselektrik* → "house wiring"; *Dipolschenkel* → "dipole leg" (glossary §14); *Dreileitersystem* → "three-conductor system".
- mantelwellen_1: *ein sogenanntes Symmetrierglied, einen Balun* → "a *balancing device*, a balun" (AG420), since §9's *Symmetrierglied* → balun would make "a balun, a balun"; indepth *aus den englischen Worten "balanced" und "unbalanced"* → 'made up of the words "balanced" and "unbalanced"' ("English" only tells an English reader what the reader already knows; the explanation itself stays); slide *(balanced-unbalanced)* kept.
- mantelwellen_1/_2: *stromkompensierte Drossel … auch als Mantelwellensperre bezeichnet* → "*current-compensated choke*, and it is also known as a *common-mode choke*" (DECISIONS.md, AG426); caption *Mantelwellensperre* → "Common-mode choke"; *Gegentaktsignale / Gleichtaktsignal / Gleichtaktanteil* → "differential-mode signals / common-mode signal / common-mode component" (glossary §9, AG426); *Spule* → "inductor", *Drosselspule* → "choke" (glossary §4).
- mantelwellen_2: *Mantelstrom mit zugehöriger Mantelwelle* → "a sheath current, with its associated sheath wave", slide *Mantelstrom erzeugt eine Mantelwelle um das Kabel* → "The sheath current produces a sheath wave around the cable" (DECISIONS.md); *Pol* (of the isolating transformer) → "terminal"; *Spartransformator* → "autotransformer"; *Speisewiderstand von möglichst 200 Ω* → "feed-point impedance of 200 Ω if possible"; *hinter der Mantelwellensperre* → "beyond the common-mode choke"; *asymmetrisch belastet* → "loaded unevenly" (AG429).
- mantelwellen_2 slides: *HF-Trenntrafo zur Mantelwellensperre* → "RF isolating transformer to block common-mode currents"; note *Zwischen den Spulenwindungen bildet sich Kapazität, die den Gleichtaktanteil nicht vollständig unterdrückt* → "Capacitance forms between the turns of the windings, so that the common-mode component is not suppressed completely" — the German relative clause makes the capacitance the subject of "does not suppress", which is not what is meant (the section's indepth says it); *Einschränkungen der Mantelwellensperre* → "Limitations of the common-mode choke".
- umwegleitung: *Umwegleitung / Umwegeleitung* → "delay line", *λ/2-Umwegleitung* → "$\lambda / 2$ delay line", also the captions (DECISIONS.md); *Anschlusspunkte* → "terminals" (AG424); *180° phasenverschoben* → "180° out of phase"; *Erdpotential* → "earth potential" (glossary §14); *leitend mit einem geerdeten Metallträger verbunden* → "connected conductively to an earthed metal support"; slide *Impedanz beachten* → "Mind the impedance".

## Suspected errors in the German original

- sections/leitung_phasenverschiebung.md — "da von der *elektrischen Länge* eines Koaxialkabels die Rede ist, weshalb das Kabel mechanisch länger sein kann": with a velocity factor below 1 the physical length is *shorter* than the electrical length (verkuerzungsfaktor_1: the cable must be cut shorter). Translated as written ("mechanically longer").
- sections/vna_1.md — caption of photo 327 "SOL(T)-Kalibrierkit. Von links nach rechts - Load, Open, Closed": the third standard of an SOL(T) kit is *Short* (the S of SOLT), not "Closed". Kept.
- sections/mantelwellen_1.md (indepth) — "dann sind die Ströme im Innenleiter nicht symmetrisch": the balance in question is between the currents in the inner *and* outer conductor (the paragraphs before and after say so). Translated as written.
- slides/lecherleitung.md — "Lecherleitung: am Ende offene Zweidrahtleitung": the section says a Lecher line can be open *or* short-circuited at the end, and the slide's last bullet itself treats the short-circuited line. Translated as written.
- Typos with no effect on the English: sections/vna_1.md "zu einander Verhalten" (*zueinander verhalten*); captions in vna_1 and vna_2 "Endgespeisten" (*endgespeisten*); slides/vna_1.md "eines Schwingkreis" twice (*Schwingkreises*); sections/impedanztransformation.md "aus dem Vorherigen Abschnitt" (*vorherigen*); sections/mantelwellen_1.md "Hierzu eigenen sich" (*eignen*); sections/mantelwellen_2.md "Koaxialkabel zur Unterdrückung … geeignet sind" (*ist*), "auf den selben Magnetkern" (*denselben*); slides/mantelwellen_2.md caption "Spannungbaluns" (*Spannungsbaluns*, twice); sections/umwegleitung.md "Umwegeleitung" beside "Umwegleitung", "einen vier mal höhere Impedanz" (*eine viermal höhere*), "Ursache hierfür, ist" (stray comma).

## Provjera

All 16 files compared paragraph by paragraph with the German of
79d8e3d~1; embedded questions (EI201–EI206, AI201–AI208, AG320,
AG406–AG418, AG420–AG429, EG404–EG408, AJ115) read in English. Nothing
dropped or added. The 19 glossary rows and the DECISIONS.md entry are kept
(the German word named once follows the existing *Oberwellen* precedent;
*Umwegleitung* → delay line and *current-compensated choke* follow AG420,
AG423, AG424, AG426); one glossary row reworded. All judgement calls kept,
including *Z_E* → "desired input impedance" (AG417: the dipole is $Z_A$).
`revizija-guard.py --rev 79d8e3d~1 --brojevi`: 16 files, *struktura netaknuta*.

Changes: omission 0, meaning 0, technical 0, style 6, glossary 2.

- glossary — sections/mantelwellen_2: *gleich groß / gleiche Größe* "equal in size", "of the same size", "with the same size" → "magnitude" (§ *Größe* → not "size"); slides/mantelwellen_2 likewise.
- glossary — sections/vna_1, slides/vna_1: the VNA conditions as EI206 has them: 'the "open-circuit", "short-circuit" and "matched" conditions', slides "*Open-circuit* / *Short-circuit* condition"; glossary row *Zustände "offen" …* updated to match.
- style — sections/vna_1: "It can also be found at which frequency an antenna is resonant" → "It is also possible to find the frequency at which …".
- style — sections/vna_2: "or formerly, now and then, *wobbulation*" → "or, occasionally in the past, *wobbulation*".
- style — sections/lecherleitung: "Which frequency forms as a resonance on a Lecher line depends mainly on its length" → "The frequency at which a Lecher line resonates depends mainly on its length" (AG320).
- style — sections/impedanztransformation: "Frequently found is what is called the pi filter" → "A circuit often found is what is called the pi filter".
- style — sections/mantelwellen_1 and _2: *genau dann* "Precisely then, …" → "It is precisely then that …".
- style — slides/mantelwellen_1 note: "which comes in Class A" → "which is covered in Class A".
