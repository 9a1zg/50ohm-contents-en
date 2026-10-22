# nea_bauelemente_1 — translation report

Chapter "Bauelemente (1/2)" (Components, part 1): 7 sections, each with its
slides, and 32 solutions. 46 files:

- `contents/sections/` and `contents/slides/`: `kondensator_1.md`,
  `phase.md`, `kondensator_2.md`, `spule_1.md`, `spule_2.md`,
  `uebertrager_1.md`, `uebertrager_2.md`.
- `contents/solutions/`: `AA101.md`, `AB302.md`, `AB303.md`,
  `AC101.md`–`AC111.md`, `AC201.md`–`AC211.md`, `AC301.md`–`AC307.md`.

`revizija-guard.py --brojevi`: 46 files checked, *struktura netaknuta*.
German-word grep: no hits outside formulas, idents
(`e_Dielektrizitätszahl`, `e_Trafo mit getrennten Wicklungen`,
`e_HF Übertrager` …), the symbol $ü$, the subscripts $R_\text{Isolator}$,
$A_\mathrm{Dr}$, and the German formula-sheet keywords and memory rhymes
kept on purpose (see DECISIONS.md).

Embedded questions looked up in English and the prose aligned with them:
EA101, EA102, EB204, EB205, EC201–EC207, EC301–EC307, EC401–EC404, ED216,
AA101, AB302, AB303, AC101–AC111, AC201–AC211, AC301–AC307.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

27 rows: *elektrische / magnetische Feldkonstante*, *relative
Dielektrizitätszahl / Permeabilität*, *magnetische Flussdichte*,
*Selbstinduktion / Selbstinduktionsspannung / Induktionsgesetz*, *Lenzsche
Regel*, *Wirbelströme*, *Kupferlackdraht / versilberter Kupferdraht*,
*Festkondensator / gepolter Kondensator / Tantalkondensator*,
*Trimmkondensator / Lufttrimmer / Luftdrehkondensator*, *Drehkondensator*
beside *veränderliche Kondensatoren* (rotary variable capacitor),
*Folien-Wickelkondensator*, *ESR / ESL*, *Antennenanalyzer / VNA*,
*Zweikanal-Oszilloskop*, *Zeigerdiagramm / Zeiger / Einheitskreis*,
*Bogenmaß / Winkelmaß*, *Satz des Pythagoras / geometrische Addition*,
*Scheinwiderstand* beside *Impedanz*, *Übertrager / Transformator / Trafo*
as synonyms, *Leerlauffall*, *Stromdichte / Belastbarkeit von Wicklungen*,
*frei verlegte Leiter*, *Pulvereisen- / Ferritringkern*, *Weißblech*,
*Unun-Übertrager / bifilar (verdrillt)*, *Stichwort (Formelsammlung)*, the
two memory rhymes.

## Added to `DECISIONS.md` (Course text)

- Formula-sheet keywords: English, with the German keyword in brackets,
  because the formula sheet used in the examination is German.
- German memory rhymes (*Kondensatooor … vooor*, *Induktivitääät …
  spääät*) kept, with the English meaning in brackets, as the
  country-prefix mnemonics.

## Judgement calls

