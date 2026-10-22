# nea_empfaenger_1 — translation report

Chapter "Empfänger (1/2)" (Receivers, part 1): 18 sections, each with its
slides, and 21 solutions. 57 files:

- `contents/sections/` and `contents/slides/`: `aufbau_empfaenger.md`,
  `detektorempfänger.md`, `ueberlagerungsempfaenger_einfachsuper_1.md`,
  `ueberlagerungsempfaenger_einfachsuper_2.md`, `mischer_2.md`,
  `spiegelfrequenzen.md`, `doppelueberlagerungsempfaenger_doppelsuper.md`,
  `trennschaerfe_1.md`, `trennschaerfe_2.md`, `bfo_1.md`, `bfo_2.md`,
  `intermodulation_kreuzmodulation.md`, `begrenzerverstaerker.md`,
  `vorverstaerker_daempfungsglied.md`, `low_noise_block.md`, `s_meter.md`,
  `daempfungsglieder.md`, `agc_1.md`.
- `contents/solutions/`: `AA113.md`, `AA114.md`, `AD801.md`–`AD806.md`,
  `AF101.md`–`AF108.md`, `AF201.md`–`AF203.md`, `AF206.md`, `AF208.md`.

`revizija-guard.py --brojevi`: 55 files checked, *struktura netaknuta*. The
guard does not see the two files `sections/detektorempfänger.md` and
`slides/detektorempfänger.md`: git quotes the non-ASCII path, `git show`
fails, and the guard skips them as new files. Both were checked with the
guard's own `signature()` and `numbers()` (imported from the tool): structure
and numbers unchanged. A checker running `--rev` will meet the same gap.
German-word grep: no hits; the only German left is formula subscripts
(`f_\text{ZF}`, `f_\text{OSZ}`, `f_\text{NF}`, `P_\mathrm{Aus}`), idents
(`begrenzverstärker`, `e_geradeausempfänger`) and the word
*Geradeausempfänger* named on purpose in aufbau_empfaenger. Line counts,
trailing spaces (markdown line breaks in AA113, AA114, AF206; the
whitespace-only line in ueberlagerungsempfaenger_einfachsuper_1) and the
final-newline state are the same as in the German, also the two trailing
blank lines of sections/daempfungsglieder.md and the stray `‚` after three
slide-separator attributes in slides/doppelueberlagerungsempfaenger_doppelsuper.md.

