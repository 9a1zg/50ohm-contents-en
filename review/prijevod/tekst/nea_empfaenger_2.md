# nea_empfaenger_2 — translation report

Chapter "Empfänger (2/2)" (Receivers, part 2): 13 sections, each with its
slides, and 10 solutions. 36 files:

- `contents/sections/` and `contents/slides/`: `agc_2.md`,
  `snr_rauschzahl.md`, `rauschen.md`, `rit.md`, `vox.md`, `squelch.md`,
  `squelch_2.md`, `notchfilter.md`, `noise_reduction.md`, `demodulator.md`,
  `frequenzmessung_1.md`, `frequenzmessung_2.md`, `frequenzgenauigkeit.md`.
- `contents/solutions/`: `AA115.md`, `AA116.md`, `AB408.md`, `AB409.md`,
  `AD503.md`, `AI506.md`–`AI510.md`.

`revizija-guard.py --brojevi`: 36 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comments (frequenzmessung_1,
noise_reduction, unchanged), formula subscripts (`f_\text{ZF}`,
`u_\mathrm{NF}`, `f_\text{Anzeige}`, `f_\text{Baken}`, `f_\text{Abstand}`,
`f_{B,\mathrm{max},\text{Abw}}`), idents, and the word *Rauschmaß* named on
purpose in the snr_rauschzahl in-depth box. Line counts, trailing spaces
(markdown line breaks in the solutions and in slides/demodulator.md,
slides/frequenzmessung_2.md), the whitespace-only lines (frequenzmessung_1,
frequenzgenauigkeit), the leading space of frequenzmessung_1 line 24 and the
final-newline state are the same as in the German in every file.

Embedded questions looked up in English and the prose aligned with them:
AF224, AF225, AF227–AF229, AB408, AB409, NF109–NF112, NF302, EF213–EF216,
AD501–AD506, EI501–EI504, AI501–AI511, AA115, AA116 (e.g. AF224 "reduces the
gain of amplifier stages", AD503 "the output for an AGC voltage", AF228 /
AF229 noise figure in dB vs noise factor F = 2, AF225 "The IF or AF
signals", NF111 "SSB voice", EF214 "pulse-type interference", "noise
blanker", EF213 "noise reduction (NR)", AD501/AD504/AD506 "envelope
detector", "slope detector", "product detector", AD505 "PLL FM demodulator",
AI511 "synchronised to GPS", AI504 "timebase oscillator", AI505 "gate time",
"the resolution", AI510 "beacon segment"; the answers quoted in solution
AD503 are the English answers verbatim).

## Added to `TRANSLATION_GLOSSARY.md` (§14)

28 rows: *Regelkreis / Regelwirkung*; *Regelspannung* of a VCO (control
voltage); *Phasenregelschleife* inside a PLL description; *aufmodulierte
NF*; *Rauschzahl … in Dezibel / Rauschmaß (laut DIN)*; *Pegeländerung der
Rauschleistung / Bezugsbandbreite*; *über das Band wandern*;
*Sprachfrequenzen gespiegelt*; *"Clarifier" / "CLAR RX"*; *Rauschsperre …
englische Begriff Squelch (SQL)*; *Sendepausen*; *Kerbe / Name
Notch-Filter*; *feste Trägerkomponenten*; *impulsförmige Störungen*;
*Kurzwellenfunkgerät*; *neu abgleichen / Abgleich / Abgleichanleitung*;
*abgesetzte Drei / vor dem Komma / Nachkommastellen*; *Frequenzmessbereich /
Bedienungsanleitung*; *Perioden … Flanken oder Nulldurchgänge / direkt
zählender Frequenzzähler*; *Aktualisierung / Notbehelf*;
*GPS-synchronisierter Oszillator* with and without *(GPSDO)*;
*Frequenzgenauigkeit / relative Abweichung*; *Abw.* in worked slides;
*Lösungsweg Teil 1/2*; *Hinweis bzgl. … 10er Potenzen*; *Gemessene Frequenz /
Anzeigefrequenz / Messwert*; *»das Komma schieben«*; *Vorüberlegung*.

## Added to `DECISIONS.md`

None. The choices of this unit follow existing entries: the bracket rule
(*Notch-Filter (Kerbfilter)*, *Rauschsperre (Squelch)*, *Störaustaster bzw.
Noise Blanker*), a remark only a German reader needs kept as information
about German usage (the DIN *Rauschmaß*, as the *USB* entry), *Figure* for
numbered references, *Solution / given / required* in worked slides,
*Method 1/2* for two methods (glossary §14), running words in formulas
translated and subscripts kept.

## Judgement calls