- kondensator_1: *Drehkondensatoren* in the list of *veränderliche Kondensatoren* → "rotary variable capacitors", so the line does not read "variable capacitors in the form of variable capacitors"; elsewhere *Drehkondensator* → "variable capacitor" (glossary §4, EC206).
- kondensator_1: *Luft beim Luftdrehkondensator oder Lufttrimmer* → "air-spaced variable capacitor or air trimmer"; *Folienwickelkondensator* → "wound film capacitor"; table *Voll-PE (Polyäthylen)* → "Solid PE (polyethylene)", *Schaum-PE* → "Foam PE" (glossary §9).
- kondensator_1: *(sprich: "Epsilon R")* → "(say: "epsilon R")"; *Naturforscher* (Faraday) → "natural philosopher" (glossary §14).
- kondensator_1, spule_1: *Formelbuchstabe* → "symbol" (glossary §14 *Formelzeichen*); *die Ladung … ist $\unit{\ampere\second}$* → "is the $\unit{\ampere\second}$" (unit named by its symbol).
- phase: *Bogenmaß* → "radians", *Zeigerdiagramm* → "phasor diagram", *rotierender Zeiger* → "rotating pointer" (the drawing's pointers B, C, D); *(vgl. Vertiefung)* → "(see In depth)", the label of the indepth box; the German's double full stop after the reference kept.
- kondensator_2, spule_2: *Der Betrag der Impedanz |Z| entspricht dem sogenannten Scheinwiderstand* → "is what German calls the *Scheinwiderstand* (in English usually also just called the impedance)": English has one word for both, so the German term is named once instead of a sentence equating impedance with itself; elsewhere *Scheinwiderstand* → impedance (slides heading "Impedance").
- kondensator_2, spule_2, solutions AC101: the memory rhymes kept in German with the English meaning in brackets (new DECISIONS.md entry); slides *Merke:* → "Remember:", *-oder-* → "-or-".
- kondensator_2: *Styroflexkondensator* → "polystyrene (Styroflex) capacitor" (glossary §4, EC206); *Güte $Q$ (Quality Factor)* → "the Q factor $Q$ (quality factor)"; *Gegenkathete / Ankathete* → "opposite side / adjacent side"; *Wirkleistung umgesetzt* → "real power … converted".
- spule_1: *gerade Zylinderspule* → "straight *solenoid*, or cylindrical coil", so the prose meets EC305's "cylindrical coil"; *Spule* → "inductor" for the component, "coil" for the winding and in the lamp question (EC302 "iron-cored coil").
- spule_1: *magnetisch leitfähiges Material* → "a material that conducts magnetic flux well" (also spule_2), not "magnetically conductive"; *Elementarmagnete* → "elementary magnets".
- spule_1 slides, spule_2 slides: *Ringspule* / *Ringkernspule* → "toroidal inductor"; *Induktivitätskonstante* → "inductance factor" (glossary §4, AC205).
- spule_2, uebertrager_2, AC204, AC307: formula-sheet keywords in English with the German keyword in brackets (new DECISIONS.md entry), e.g. "keyword: current rating of windings (*Belastbarkeit von Wicklungen*)".
- spule_2 slides, solutions AC208: `\text{Windungen}` → `\text{turns}` (running word in `\text{}`); headings *Gegeben / Gesucht / Lösungsweg* → "Given / Required / Solution", slides "given: / required:" as in earlier units.
- uebertrager_1: *der Übertrager oder Transformator, kurz Trafo* → "the *transformer* (in German *Übertrager* or *Transformator*, *Trafo* for short)", the German names kept as information, since English has one word; *Übersetzungsverhältnis* → "transformation ratio" (the symbol $ü$ stays), *Windungsverhältnis* → "turns ratio" (AC305, AC306).
- uebertrager_2: *Anpassungsübertrager* → "matching transformer" (glossary §11); *nach VDE* → "according to the VDE"; *HF-Übertrager (BALUN)* → "RF transformer (balun)" (glossary §13); *Stromdichte $S$* kept with its symbol.
- AC207: *Man wird 90 Windungen aufbringen* → "In practice, 90 turns would be wound" (see errors).
- AC307: the garbled *kann nur mit der nach der Formel zu "Belastbarkeit von Wicklungen" berechnet werden* → "can only be solved with the formula for the "current rating of windings"", its evident meaning.

## Suspected errors in the German original

- sections/kondensator_1.md and slides/kondensator_1.md — $\varepsilon_0 = \qty{0,855e-11}{\ampere\second\per\volt\meter}$: the electric constant is 8.854 × 10⁻¹² As/Vm, i.e. 0.885e-11 (two digits swapped). Translated as written.
- sections/uebertrager_1.md — "Auf Grund der Selbstinduktion in Spulen lässt sich Energie … zwischen zwei Spulen … übertragen": transfer between two coils is mutual induction (*Gegeninduktion*), as uebertrager_2 and AC301 say. Translated faithfully ("Because of self-induction").
- slides/kondensator_2.md (note on AC111) — "Im eingeschwungenen Zustand fließt nahezu kein Strom mehr, weshalb die Leistung ebenso nahezu 0W ist": with AC a capacitor current keeps flowing (1 µF at 10 kHz is 15.9 Ω, so about 0.75 A at 12 V); the real power is about 0 W because of the 90° phase shift, as the section and solution AC111 say.
- sections/uebertrager_2.md — "an einen Sender mit einer Lastimpedanz von 50 Ω": the 50 Ω is the transmitter's output (source) impedance, or the load impedance it expects; translated as written ("load impedance").
- slides/spule_1.md — "Die Induktivität einer Ringspule …" over the solenoid formula with $l$ as length; the right column covers both ("Länge der Spule bzw. mittlere Feldlinienlänge"), but the heading names only the toroid.
- solutions/AC207.md — "Man wird 90 Windungen aufbringen": the exam's correct answer is 89 (≈ 89.4), and the slides give 89 turns.
- solutions/AC204.md — the result 1884 Ω (from 2π ≈ 6.28) differs from the exam's 1885 Ω (1884.96 Ω unrounded).
- solutions/AC306.md — "$\frac{Z_P}{Z_S} = \frac{2500}{50} = 50$" puts the 2500 Ω on the primary side, while the text before it, uebertrager_2 and the result 1:7 take the 50 Ω side as primary; the turns are then written $N_2/N_1$ instead of $N_S/N_P$. Translated as written.
- Typos with no effect on the English: sections/kondensator_1.md "Kondesators" (captions 1015, 185), "anggeben", "aufgerauhte", "ist eine spezielle Eigenschaft … ist die sogenannte" (verb twice), "vom Verwendeten"; sections/phase.md "Eine ganz Umdrehung", ".." after the reference; sections/spule_1.md "Ihre Schaltsymbole", "In der folgenden Frage,  steigt"; sections/spule_2.md "Im gegensatz", "Wechelstromwiderstand", "nach dem den Satz"; sections/uebertrager_1.md "Bei der Folgenden"; sections/uebertrager_2.md "dass das Impedanzverhältnis ist das Quadrat"; slides/spule_2.md "leitfähigereres", "gut leitfähigem"; slides/uebertrager_1.md "Übersetzungverhältnis", "verhalten sich wie zur Anzahl"; slides/uebertrager_2.md "Gegendinduktion", "nach ziehen"; solutions/AC111.md "in form"; AC306.md "Aus sicht".

## Provjera

All 46 files compared paragraph by paragraph with the German (`66c8363~1`),
embedded questions checked against their English in the bank. Nothing
dropped or added; the translation is faithful and technically sound. The
two DECISIONS.md entries and 25 of the 27 new glossary rows kept as they
are; the judgement calls kept except where listed below.
`revizija-guard.py --rev 66c8363~1 --brojevi`: 46 files, *struktura netaknuta*.

Changes: omission 0, meaning 2 (additions removed), technical 2, style 6, glossary 2.

- Glossary §4: *Übersetzungsverhältnis* (ü) → **transformation ratio**, split from *Windungsverhältnis* → turns ratio. The old row gave both as "turns ratio", but the translator (rightly) used "transformation ratio" for ü to match EC401, AD303 and AD304 (*Transformationsverhältnis*, the same ratio), and the row was not updated. Text unchanged; row now matches it (also needed by gleichrichter_2 later).
- Glossary §14 and phase, AB302: *rotierender Zeiger* → "rotating **phasor**" (not "pointer"), also the drawing's coloured lines ("the green phasor B"); phasor is the established English term, and the text already says "phasor diagram".
- kondensator_2 (section, slides), AC103: *Wirkleistung umsetzen* → real power "dissipated", not "converted" (technical: what a resistance does with real power).
- AC207: "In practice, 90 turns would be wound" → "90 turns would be wound": "In practice" was not in the German (*Man wird 90 Windungen aufbringen*).
- spule_1 slides: *Selbstinduktionsspannung, die entgegengerichtet ist* → "that acts in the opposite direction", not "that opposes the current" (an addition).
- Style: "An empty capacitor" → "An uncharged capacitor" (kondensator_1 slides); "the skin effect acts" → "there is the skin effect" (spule_2 section and slides); "Why is there a 230 V AC mains?" → "Why do we have a 230 V AC mains supply?" and "Given are" → "We are given" ×2 (uebertrager_1); the garbled "is the same as …, but the same as …" ratio sentence recast (uebertrager_2 slides); "0W" → "0 W" (kondensator_2 slides).
