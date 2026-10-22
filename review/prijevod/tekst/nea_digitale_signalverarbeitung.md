# nea_digitale_signalverarbeitung — translation report

Chapter "Digitale Signalverarbeitung" (Digital signal processing): 9
sections, each with its slides, and 6 solutions. 24 files:

- `contents/sections/` and `contents/slides/`:
  `digitale_signalverarbeitung_einleitung.md`, `sampling_quantisierung.md`,
  `abtasttheorem.md`, `dac_adc.md`, `anti_alias_rekonstruktionsfilter.md`,
  `fourier_transformation.md`, `digitale_filter.md`, `digital_iq.md`,
  `latenz.md`.
- `contents/solutions/`: `AB404.md`, `AB405.md`, `AB406.md`, `AB407.md`,
  `AF619.md`, `AF622.md`.

`revizija-guard.py --brojevi`: 24 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comment block of
sections/anti_alias_rekonstruktionsfilter.md (unchanged), the formula
subscript `f_\text{abtast}` (AF622) and the two applet labels kept in
brackets on purpose (sampling_quantisierung, DECISIONS.md). Line counts,
blank lines (the leading empty line of sections/latenz), trailing spaces
(markdown line breaks in the solutions and in the slides of abtasttheorem,
fourier_transformation, digitale_filter, digital_iq, latenz; the trailing
spaces after "auf." and "Stereoanlagen." in sections/abtasttheorem, after
"Helligkeitseinstellungen" in slides/sampling_quantisierung), the leading
space of AF619 line 13, the four-space indent in slides/digital_iq and the
final-newline state are as in the German in every file.