Embedded questions looked up in English and the prose aligned with them:
NF201, NF303, EF101, EF102, EF208–EF212, EF217, EF218, AA113, AA114,
AD801–AD806, AF101–AF120, AF201–AF214, AF216–AF223, AF226, AF230, AF231
(e.g. EF101 "crystal set", EF102 "tuned radio frequency (TRF) receiver",
"Better selectivity", EF208 "direct-conversion receiver", EF209 "auxiliary
carrier", AF216 "carrier insertion oscillator", "crystal-controlled
oscillator", AF111/AF115 "close-in selectivity", AF204 "preselection",
AF109 "very high first IF", AF113/AF221 "strong-signal performance", AF114
"roofing filter", AF116 "the largest bandwidth required by the intended
modes", AF117 "CO", AF212 "transfer characteristic", AF213/AF214 "balanced
mixer", "balanced ring mixer", AF208 "steepest skirts", AF220 "switching in
an attenuator ahead of the receiver input", AF221 "intercept point", AF226
"limiting amplifier", AF231 "bias tee", AF107/AF203 "image-frequency
interference", AD805/AD806 "symmetrical … attenuator", AA114 "receiver input
voltage", AF101 "S meter reading", "S unit").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

31 rows: *Geradeausempfänger* explaining its own name; *Selektivität
(Trennschärfe) / Nahselektion oder auch Trennschärfe*; *hochohmiger
Kopfhörer / träge / Stromstöße*; *Rundfunksender im Lokalbereich /
Fernempfang*; *Eingangsfilterblock*; *Wortneubildung*; *Lokal-Oszillator /
Schaubild*; *Ringschaltung / Ringmodulator / Dioden-Gleichrichter*;
*konzeptbedingt / prinzipbedingt*; *Spiegelfrequenzstörungen*;
*Vorselektion (Empfänger)*; *CO (Quarzoszillator) / Funktionsblöcke*;
*Regelspannung … (AGC)*; *Störunterdrückungsverfahren*;
*Lösungsmöglichkeiten / 1. Lösung, 2. Lösung*; *Überlagerungsmischung*;
*Hörfrequenz / Tonfrequenz*; *nichtlinearer Grenzbereich*; *Grundsignale /
Steigung / Schnittpunkt*; *Intercept Point dritter / 3. Ordnung*;
*Abschwächer (auch Attenuator genannt) / Dämpfungsglied (Attenuator)*;
*Leistungsdämpfungsglied / ohmsches / T- und π-Dämpfungsglied /
PI-Konfiguration*; *Systemimpedanz / impedanzrichtiger Abschluss*;
*Störimpulse*; *Antennenzuleitung / PTT-gesteuert*; *Low Noise Block
Converter*; *Polarisationsrichtungen*; *S-Wert*; *Grundrauschen oder
Eigenrauschen*; *Ansprechverhalten / Ansprechzeit / Abfallzeit /
Empfängerausstattung*; *Keramikresonatoren*.

## Added to `DECISIONS.md`

None. The choices of this unit follow existing entries: the bracket rule
(German synonyms and English glosses in brackets dropped), the *Schwingkreis*
pattern for a German word that explains its own name (glossary §14), *Figure*
for numbered references, *Solution / given / required* in worked slides.

## Judgement calls

- aufbau_empfaenger (section indepth): *Der hier dargestellte Empfänger wird als Geradeausempfänger bezeichnet. Der Name kommt daher, dass …* — the English name (TRF receiver, EF102) does not carry the German argument, so the German word is named once with a literal gloss, "(in German *Geradeausempfänger*, literally "straight-through receiver"). The German name comes from …", as the glossary does for *Schwingkreis*. The slide keeps the plain English name and the reason after the colon.
- aufbau_empfaenger: *Hochfrequenz-Verstärker (HF-Verstärker)* → "radio-frequency amplifier (RF amplifier)", *Niederfrequenz-Signal, kurz NF-Signal* → "audio-frequency signal, or AF signal for short"; *im Kapitel "Bauteile und Schaltkreise"* → "in the chapter on components and circuits" (chapter titles not yet translated; descriptive, as in earlier units).
- detektorempfänger: *Detektorempfänger* → crystal set (EF101); the bare "durch ein empfangenes Rundfunksignal [ref:am_detektor_antenne]" → "(Figure [ref:…])"; *AM-Modulation gleichgerichtet* → "rectifies the AM modulation"; *träge* headphones → "sluggish".
- ueberlagerungsempfaenger_einfachsuper_1: *Selektivität (Trennschärfe)*, *Selektivität, also Trennschärfe* → "selectivity" (one English word; glossary row). On the slide, the two bullets *Bessere Selektivität des Empfangssignals* and *Höhere Trennschärfe* → "Better *selectivity* for the received signal" and "Sharper *selectivity*", both kept, so that the slide does not read the same line twice. *Überlagerungsempfänger … in der Fachsprache auch Superheterodyn oder Superhet genannt* → "the *superheterodyne receiver* … also called a *superheterodyne* or *superhet* for short"; *variabler Oszillator (VFO, engl. Variable Frequency Oscillator)* → "variable-frequency oscillator (VFO)" (bracket rule); *ZF* → IF; *Kurzwelle* → HF; *Funk- und Radiotechnik* → "radio and wireless technology"; German „…" quotes → English "…".
- ueberlagerungsempfaenger_einfachsuper_2: *Nahselektion oder auch Trennschärfe* → "*close-in selectivity*, or simply *selectivity*" (AF115); slide heading accordingly.
- mischer_2: *Steuerkennlinie(n)* → transfer characteristic(s) (AF212); *durchgesteuert* → "turned fully on"; *Polwender* → polarity reverser; *symmetrischer / unsymmetrischer Aufbau* of a mixer → "balanced / unbalanced design" (DECISIONS.md: *symmetrisch* on a circuit block is *balanced*); the bare "[ref:mischer_ringmischer]" → "(see Figure [ref:…])"; slide *Verzerrung von einem Eingangssignal zu unterschiedlichen Änderungen am Ausgangssignal* → "distorts an input signal, producing unequal changes in the output signal".
- spiegelfrequenzen: *Konzeptbedingt* → "By the very nature of the concept"; *prinzipbedingt* (slide) → "By its very principle"; *Betrag* → magnitude; slide formula `\text{wenn }` → `\text{if }` (running word), subscripts unchanged; *Spiegelfrequenzunterdrückung* → image rejection; *Vorselektion* → preselection (AF204).
- doppelueberlagerungsempfaenger_doppelsuper: *Roofing Filter* → "roofing filter", lower case as a term (AF114, AF116); *Regelspannung für die Steuerung der Eingangsempfindlichkeit des Empfangszweigs (AGC)* → "a control voltage for controlling the input sensitivity of the receive path (AGC)", not the glossary's "AGC voltage", which would say AGC twice in one phrase; *Modulationsart/Betriebsart* → "type of modulation/mode"; slides *1. Lösung / 2. Lösung* → "Solution 1: / Solution 2:" (two correct oscillator frequencies, not two methods); *gegeben / gesucht* → given / required, *Lösungsweg* → Solution, as in earlier units.
- trennschaerfe_2: *steilflankig(st)* → "with (the) steep(est) skirts" (AF208); *im HF-Bereich von Empfängern* → "in the RF section of receivers" (German HF = RF).
- bfo_1, bfo_2: *Hilfsträger* → auxiliary carrier (EF209), *Hilfsträgeroszillator* → carrier insertion oscillator (AF216), so "That is why it is also called a carrier insertion oscillator" still follows; *Überlagerungsmischung* → heterodyne mixing; *(engl. Beat Frequency Oscillator)* kept as the expansion "(beat frequency oscillator)".
- intermodulation_kreuzmodulation: *Saugkreis* → acceptor circuit (glossary §5), also the slide heading and caption; *Intercept Point dritter Ordnung (IP3)* → "third-order intercept point (IP3)", *Intercept Point 3. Ordnung* → "3rd-order intercept point" (the digit kept for the number check); slide *Interception Point* → intercept point (glossary §6); `\text{Ordnung}` → `\text{order}`; *Dämpfungsglied (Attenuator)* → attenuator (bracket rule); *um den Faktor 3 (3. Ordnung) in dB* → "by a factor of 3 (3rd order) in dB"; *Wasserfalldiagramm* → waterfall display.
- vorverstaerker_daempfungsglied: *Abschwächer (auch *Attenuator* genannt)* → "so-called *attenuators*" (bracket rule; *Abschwächer* is *attenuator*, glossary §14); *Kurzwellenempfänger* → HF receivers; slide *Hohe Signale (UHF und höher)* → "Signals at high frequencies (UHF and above)" — the German means high-frequency, not strong, signals (see errors).
- low_noise_block: *Low Noise Block Converter (LNB)* → "low-noise block converter (LNB)"; *Bias-T / BIAS-T* → bias tee (AF231); *SAT-Spiegel* → satellite dish; *Amateurfunkverkehr über Satelliten* → "amateur radio communication via satellite".
- s_meter: *S-Wert* → "S reading", *S-Stufe* → S unit; *Abb.* → "Fig.", as in gleichrichter_2; *an 50 Ω* → "across 50 Ω"; slide *sind 3-Stufen* → "is 3 S units", *4-fache / 10-fache / 100-fache Leistung* → "4 / 10 / 100 times the power"; "S9 + 20 dB" and "S9+8 dB" forms unchanged.
- daempfungsglieder: *symmetrisch aufgebautes Dämpfungsglied* → symmetrical attenuator (DECISIONS.md, AD805, AD806); *ohmsche Dämpfungsglieder* → resistive attenuators; *PI-Konfiguration* → "pi configuration", slide note "as a &Pi;" with the entity unchanged.
- agc_1: *Automatische Verstärkungsregelung (Automatic-Gain-Control, kurz AGC)* → "*Automatic gain control* *(AGC)*" (bracket rule; EF211, EF212); *ALC (Automatic-Level-Control)* → "ALC (automatic level control)"; *Ansprechzeit, Abfallzeit* → attack time, decay time; menu labels *AGC Slow / Normal / Fast / Off* unchanged; *Digimodes* → data modes (glossary §8); *Morsen* → Morse.
- Solutions: *Ausschlussverfahren* → "by elimination"; *vervierfacht / verzehnfacht* → "quadrupled / multiplied by ten"; *Einsetzen der gegebenen Werte ergibt* → "Substituting the given values gives"; AF104 "… um $…$ erhöht." → "has increased by $…$ in total.", so the sentence still ends after the formula; AF206 *in den Hilfsmitteln* → "among the examination aids" (glossary §14); AD801, AD802, AF208 rewrapped to the German line count; German spaced hyphens used as dashes → en dashes, as in earlier units; decimal commas → points throughout (`\qty{3,455}` → `\qty{3.455}`, `\num{3,98}` → `\num{3.98}`).

## Suspected errors in the German original

- slides/doppelueberlagerungsempfaenger_doppelsuper.md (AF120 working) — "$f_\text{E}+f_\text{ZF1} = \qty{3,65}{…}+\qty{50}{…} = \qty{53,64}{\mega\hertz}$": 3.65 + 50 = 53.65 MHz, as the summary line of the same slide gives. Kept.
- slides/doppelueberlagerungsempfaenger_doppelsuper.md (AF120 working) — "gegeben: $f_\text{NF} = \qty{455}{\kilo\hertz}$": 455 kHz is the third IF of the receiver in AF120 (three oscillators VFO, CO1, CO2), not an audio frequency; the symbol says *NF*. Kept.
- slides/doppelueberlagerungsempfaenger_doppelsuper.md (AF210 working and "Oszillator-Frequenzen") — "$f_\text{ZF} = |f_\text{E} − f_\text{OSZ}| \Rightarrow f_\text{OSZ} = f_\text{ZF} \pm f_\text{E}$": from the difference follows $f_\text{OSZ} = f_\text{E} \pm f_\text{ZF}$; $f_\text{ZF} - f_\text{E}$ (the 20–47 MHz of AF210) comes from the sum product $f_\text{ZF} = f_\text{E} + f_\text{OSZ}$. The section's own rule ("Oszillatorfrequenz = Eingangsfrequenz ± Ausgangsfrequenz") gives $f_\text{E} - f_\text{ZF}$ as the second case, which differs from the slide's $f_\text{ZF} - f_\text{E}$. Kept.
- sections/doppelueberlagerungsempfaenger_doppelsuper.md — "Die 1. ZF sollte daher das Doppelte der maximalen Empfangsfrequenz betragen" (also on the slide): AF114's correct answer says *higher than* twice the maximum receive frequency, and avoiding direct reception of the IF (the reason given) does not by itself lead to a factor of two. Kept.
- slides/daempfungsglieder.md (AD806 working) — "gesucht: $\Delta P = P_2 - P_1$" and "$\Delta P = P_2 - P_1 = \qty{100}{\watt} - \qty{1}{\watt}$": with $P_1 = \qty{100}{\watt}$ and $P_2 = \qty{1}{\watt}$, $P_2 - P_1$ is −99 W; the subtraction actually written is $P_1 - P_2$. Kept.
- sections/vorverstaerker_daempfungsglied.md — caption of picture 1054 (`e_att_blockschaltbild`) "Vorverstärker im Überlagerungsempfänger", the same caption as picture 839, while the text says this figure shows the block symbols of attenuators (T and π). Kept ("Preamplifier in a superhet").
- slides/vorverstaerker_daempfungsglied.md — "Hohe Signale (UHF und höher)" where the section says "höheren Frequenzbereichen (VHF und höher)"; "im Empfangsbereich" where the section says "Eingangsbereich". Kept.
- sections/intermodulation_kreuzmodulation.md and slide — the IP3 as the point "an dem unerwünschte Mischprodukte 3. Ordnung den Amplitudenwert des Eingangssignales erreichen": as the in-depth part of the same section says, it is the extrapolated point where the 3rd-order products reach the output power of the fundamental (wanted) signals, not the amplitude of the input signal. Kept.
- sections/ueberlagerungsempfaenger_einfachsuper_1.md — "den Detektorempfänger im vorherigen Kapitel": the crystal set is the previous section of the same chapter. Kept ("in the previous chapter").
- Typos with no effect on the English: sections/aufbau_empfaenger.md "das wichtigste Bestandteil"; sections/mischer_2.md "Zum erreichen", "(Kathode jeweils mit folgender Anode der folgenden Diode verbunden)"; slides/mischer_2.md "Mathematischen Verhalten"; sections/doppelueberlagerungsempfaenger_doppelsuper.md tip "entsprechend dem des Doppelsupers"; sections/ueberlagerungsempfaenger_einfachsuper_2.md "Der ZF-Filter"; slides/trennschaerfe_1.md "das zu empfangene Signal"; sections/bfo_2.md "widergegeben"; slides/intermodulation_kreuzmodulation.md "des Eingangssignal"; caption "Wirkungsweise eine Begrenzverstärkers" (section and slide; the ident `begrenzverstärker` kept, as idents never change); slides/vorverstaerker_daempfungsglied.md "Verzerrrte"; sections/agc_1.md "bzgl. Ihres"; slides/agc_1.md "Ansprechsverhalten"; slides/s_meter.md "3-Stufen"; the stray `‚` after `--- style="font-size: smaller;"` (3×) in slides/doppelueberlagerungsempfaenger_doppelsuper.md, kept as markup.

## Provjera

Checked against `git show 31788eba~1:<file>` for all 57 files, paragraph by
paragraph, and against the English of every embedded question (NF201, NF303,
EF101, EF102, EF208–EF212, EF217, EF218, AA113, AA114, AD801–AD806,
AF101–AF120, AF201–AF214, AF216–AF223, AF226, AF230, AF231). Complete:
nothing dropped or added. Numbers, formulas and markup intact;
`revizija-guard.py --rev 31788eba~1 --brojevi`: 55 files, *struktura
netaknuta*; the two `detektorempfänger.md` files, which the guard skips,
checked with its own `signature()` and `numbers()`: unchanged. Line counts
equal to the German in every file.

Changes: omission 0, meaning 2, technical 1, style 9, glossary 2.

- ueberlagerungsempfaenger_einfachsuper_1 (meaning): "the signal is only demodulated after reception and … amplification" read as if demodulation came only afterwards; the German says that after reception and amplification the signal is *merely* demodulated → "after reception and, where necessary, amplification, the signal is simply demodulated".
- mischer_2 (meaning): *ausreichend durchgesteuert* → "driven sufficiently into conduction", not "turned fully on", which dropped *ausreichend* and overstated it.
- intermodulation_kreuzmodulation (technical): *Betrieb im nichtlinearen Grenzbereich* → "operation at the edge of its range, in the non-linear region"; "non-linear limit region" is not an English term. Glossary row reworked accordingly.
- spiegelfrequenzen (style, section and slide): *konzeptbedingt* "By the very nature of the concept, …" → "In a superhet, the mixing process … by its very nature always gives …"; *prinzipbedingt* "By its very principle" → "inherently". Glossary row reworked (*by its very nature / inherently*).
- intermodulation_kreuzmodulation (style): "the effect shows itself in that …" (twice) → "the effect is that …"; "may not both be zero" → "must not both be zero" (British *may not* can read as "might not"); "unwanted mixing products in the receiver input by strong signals" → "by strong signals at the receiver input".
- bfo_2 (style): "the BFO must be a certain distance from the CW signal. This distance …" → "must be offset from the CW signal by a certain amount. This offset …".
- aufbau_empfaenger "built up" → "constructed"; daempfungsglieder "commonest" → "most common"; solution AD805 stray comma after "the load resistor" before the displayed formula removed.

Translator's judgement calls: all kept except *konzeptbedingt / prinzipbedingt*
(reworked above). Glossary: 31 rows reviewed, 29 kept, 2 reworked
(*konzeptbedingt / prinzipbedingt*, *nichtlinearer Grenzbereich*). DECISIONS.md:
no entry added, none needed. The suspected errors in the German are confirmed
as listed (in particular 53.64 vs 53.65 MHz, $f_\text{NF}$ for the 455 kHz third
IF, the AD806 $\Delta P$ sign, $f_\text{OSZ} = f_\text{ZF} \pm f_\text{E}$, the
IP3 definition against the section's own in-depth text, and the picture 1054
caption) and kept as translated.
