# nea_modulation — translation report

Chapter "Modulation": 19 sections, each with its slides, and 6 solutions.
44 files:

- `contents/sections/` and `contents/slides/`: `rauch_und_morsezeichen.md`,
  `unmodulierter_traeger.md`, `modulationsarten.md`, `sprachsignale.md`,
  `am.md`, `am_2.md`, `ssb.md`, `ssb_2.md`, `ssb_3.md`, `fm.md`, `fm_2.md`,
  `fm_3.md`, `pm.md`, `bandbreite.md`, `bandbreite_2.md`, `bandreite_3.md`,
  `trxmodulation.md`, `dynamik_kompressor_1.md`, `dynamik_compressor_2.md`.
- `contents/solutions/`: `AE202.md`, `AE308.md`–`AE312.md`.

`revizija-guard.py --brojevi`: 44 files checked, *struktura netaknuta*.
German-word grep: no hits; the only non-English strings left are idents
(`a_pep_hüllkurve`), the `%` comments (`% Tastkopf 1:1 PEP`, `%[class:N]`),
formula subscripts (`f_{\textrm{mod max}}`, `\hat{U}_\mathrm{T}`), and the
German words quoted on purpose in the *USB* warning (*unteres Seitenband*).
Line counts, blank lines, trailing spaces and the final-newline state are
the same as in the German (also the files without a final newline and the
two trailing blank lines of sections/bandbreite.md and sections/fm.md).

