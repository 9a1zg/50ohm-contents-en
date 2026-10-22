# nea_grundlegende_schaltungen_3 — translation report

Chapter "Grundlegende Schaltungen (3/3)" (Basic circuits, part 3): 5
sections, each with its slides, and 2 solutions. 12 files:

- `contents/sections/` and `contents/slides/`: `verstaerker_wirkungsgrad.md`,
  `verstaerker_klasse.md`, `verstaerker_linearverstaerker.md`,
  `verstaerker_eigenschwingung.md`, `verstaerker_begrenzung_bandbreite.md`.
- `contents/solutions/`: `AD429.md`, `AD430.md`.

`revizija-guard.py --brojevi`: 12 files checked, *struktura netaknuta*.
German-word grep: no hits. Formula subscripts (`P_\mathrm{HF}`,
`P_\text{ab}`, `P_\text{zu}`, `I_\mathrm{A/B}`, `\eta_\text{A}`) stay German
by the formula rule; the `%` comments (`% A-Betrieb des Verstärkers:` …) stay
as markup. Line counts, trailing spaces and final-newline state are the same
as in the German (also the blank last line of
sections/verstaerker_eigenschwingung.md).

Embedded questions looked up in English and the prose aligned with them:
AF401–AF403, AD416–AD425, AD429–AD433, AJ215, AJ216, AJ218 (e.g. AF401
"the ratio of the RF output power to the DC input power supplied", AD416
"class AB", AD419–AD421 "harmonic content", "quiescent current", "Efficiency
approx. 40 %", AD422/AJ218 "Class A, AB or B operation", AD423 "overdriven
… splatter on adjacent frequencies", AF403 "screening", AD429 "driver
stage", "DC power", AD431 "waveform", AD432 "self-oscillation", AJ215
"decoupled from each other", AJ216 "well screened", AD433 "band-pass
filter", "audio bandwidth of a microphone amplifier").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

10 rows: *A/B-Betrieb / Verstärkerklasse A/B* (class AB), *Verstärkerklassen
/ Klasse D, E, F, J, S*, *Ruhearbeitspunkt / Arbeitsgerade / Sperrung und
Sättigung / Sperrpunkt*, *Stromflusswinkel*, *Steuergröße / Ausgangsgröße*,
*Einsetzen des Kollektorstroms*, *Stromimpulse / konstante Hüllkurve*,
*Gegentaktschaltung, im Englischen push-pull amplifier*, *zugeführte /
aufgenommene Gleichstromleistung / Gleichstrom-Versorgungsleistung /
Gleichspannungsleistung*, *Oszillation/Pfeifen*.

## Added to `DECISIONS.md`

None. *A/B* → *AB* follows the question bank and the glossary's existing
§5 row (*AB-Betrieb* → class AB operation), and is recorded in its
glossary row.

## Judgement calls

- verstaerker_klasse (section and slides): *A/B-Betrieb*, *Verstärkerklasse A/B* → "class AB operation", "amplifier class AB": the German course text writes *A/B*, but its own list of classes ("A, B, AB und C") and the questions (AD416, AD422, AD423) write *AB*, and *class AB* is the English term. `I_\mathrm{A/B}` stays as a symbol.
- verstaerker_klasse: *A-Betrieb* etc. → "class A operation", lower-case *class* in running text (glossary §5), "Class A" at the start of bullets and in the table header; *B-Verstärker* → "class B amplifier"; *Klasse-D- und Klasse-E-Verstärker* → "class D and class E amplifiers".
- verstaerker_klasse: *Stromflusswinkel* → conduction angle; *Ruhearbeitspunkt* → quiescent operating point; *Arbeitsgerade* → load line; *zwischen Sperrung und Sättigung* → "between cut-off and saturation"; *Sperrpunkt* → cut-off point; *Halbwelle* → half cycle (glossary §3); *Oberwellenanteil* → harmonic content (AD419–AD421); *Übersteuerung* → overdriving (AD423).
- verstaerker_klasse: *eine Gegentaktschaltung, im Englischen push-pull amplifier* → "a *push-pull* circuit": the German gives the English name as a gloss, which in English only repeats the term (bracket rule); the italics stay on the term.
- verstaerker_klasse: *In linearer Darstellung … an einem geraden Verlauf, ohne Krümmung, zu erkennen* → "On linear axes, these regions can be recognised by their straight course, without any curvature".
- verstaerker_klasse: *ein abgestimmter Schwingkreis* → "a tuned circuit" (glossary *Schwingkreis* → tuned circuit already says *abgestimmt*); *schaltungstechnische Tricks* → "circuit techniques".
- verstaerker_klasse: *Der Ruhestrom beeinflusst die Effizienz … und damit dessen Wirkungsgrad reduziert* → "has a major influence on how efficient an amplifier is, since it increases the power the amplifier dissipates as heat and so reduces its efficiency": German *Effizienz* and *Wirkungsgrad* are both *efficiency* in English; recast so the sentence does not say "influences the efficiency … reduces its efficiency". *thermische Verlustleistung* → "power dissipated as heat" (also on the slide).
- verstaerker_klasse slides: *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", as in the earlier units; `0,4`, `0,85` → `0.4`, `0.85`. *Wirkungsgrad zwischen 50 % bis 80 %* (AP3) → "between 50 % and 80 %".
- verstaerker_wirkungsgrad: *zugeführte Gleichstromleistung* → "DC input power supplied" (AF401 a), *aufgenommene Gleichstromleistung* → "DC power drawn"; *Gleichstrom-Versorgungsleistung* → "DC supply power"; *im folgenden Kapitel* → "in the next chapter" (see errors).
- verstaerker_linearverstaerker: *Modulationsarten* → "modes" (glossary §7 *Modulationsart* → mode); *Signalformen* → "waveforms", as AD431.
- verstaerker_eigenschwingung tip: *Audio-Verstärker, die mit einem Mikrofon am Eingang für Veranstaltungen etc. betrieben werden* → "audio amplifiers that are operated with a microphone at the input at events and the like"; *Oszillation/Pfeifen* → "oscillation/whistling", keeping the slash.
- verstaerker_begrenzung_bandbreite: *des aufmodulierten NF-Signals* → "of the AF signal modulated onto the carrier"; *maximale Modulationsfrequenz* → "maximum modulating frequency" (glossary §7 *Modulationsfrequenz*); *gesetzliche Bestimmungen bzgl. der maximal zulässigen Bandbreite* → "legal requirements on the maximum permitted bandwidth".
- AD429, AD430: `\num{0,4}`, `\num{0,45}`, `\qty{12,5}` → decimal points; *abgegebene HF-Leistung* → "RF power delivered".

## Suspected errors in the German original

- sections/verstaerker_klasse.md — caption of picture 1085 "Vereinfachte Eingangskennlinie eines Transistors": the text describes the curve as relating base-emitter (gate-source) voltage to collector (drain) current, which is the transfer characteristic (*Steuerkennlinie*, as AD416 calls the same kind of drawing); an input characteristic relates base current to base-emitter voltage. Translated "input characteristic".
- sections/verstaerker_wirkungsgrad.md — "Ruhestrom …, welchen wir im folgenden Kapitel genauer betrachten": the quiescent current is treated in the next section (verstaerker_klasse), in the same chapter. Kept ("in the next chapter").
- sections/verstaerker_linearverstaerker.md and slides — a linear amplifier "für alle Modulationsarten …, die Modulationsinformation in ihrer Amplitude oder Phase übertragen (… QPSK, PSK)": a signal whose information is purely in its phase has a constant envelope and, like FM (verstaerker_klasse: information "nur in der Frequenz"), can be amplified non-linearly; PSK and QPSK as used need a linear amplifier because their filtering gives them an amplitude variation. Kept.
- sections/verstaerker_klasse.md — class AB efficiency "zwischen 50 % und 80 %" (text, summary, table, AP3 slide), the same upper limit as class B; the question bank's description of the class between A and B (AD419–AD421, answer b: "Wirkungsgrad bis zu 70 %, … geringer bis mittlerer Ruhestrom") gives up to 70 %. Kept.
- slides/verstaerker_eigenschwingung.md — "Je höher der Verstärkungsfaktor, umso mehr Eigenschwingungen und Rückkopplungen treten auf": the section says the amplifier *tends* more to self-oscillate (*neigt … zu*); the feedback itself does not grow with the gain. Kept.
- Typos with no effect on the English: sections/verstaerker_wirkungsgrad.md "Der Wirkungsgrad eine HF-Leistungsverstärkers", "also  durch" (double space); slides/verstaerker_klasse.md "nichtliniear", "duch", "Bei Kenntnis des Arbeitspunkt", "zwischen 50 % bis 80 %", note "Röhren- und Transistorverstärker" (for *-verstärkern*); sections/verstaerker_klasse.md "Modulations-Information … nicht in der Amplitude sondern" (missing comma).