- agc_2: *In der Klasse E … kennen gelernt* → "In Class E we have already met", as earlier units; *Empfängerzweig* → receive path (glossary §6; AF224 says "receive section" for the German *Empfangsteil*); *die NF übersteuern* → "overdrive the AF stages"; *AGC-Regelspannung* (caption) → "AGC voltage", *Regelspannung* → *AGC voltage* (AD503), *geschlossener Regelkreis* → closed control loop; *das hochfrequente ZF-Signal* → "the high-frequency IF signal" (high relative to the AF, not an RF stage).
- snr_rauschzahl: German *Rauschzahl* is used for the ratio and for its dB value; English splits it (glossary §6). The ratio sentences say "noise factor"; *wird üblicherweise mittels Logarithmierung in Dezibel dargestellt* → "is usually converted to a logarithm and expressed in decibels, as the *noise figure*", and "a noise factor of 2 … corresponds to a noise figure of 3 dB". The in-depth box (DIN calls the dB value *Rauschmaß*, a term "nicht sehr verbreitet") is about the German word and stays so: "is called the *Rauschmaß* in German … this German term is not very widespread" — in English *noise figure* is the common term, so translating the remark onto it would be false. Slide heading *Rauschzahl* → "Noise factor"; slide *Rauschmaß* → noise figure.
- rauschen: *ins Verhältnis gesetzt* → "expressed as a ratio of one to the other"; the symbols $p_\text{r}$ / $\Delta P_\text{R}$ unchanged (see errors).
- rit: *Sprechfunk mit SSB-Modulation* → "SSB voice operation" (glossary §2, NF111); "Clarifier" / "CLAR RX" quoted as the manufacturers' labels; *gespiegelt* → inverted; *"über das Band wandern"* → "wander across the band"; *für eine Gegenstation* → "for each station you work"; *Wie schon bei der Modulation erwähnt* → "As already mentioned in the chapter on modulation"; slide *versteht mich die Gegenstation schlecht* → "makes it hard for the other station to understand me".
- vox: *PTT-Taste* → PTT button (glossary §14); *voice-operated exchange* kept lower case and italic as the German has it.
- squelch: *Rauschsperre … Meist wird für diese Funktion der englische Begriff Squelch (Abkürzung: SQL) verwendet* → "a *squelch* (abbreviation: SQL)": English has one word, so the sentence that only names the English term is dropped (bracket rule) and the abbreviation moves to the first mention; slide *Englisch Squelch (SQL)* → "Abbreviated *SQL*". *zu schwach / zu stark eingestellt* → "set too low / too high"; *in Sendepausen gerade nicht mehr rauscht* → "the noise just disappears in the pauses between transmissions"; the long caption of picture 737 translated identically in all three places.
- squelch_2: *die Rauschsperre (Squelch)* → "the squelch" (bracket rule).
- notchfilter: *Notch-Filter (Kerbfilter)*, slide *Notch-Filter oder Kerbfilter* → "notch filter" (bracket rule); *Kerbe … Daher auch der Name Notch-Filter* → "a notch … hence the name notch filter", which works in English as it stands; *Auto-Notch-Filter* → automatic notch filter (glossary §14); *parametrisiert* → "set precisely".
- noise_reduction: *impulsförmige Störungen* → "pulse-type interference" (EF214); *Störaustaster bzw. Noise Blanker (NB)* → "noise blanker (NB)" (bracket rule); *Kurzwellenfunkgerät FT-710* → "the FT-710 HF radio"; the `% TODO` comment unchanged.
- demodulator: *Die einfachste Form der Demodulation … stellt die Amplituden-Modulation (AM) dar* → "Amplitude modulation (AM) offers the simplest form of demodulation of a radio-frequency signal" (see errors); *angepasster Schwingkreis* → "suitably tuned resonant circuit"; *aufmodulierte NF* → "the AF modulated onto the carrier"; *ZF-Frequenz* → "the IF"; *Regelspannung des VCO* → control voltage (not AGC voltage); *über eine Phasenregelschleife frequenzfolgend … gekoppelt* → "locked … by a phase control loop so that it follows its frequency", to avoid "In a PLL … via a phase-locked loop"; *(FM-Modulation)* → "(frequency modulation)"; *PLL (Phase Locked Loop)* and *BFO (Beat Frequency Oscillator)* kept as ordinary expansions; *Durch Mischung (Produkt)* → "Mixing these two input signals (forming their product)"; *oberer Verlauf* → "upper trace"; slide heading `####  FM-Demodulation mittels PLL  ` kept with its double space.
- frequenzmessung_1: *neu abgleichen* → realign, *Abgleichanleitungen* → alignment instructions; *abgesetzte Drei* → "the separate three"; *vor dem Komma* → "before the decimal point" (English writes a point); *hoher Innenwiderstand* → "high internal resistance" (glossary §3, and as the earlier meter sections say); the commented-out photo block left as it is; *Messobjekt* → device under test (glossary §11).
- frequenzmessung_2: *Frequenzgenerator* → signal generator (glossary §11, AI511); *GPS-synchronisierte Oszillatoren* → "GPS-synchronised oscillators" (AI511's wording; no *GPSDO* given here); *temperaturstabilisierte Quarzoszillatoren (OCXO)* kept as written; *Frequenz des nicht ausgesendeten Trägers* → "the frequency of the carrier, which is not transmitted"; *Notbehelf* → makeshift; *direkt zählender Frequenzzähler* → "direct-counting frequency counter"; caption 1126 *bei sehr kleinen Torzeiten* → "with very short gate times".
- frequenzgenauigkeit: *GPS-synchronisierter Oszillator (GPSDO)* → "GPS-disciplined oscillator (GPSDO)" (the abbreviation decides, glossary §14); *maximal zu erwartende Frequenzabweichung* → "maximum frequency error to be expected" (glossary §14, not *deviation*); *10er Potenzen* → "powers of 10" (the digit kept for the number check); slides `$\textrm{Abw.} = …$` → `$\textrm{Dev.} = …$`, an abbreviated word naming the quantity, translated as `\text{Ordnung}` → `\text{order}` was in nea_empfaenger_1, while the subscript in $f_{B,\mathrm{max},\text{Abw}}$ stays; *Lösungsweg Teil 1/2* → "Solution, part 1/2"; AA116 slide `14,200.\qty{000}` → `14.200.\qty{000}`, as the English question writes "14.200.000 MHz".
- Solutions: *Gegeben / Lösungsweg / Abkürzung* → Given / Solution / Shortcut (glossary §14); AI506 *Lösungsweg 1 / 2* → "Method 1 / Method 2" (two methods to one answer, glossary §14); *Vorüberlegung* → "Preliminary consideration"; *Lösung über Ausschlussverfahren* → "Solution by elimination"; AD503 *im Kapitel "Demodulator"* → "in the chapter on the demodulator" (chapter titles not yet translated; descriptive, as in earlier units), *die Formel (Filter, RC-Tiefpass) aus der Formelsammlung* → "the formula (filter, RC low-pass) in the formula sheet", the section name lower case as glossary §14 *(Formelsammlung:) Pegel, …*; AI506 »das Komma schieben« → "move the decimal point" in English quotes; AI509 *Messwert* → "Reading"; decimal commas → points throughout (`\qty{14,2}` → `\qty{14.2}`, `0,1` → `0.1`, `\qty{2,8444}` → `\qty{2.8444}`).

## Suspected errors in the German original

- slides/rauschen.md (AB409 working) — "gegeben: $B_1 = \qty{2,5}{\kilo\hertz}$, $B_2 = \qty{0,5}{\kilo\hertz}$ … $\approx \qty{7}{\dB}$": with the formula as written this is +7 dB, an increase, while AB409's correct answer is a *decrease* by about 7 dB; solution AB409 assigns them the other way round ($B_2 = \qty{2,5}{\kilo\hertz}$ as the reference) and gets −7 dB. Kept.
- sections/rauschen.md, solutions/AB409.md — the same quantity is written $p_\text{r}$ (prose), $\Delta P_\text{R}$ (formula, "gesucht") and $\Delta p_\text{R}$ (AB409 working). Kept.
- sections/demodulator.md (in-depth box) — "Das ZF-Signal wird dadurch abwechselnd unverändert durchgeschaltet oder in seiner Polarität umgekehrt. In der vereinfachten Darstellung kann das ZF-Signal deshalb als Produkt aus dem NF-Signal und dem BFO-Schaltsignal betrachtet werden": the switching in the product detector does not make the incoming IF signal a product of AF and BFO signal ("deshalb" does not follow), and $u_\mathrm{ZF} = u_\mathrm{NF} \cdot s_\mathrm{BFO}$ describes a double-sideband suppressed-carrier signal, not an SSB signal. Kept.
- sections/demodulator.md — "Die einfachste Form der Demodulation eines Hochfrequenz-Signals stellt die Amplituden-Modulation (AM) dar" names a modulation as a form of demodulation; "das gewünschte NF-Signal (SSB-Signal)" calls the demodulated AF the SSB signal. Kept (rendered "AM offers the simplest form of demodulation …", "the desired AF signal (SSB signal)").
- slides/frequenzmessung_2.md — "Lange Torzeit: höhere Messgenauigkeit": the section says a longer gate time gives a finer *resolution* and that "Die Genauigkeit der Frequenzmessung ist von der Auflösung zu unterscheiden" (accuracy depends on the timebase); AI505's correct answer is also "die Auflösung". The slide also says "fast immer" where the section says "häufig". Kept.
- solutions/AA116.md — "$\frac{14,2\cdot \qty{\cancel{10^6}}{\mega\hertz}}{\cancel{10^6}}$" (twice): $14.2 \cdot 10^6$ is in hertz, not megahertz, as the slide working has it. Kept.
- solutions/AI509.md — "$\qty{145}{\mega\hertz} - \qty{1450}{\mega\hertz}$" (and +): $\Delta f$ is 1450 Hz, as computed one line above and on the slide. Kept.
- Typos with no effect on the English: sections/agc_2.md "bereites kennen gelernt"; sections/rauschen.md "die folgende Fragen"; sections/rit.md "eines Transceiver"; sections/squelch.md "SSB-modulierte Signalen"; sections/demodulator.md "eines sog. Hüllkurven-Demodulator"; sections/frequenzmessung_1.md the leading space before "In Abbildung" (kept as markup); picture 77 carries the ident `demodulator_pll` in the section and `a_fm_demodulation_pll` on the slide (idents never change).