Embedded questions looked up in English and the prose aligned with them:
NE101, NE102, NE201–NE212, NE301–NE306, EE101, EE201–EE207, EE301–EE306,
EF306, EF310, EJ210, EJ211, EJ215, EA105, AE101, AE201–AE205, AE207–AE213,
AE301–AE313, AI304–AI306, BC202, BC203, BC216, VD738–VD742 (e.g. NE201
"switching an RF carrier on and off", NE102 "types of modulation", EE306
"the deviation of the carrier frequency", EE305 "deviation setting", EE303
"in motor vehicles", AE201 "modulation depth", AE204 "sideband splatter",
AE205 "splatter", AE210 "AF compressor … dynamic range", AE211 "mean
transmitter power is raised with little distortion", AE213 "equaliser …
matched to the operator", AE302 "impulse interference … sparking", AE303
"varactor diode", AE306 "adjacent-channel interference", AE308 "Carson's
rule", AE310 "peak deviation … channel spacing", VD738 "maximum permitted
occupied bandwidth of an emission", EJ215 "closely adjacent frequencies").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

20 rows: *Hilfsmittel* (medium), *Morsezeichen geben*, *Modulationsarten*
as a concept (types of modulation), *Sprachsignal / Sprachspektrum /
Audiospektrum*, *Phasenlage*, *Additionstheoreme für Winkelfunktionen*,
*ausschlagen* (spectrum display), *unteres / oberes Seitenband, englisch
…*, *Einseitenbandmodulation, gebräuchlicher englisch …*,
*Trägerfrequenzauslenkung / Frequenzauslenkung / Trägerauslenkung*,
*Lautstärkeinformation*, *Hub-Regler*, *Schmalband-FM (englisch Narrow-FM,
kurz NFM)*, *Spitzen-Hüllkurvenleistung / Tastkopfverhältnis*,
*Zweiton-Nutzsignal / Eintonsignal*, *Winkelmodulationstechniken /
Phasensprung / Flanke*, *Kanalleistungsmessung /
Nachbarkanalleistungsmessung*, *zus. Nutzungsbedingungen / Auszug*,
*Dynamic Compressor / NF-Dynamikkompressor / Sprachkompressor*,
*prägnant und durchdringend*.

## Added to `DECISIONS.md`

One entry (Course text): a remark that only a German reader needs — the
warning that *USB* is not *unteres Seitenband* — is kept as information
about German usage, as the glossary's *Relais oder Repeater* row does;
a German gloss that only gives the English term is dropped (bracket rule).

## Judgement calls

- rauch_und_morsezeichen (section and slides): *Hilfsmittel* (the smoke, the oscillation that is then called the carrier) → "medium"; "aid" would not read as the thing that carries the message, and "aid" is kept for the examination aids (formula sheet, band plan). *Morsezeichen* → "Morse characters" (glossary §2), also in the slide heading; *Morsezeichen zu geben* → "*sending* Morse characters"; *Continuous Wave (CW)* → "continuous wave (CW)", lower case as NE201. *Modulatio … Taktmaß bzw. Rhythmus* → "measure or rhythm". German spaced hyphens used as dashes → en dashes, as in earlier units.
- rauch_und_morsezeichen slides: *Andere Modulationsarten* → "Other types of modulation"; *Modulationsart(en)* as a concept → "type(s) of modulation" throughout (NE102), *mode* only for the radio's *Mode* switch and its table (trxmodulation) and where the German means the operating mode (bandbreite: *hängt … von der Modulationsart … ab* → "depends on the mode").
- unmodulierter_traeger: *Kurvenform* → "waveform"; *Mit einem unmodulierten Träger kann ohne weitere Modulation z.B. durch Ein- oder Ausschalten keine Information übertragen werden* → "Without some further modulation, e.g. switching it on or off, an unmodulated carrier cannot transmit any information".
- sprachsignale: *Amplitudenspektrum* → "amplitude spectrum" (glossary §14); *Modulationssignal* → "modulating signal" (glossary §7), also in the later sections.
- am slides note: *Vertiefung* → "In depth" (the label of the in-depth box), the 50ohm link kept; *Additionstheoremen für Winkelfunktionen* → "trigonometric addition formulas".
- am_2: *Hüllkurvendemodulator* → envelope detector (glossary §6); *vollständig ausgesteuert* → "fully driven"; *(inkl. Abbildung … in der Formelsammlung)* → "(included, with Figure …, in the formula sheet)"; slides *Lösungsweg / gegeben / gesucht* → "Solution / given / required", as in earlier units; `0,5` → `0.5`.
- AE202: *Kästchen* → "square" (glossary §14).
- ssb: *Im Englischen wird von "lower sideband" (LSB) … und "upper sideband" (USB) … gesprochen* → the English names are given with the abbreviations in the preceding sentence, "the "lower sideband" (LSB) lies below the carrier … and the "upper sideband" (USB) above it" (bracket rule). The `<attention>` box and the slide *(im Deutschen wird es gerne mit Unteres Seitenband verwechselt)* are kept as information about German usage (DECISIONS.md). *Einseitenbandmodulation … Gebräuchlicher ist dafür die englische Bezeichnung single-sideband modulation, kurz SSB* → "single-sideband modulation, *SSB* for short"; slide *Einseitenbandmodulation bzw. single-sideband (SSB)* → "*Single-sideband modulation* (*SSB*)". The bare "in [ref:n_seitenband_3]" → "in Figure [ref:…]", as in earlier units.
- ssb_2: *Gebegeschwindigkeiten von 20 Wörtern pro Minute (100 Zeichen pro Minute)* → "sending speeds of 20 words per minute (100 characters per minute)"; *Im Kapitel Dynamikkompressor* → "in the chapter on the compressor" (chapter titles not yet translated; descriptive, as in earlier units). Slides: *Bandfilter* → band-pass filter (glossary §5), *Afu-Band* → amateur band, *Vorauswahl von USB und LSB* → "Preselecting USB or LSB", decimal points in all frequencies.
- ssb_3: *Nebenaussendungen* → spurious emissions (glossary §6); *Spitzen-Hüllkurvenleistung (PEP)* → peak envelope power (PEP); *effektive Leistung / Effektivleistung* → RMS power (glossary §11, as AI305/AI306 ask for a power from a measured voltage); *Tastkopfverhältnis* → probe ratio; *Zweiton-Nutzsignal* → two-tone wanted signal; slide note *PEP = Peak Envelope Power* → "PEP = peak envelope power".
- fm: *Schmalband-FM (englisch Narrow-FM, kurz NFM)* → "narrowband FM (NFM)" (bracket rule, glossary §2); *der bei der Prüfung als Hilfsmittel vorliegt* → "which is available as an aid in the examination"; slide formula `\text{Bandbreite} … \text{Hub} … \text{Bandbreite des NF-Signals}` → `\text{Bandwidth} … \text{deviation} … \text{bandwidth of the AF signal}`: running words, not subscripts.
- fm_2: *Trägerfrequenzauslenkung (Frequenzhub)* → "*deviation of the carrier frequency (frequency deviation)*", EE306's wording; *Frequenzabweichung (Frequenzhub)* of the carrier → "frequency excursion (frequency deviation)", not *frequency error*, which is *Frequenzabweichung* of an oscillator (glossary §14); *Hub-Regler* → "deviation control" (EE305 "deviation setting"); *KFZ / Kfz* → motor vehicles / vehicles (EE303). The space before the full stop in "… des FM-Signals führen ." is kept.
- fm_3: *systembedingt* → "by its very nature" (glossary §14); *Kapazitätsdiode* → varactor diode (AE303); *(vgl. [ref:…])* → "(see Figure [ref:…])"; slide note *im Kapitel Sender* → "in the chapter on transmitters".
- AE308–AE312: *Einsetzen ergibt* → "Substituting gives" (glossary *Mit eingesetzten Werten*); *Summanden* → "terms" (AE310).
- pm: *„Versatz"* → "offset"; *Winkelmodulationstechniken* → angle modulation techniques; *Für mathematisch Interessierte* → "For the mathematically minded"; *Nutzsignal* → wanted signal (glossary §6).
- bandbreite: first mention in the section and on the slides "Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)", afterwards "AFuV"; *Anlage 1* → "Annex 1 to the AFuV" (glossary §1.2), also the table caption *Auszug AfuV Anlage 1* → "Extract from Annex 1 to the AFuV"; table header *zus. Nutzungsbedingungen* → "Add. conditions of use"; status letters P/S unchanged; *Bundesgesetzblatt mit der neuen Verordnung* → "Federal Law Gazette with the new ordinance", link unchanged; *Falsch / Richtig* captions → "Wrong / Right", keeping the `--`.
- bandreite_3: *ausgesendeter Bandbereich* → "the part of the band transmitted"; *Kanalleistungsmessung, Nachbarkanalleistungsmessung* → channel power measurement, adjacent-channel power measurement.
- trxmodulation: table *SSB unteres Seitenband ("lower sideband")* → "SSB lower sideband" (bracket rule); caption *Häufig verwendete Modulationsarten* → "Commonly used modes" (the column is headed *Mode*); slide note *Seefunk* → maritime radio (glossary §14).
- dynamik_kompressor_1, dynamik_compressor_2: *Kompressor / Dynamikkompressor* → compressor (glossary §14); *Dynamic Compressor* (the German's English name of the function) → "dynamic compressor", lower case as a term; *NF-Dynamikkompressor oder NF-Sprachprozessor* → "AF compressor, or audio speech processor" (AE210, glossary §14); *prägnanter und durchdringender* → "punchier and more penetrating"; *2. Empfänger* → "a 2nd receiver", keeping the digit for the number check; *Dummy-Load* → dummy load.

## Suspected errors in the German original

- sections/ssb.md — "Die bei SSB belegte Bandbreite … Bei den Beispielen für SSB in [ref:n_seitenband_3] also 2700 Hz und somit etwas weniger als die Hälfte der Bandbreite von AM": the example speech signal of sprachsignale runs from 300 Hz to 2700 Hz, which that section itself gives as a bandwidth of 2400 Hz; 2700 Hz is exactly half the 5400 Hz that am gives for AM, so "a little less than half" fits only 2400 Hz. Kept.
- sections/pm.md (indepth) — $f_i(t) = \frac{1}{2\pi} \cdot \frac{d\varphi(t)}{dt}$ with "die Frequenz ist die zeitliche Ableitung der Phase": with $s(t) = A_c \cos(2\pi f_c t + \varphi(t))$ as written just above, the instantaneous frequency is $f_c + \frac{1}{2\pi}\frac{d\varphi}{dt}$; the formula as given is the instantaneous frequency deviation. Kept.
- sections/fm.md (indepth) and slides/fm.md — the FM bandwidth as twice "Hub und der Bandbreite des NF-Signals": Carson's rule, as fm_2 and fm_3 write it, uses the highest modulating frequency $f_\mathrm{mod\,max}$, not the bandwidth of the AF signal; for a 300–3000 Hz signal the two differ. Kept.
- slides/dynamik_compressor_2.md — "Dazu wird das NF-Signal in einem dynamischen Equalizer verstärkt und gedämpft": the section describes a compressor (gain depending on level), not an equaliser (gain depending on frequency), which ssb_3 introduces separately. Kept ("dynamic equaliser").
- slides/am_2.md — "Signal steuert zwischen Träger und maximal möglichem Wert aus" (for $m = 1$): the section says the envelope then varies between zero and twice the unmodulated carrier amplitude. Kept.
- Typos with no effect on the English: sections/am.md "Übertagung", double space in "zwischen  minimaler"; slides/am.md "kann *Additionstheoremen* … nachschlagen"; sections/sprachsignale.md "mit kleiner und große Amplitude", caption "Beispiel für ein Audiospektrums" (the slide has "Audiospektrum"); sections/fm_2.md "Eine lauteres NF-Signal", "führen ." ; sections/fm_3.md caption "Einfache Schlatung"; slides/ssb_2.md "Ausgangleistung"; sections/bandbreite.md caption and slides/bandreite_3.md "AfuV" for *AFuV*; sections/rauch_und_morsezeichen.md "τηλε" without the accent the slides give (τῆλε); the file name `bandreite_3` (for *bandbreite_3*) kept, as file names never change.

## Provjera

Checked all 44 files paragraph by paragraph against `git show 40104cd~1`
(German), the embedded English questions looked up in
`contents/questions/fragenkatalog3b.json`, and the 20 glossary rows and the
DECISIONS.md entry of the commit. Nothing dropped or added; numbers,
formulas and markup intact. `revizija-guard.py --rev 40104cd~1 --brojevi`:
44 files, *struktura netaknuta*.

Changes: omission 0, meaning 0, technical 3, style 5, glossary 3.

- technical — sections/am_2.md: *vollständig ausgesteuert* (carrier at $m=1$) "fully driven" → "fully modulated", the English phrase for 100 % modulation; "driven" suggests the drive level of an amplifier. Glossary row added.
- technical — sections/pm.md (3×): *Nutzsignal* $m(t)$ "wanted signal" → "information signal", as NE202/NE301 render *Informationssignal*; *wanted signal* is the receiver's sense (wanted vs. interfering) and reads wrongly for the message $m(t)$. Glossary row added. In ssb_3 *Nutzsignal(e)* stays "wanted signal(s)", where the text speaks of intermodulation between them.
- technical — sections/ssb_3.md: *Tastkopfverhältnis* "probe ratio" → "the probe's division ratio", the glossary's existing term (*Teilverhältnis (Tastkopf)*, oszilloskop units); the new glossary row changed accordingly.
- style — sections/fm_2.md: the stray space before the full stop ("FM signal .") removed; a typo in the German, no reason to copy it.
- style — sections/fm_3.md: "impulse interference to the amplitude" → "impulse interference affecting the amplitude".
- style — sections/pm.md: "The stronger the amplitude" → "The larger the amplitude".
- style — sections/dynamik_kompressor_1.md: "periods of low or quiet drive" → "quiet periods of low drive".
- style — solutions/AE308.md: "Given are the frequency deviation …" → "The given values are the frequency deviation …".
- glossary — the *Trägerfrequenzauslenkung* row now also records *Frequenzabweichung (Frequenzhub)* of an FM carrier → "frequency excursion (frequency deviation)", as fm_2 has it, so it is not taken for the oscillator's *frequency error*.

Kept after review: *Hilfsmittel* → "medium" (rauch_und_morsezeichen); *Modulationsart* → "type of modulation" / "mode" split; the DECISIONS.md entry on the *USB* warning; RMS power for *effektive Leistung* in the PEP definition (glossary §11); all other judgement calls and glossary rows. The suspected errors in the German are confirmed as listed (ssb 2700 Hz vs. 2400 Hz, pm instantaneous frequency, fm AF bandwidth vs. $f_\mathrm{mod\,max}$, the "dynamic equaliser" on the compressor slide, am_2 slide on $m = 1$).