Embedded questions looked up in English and the prose aligned with them:
EF601–EF603 ("A/D converter", "D/A converter", "digitised", "At least part
of the signal processing is implemented in software"), AF601–AF606
("continuous-time", "discrete-time", "continuous-value", "discrete-value",
"Quantisation", "Sampling"), AF607–AF614 ("quantisation errors", "8-bit
resolution", "step size between the voltage levels", "range of values"),
AF615 ("Samples per unit of time"), AF616–AF619 ("minimum sampling rate
theoretically required to reconstruct a signal without errors", "aliasing",
"higher than half the sampling frequency", "aliasing effects",
"samples/s"), AF620 ("Sampling clock generator", "digital direct-sampling
receiver"), AF621 ("clock jitter", "Additional noise appears in the sampled
result"), AF622–AF625 ("anti-aliasing filter", "reconstruction filter",
"amplitude response"), AF630 ("discrete Fourier transform by means of the
FFT", "frequency spectrum"), AF631 ("FIR or IIR filters"), AF634–AF636
("centre or carrier frequency", "I and a Q component"), AF637 ("propagation
time or delay … in seconds"), AB404–AB407 (signal / spectrum pairs).

## Added to `TRANSLATION_GLOSSARY.md` (§14)

24 rows: *Sampling (… Probenahme) / Samples (Proben)*; *Samplingrate oder
Abtastrate*; *Abtastzeitpunkt / Abtastwert / Samplewert / Momentanzustand*;
*Zeitachse / Wertachse / Zeitdiskretheit / Wertdiskretheit*; *Dimmer /
Stufenschalter*; *Quantisierungsfehler / Quantisierungsstufen*;
*Zeitquantisierung / Wertquantisierung* with the applet labels;
*Abtasttaktgenerator / Taktgenerator / Taktrate*; *Nyquist-Shannon-
Abtasttheorem / Nyquist-Bedingung*; *Alias-Effekte bzw. Aliasing-Effekte /
Aliase*; *Moiré-Muster / räumliche Auflösung / Bildpunkte*;
*HiFi-Frequenzbereich*; *Zaunpfahlproblem*; *Stufen / Zwischenschritte /
Abstände*; *DFT / FFT*; the four waveform names; *ungeradzahlige /
geradzahlige / ganzzahlige Vielfache / Gleichanteil*; *Spektralanteil /
Spektralspitze*; *Finite / Infinite Impulse Response* with the dropped
gloss; the FIR terms (*gleitender Mittelwert, Faltungsoperation …*);
*Mixed Signal Frontends / Dezimationsfilter*; *Pufferspeicher (englisch
"buffer")*; *Laufzeit (Latenz)*; *Filmkamera / Bilder pro Sekunde*.

## Added to `DECISIONS.md`

None. Everything followed existing entries: the bracket rule (German glosses
of English words dropped), applet labels with the German label in brackets,
*Figure* before numbered references, *Given / Required / Solution* in
solutions, word subscripts kept and running words in `\text{}` translated.

## Judgement calls

- Throughout: *A/D-Umsetzer* / *D/A-Umsetzer* → "A/D converter" / "D/A converter", as the bank (AF607–AF625, EF601); *Analog-Digital-Umsetzer (A/D-Umsetzer)* → "analogue-to-digital converter (A/D converter)"; *AD-/DA-Umsetzer*, *AD/DA-Wandler* → "A/D and D/A converters"; *Stufen* → levels (AF610 "voltage levels"), *Schrittweite* → step size; *Wertebereich* → range of values (AF610–AF614); *Abbildung [ref:…]* → "Figure [ref:…]", *(vgl. Abbildung …)* → "(see Figure …)"; *Nutzsignal* / *Nutzfrequenzbereich* → wanted signal / wanted frequency range; *Klasse A* → Class A; German „…" → "…"; decimal commas → points (`\qty{44.1}{\kilo\sps}`, `\qty{22.05}{\kilo\hertz}`).
- digitale_signalverarbeitung_einleitung: *Dieser Prozess nennt sich Sampling (in Deutsch könnten man dies mit dem Wort Probenahme übersetzen)* → "This process is called sampling." and the slide's *Samples (Proben)* → "samples": the brackets only translate the English word back into German (bracket rule, DECISIONS.md); *SDR-Geräte* → "SDR equipment"; *Handys* → mobile phones; *bildgebende Systeme im medizinischen Bereich* → "medical imaging systems"; *Software Defined Radio* → "software-defined radio" (§6); the double space in the slide's *steht dabei  für* not kept (not a line break, nothing renders it); *Mehr dazu in Klasse A* → "More on this in Class A".
- sampling_quantisierung: *Samplingrate oder Abtastrate* → "*sampling rate* or *sample rate*" (both are established English names, so the pair stays a pair); *Stufenschalter* → "step switch", its *Stufen* → steps; the indepth's *An den Reglern kann man die Zeitquantisierung und die Wertquantisierung … einstellen* → "The sliders let you set the time quantisation (*Zeit-Sampling*) and the value quantisation (*Wert-Quantisierung*)": the applet `quantisierung_und_sampling` is still German and its sliders read *Zeit-Sampling:* and *Wert-Quantisierung:*, so the labels go in brackets (DECISIONS.md, applet labels; the German text paraphrases them); captions *Wert- und Zeitkontinuierliches Signal* etc. keep the German order ("Continuous-value and continuous-time signal"); slide *Der Vorgang der zeitlichen Abtastung wird als Sampling bezeichnet* → "The process of taking values at particular moments in time is called *sampling*" (English has one word for *Abtastung* and *Sampling*, so a literal rendering would define the word by itself); *Zeitdiskretheit und Wertdiskretheit* → "discrete time and discrete values".
- abtasttheorem: *Alias-Effekte, bzw. Aliasing-Effekte* → "what are known as aliasing effects" (one English term, AF618); *Nyquist-Shannon-Abtasttheorem oder Nyquist-Bedingung* → "Nyquist–Shannon sampling theorem or the Nyquist condition" (not *Nyquist criterion*, which in English usually names the intersymbol-interference criterion); *(merke: zeitdiskret)* → "(remember: discrete-time)"; *entsteht ein optisch kontinuierlicher Bewegungsablauf* → "the result is a movement that looks continuous"; digits written as digits kept ("between 2 successive pictures", "in at least 2 pictures"); *Bilder* → pictures, as in the introduction's camera; *ca.* → about; *Mit der folgenden Aufgabe kannst du …* → "You can test your knowledge … with the following exercise"; the slide's *Abtastung eines kontinuierlichen Signals* → "taking values of a continuous signal" (same reason as above); the line break inside the `<webonly>` paragraph kept.
- dac_adc: *Gegenspieler* → counterpart; *Abtasttaktgenerator* → sampling clock generator (AF620); *um Faktor 256 besser* → "better by a factor of 256"; captions *… und anschließende D/A-Umsetzung* → "…, followed by D/A conversion"; *15 Zwischenschritte* → "15 steps", the slide's *Abstände* → intervals; *Zaunpfahlproblem* → "fencepost problem", the established English name; *Clipping* → clipping.
- anti_alias_rekonstruktionsfilter: *Aliase* → aliases; *Moiré-Muster* → moiré patterns; *Bildpunkte* → picture elements; *Lektion zum Abtasttheorem* → "lesson on the sampling theorem"; slide heading *Abtastratengenerator* → "Sampling clock generator" (§8, AF620), caption *Taktgenerator* → clock generator; the `% TODO` comment and the commented-out picture line unchanged.
- fourier_transformation: *Fourier-Transformation* → Fourier transform, *Fast-Fourier-Transformation (FFT)* → "fast Fourier transform (FFT)", slide heading *Fast Fourier Transformation (FFT)* → "Fast Fourier transform (FFT)"; *Rechtecksignal* etc. → square-wave / sawtooth / triangular-wave / sine-wave signal, on the slides *Rechteck* etc. → square wave / sawtooth / triangular wave / sine wave (§3); *Oberwellen*, *ungeradzahlige Oberwellen* → harmonics, odd harmonics (unwanted multiples, no contrast with *Harmonische* here, so not *overtone*); *Gleichanteil* → DC component; *X-Achse* → X axis.
- digitale_filter: *Finite Impulse Response* / *Infinite Impulse Response* → lower case as expansions; *wie auch schon die Bezeichnung "finite" (zu Deutsch endlich) besagt* → 'as the name "finite" already says' (bracket rule); slide *"Finite" = …* → '"Finite": …'; *Mixed Signal Frontends* → mixed-signal front ends; *gleitender Mittelwert* → moving average; *Faltungsoperation* → convolution; the sequences `$0,0,0,4,0,0,0,0$` and `$0,0,0,1,1,1,1,0$` kept as written (the commas separate list items, they are not decimal commas).
- digital_iq: *Frequenzabweichungen* → "frequency offsets" (§14: not *deviation*); `\text{ bis }` → `\text{ to }` (running word); slide *$\num{10}$ Mio. Samples/s* → "$\num{10}$ million samples/s"; *ca.* → approx. (slide).
- latenz: *Pufferspeichern (englisch "buffer")* → "buffers", slide *Zwischenspeicherung (Buffer)* → "temporary storage (buffering)" — the first bracket only gives the English word (bracket rule), the second names the technique; *Laufzeit* → "propagation time", as AF637.
- Solutions: *Gegeben / Gesucht / Lösung* → Given / Required / Solution; *Wir setzen ein:* → "Substituting the values:"; heading *# Ausschlussverfahren* → "# By elimination" (as AA104); *Hilfsmitteln* → examination aids; *stufenweise analoges Signal* → "stepped analogue signal"; AF619 *Damit bleibt nur die Lösung … übrig* → "This leaves only the answer …"; the subscript `f_\text{abtast}` stays.

## Suspected errors in the German original

- solutions/AF622.md — "Es besagt, dass die höchste Signalfrequenz immer kleiner als die Abtastrate sein muss": the sampling theorem quoted one line above ($f_\text{abtast} > 2 \cdot f_{\mathrm{max}}$) and the last sentence of the solution require the highest signal frequency to be lower than *half* the sampling rate. Translated faithfully ("lower than the sampling rate").
- sections/anti_alias_rekonstruktionsfilter.md and slides — drawings 300 (`a_adc_4bit`) and 299 (`a_adc_12bit`), which sections/dac_adc.md captions as a sine wave digitised with 4 and with 12 bits, are captioned here "Signal vor / nach dem Rekonstruktionsfilter", and the text says "(vgl. Abbildung [ref:a_adc_12bit], das Rekonstruktionsfilter glättet das Signal)". The finer steps of the 12-bit signal come from the higher resolution, not from a reconstruction filter; a filtered 4-bit signal would look different. Kept.
- sections/fourier_transformation.md against sections/nicht_sinus_signale.md — here a sawtooth signal contains "sowohl die geradzahligen als auch die ungeradzahligen Vielfachen" ($f$, $2f$, $3f$ …), which is right; nicht_sinus_signale says "Sägezahnförmige Signale enthalten überwiegend gradzahlige Harmonische bzw. ungradzahlige Oberwellen" (mainly even harmonics), which contradicts it. Not changed here; noted for DARC.
- slides/fourier_transformation.md — "Jedes Signal lässt sich als Überlagerung von Sinusschwingungen darstellen", where the section, more carefully, says *periodische Signale*. Kept.
- Typos and slips with no effect on the English: sections/digitale_signalverarbeitung_einleitung.md "könnten man"; slides/digitale_signalverarbeitung_einleitung.md "Analog-Digital Umsetzers" and the double space in "steht dabei  für"; sections/abtasttheorem.md "nach dessen Entdeckern Nyquist und Shannon" (*deren*); slides/digitale_filter.md "Es werden nur eine begrenzte Anzahl"; solutions/AB404.md "ehält" (*enthält*); the picture ident `a_anit_alias` (*anti*) and drawing 1131 carrying two idents (`a_adc_dac_filter`, `a_adc_dac_filter_aa`) in slides/anti_alias_rekonstruktionsfilter.md (idents never change).
