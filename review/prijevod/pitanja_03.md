# pitanja_03 — translation report

175 questions (ED1, AD2, ED2, AD3, ED3, ND1, AD4, ED4, AD5, AD6, ED507),
831 fields. `qbank-prevedi.py`: 0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §4: *Einzelbelastbarkeit* → individual power rating; *Strombelastbarkeit*
  → current rating; *Aluminium- / Tantal-Elektrolytkondensator*.
- §5: *Teilspannung* → partial voltage; *Übertragungskurve* → response curve;
  *Impedanzfrequenzgang* → impedance-versus-frequency response;
  *Höcker- / Sattelspannung* → peak / dip voltage; *Wechselstromkopplung /
  Gleichspannungsentkopplung* → AC coupling / DC blocking;
  *Spannungskonstanz* → voltage stability; *Brummfrequenz* → hum frequency;
  *Überspannungsableiter* → surge arrester; *Phasenumkehrstufe* → phase
  inverter stage; *ungedämpfte Schwingungen* → sustained (undamped)
  oscillations; *Schleifenverstärkung* → loop gain; *Audion(schaltung)* →
  regenerative detector (audion); *Tongenerator*; *Abwärtsmischer* →
  down-converter.
- §6: *Flankendemodulator / Flanken-Diskriminator* → slope detector.
- §12: *Schutzkontakt* → earthing contact; *Kurzschlussstrombegrenzung /
  thermische Abschaltung*; *Bürstenmotor* → brush motor.
- §13: *zweipolig* (supply lead) → two-conductor; *Mobilfunktransceiver* →
  mobile transceiver; *Masseleitung* → chassis lead.

## Judgement calls

- Units after a number are always symbols, per the new rule in
  `TRANSLATION.md`: *Ohm / kOhm / MOhm* → Ω / kΩ / MΩ throughout (ED1xx,
  AD2xx, AD321). AD203's `\kiloOhm` macro left as it is. "nahezu null Volt"
  (AD317) and "null Ampere" (AD418) have no numeral → "zero volts" /
  "Zero amperes".
- ED104: the German writes `$R_1 = 100 Ohm$` with the unit inside the
  formula; rendered `$R_1$ = 100 Ω` like its twin ED105, so the unit is not
  set as italic variables. Same $ count, no command changed.
- ED101: German "$R_1$ = 5-mal so groß ist wie $R_2$" (stray "=") →
  "$R_1$ is 5 times as large as $R_2$".
- *ca.* / *Zirka* → "Approx." (AD203, AD302, ND102, AD317, AD421…);
  *etwa* → "About" (AD219, AD306, AD418); each set consistent.
- AD322: "Bias-T (Fernspeiseweiche)" → "bias tee (remote DC feed)", giving a
  gloss for the German synonym rather than dropping it.
- AD217–AD213: *Spule zusammenschieben / auseinanderziehen* → "Push the turns
  of the coil closer together" / "Pull the turns of the coil apart";
  *verringern / vergrößern* the resonant frequency → "lower" / "raise".
- ED215/ED214 etc.: *Saugkreis / Sperrkreis* → "Acceptor circuit" /
  "Rejector circuit" (RSGB terms, glossary).
- AD422, AD416, AD419–AD425: *A-/AB-/B-/C-Betrieb* → "class A … operation";
  AD416 keeps the drawing label `\text{AP}` (operating point) untranslated.
- AD617: stem "… crystal oscillator in ..." completed by "common-collector
  configuration. …" / "common-emitter configuration. …".
- AD507, AD506, AD505, AD504, AD501, AD409, AD401: German has the article in
  the stem ("um einen ..."); English stem "This circuit is ..." with a/an in
  each answer.
- AD504 a *Flanken-Diskriminator* → "slope detector" (glossary), while AD506 d
  bare *Diskriminator* stays "discriminator".
- AD503: *Regelspannung* at an envelope detector → "AGC voltage" (glossary).
- AD509: *FM-Funkgeräte* → "FM transceivers" (not "FM radios", which reads as
  broadcast receivers).
- AD612: *Rückwirkungen … zu verhindern* → "to prevent the following RF power
  amplifier stages from acting back on it".
- AD620: the German's English expansions misspell "Oszillator"; written
  correctly, lower case as in the glossary.
- AD607: *Teflon* and *Pertinax* kept as the German names them.
- ED302: *Volumen* → "volume" (small / large volume), parallel to weight.
- ND105: *grüngelb* → "green-yellow".
- Suspected slips in the German, translated normally: AD321 stem ends with
  "." instead of "?" ("?" in English); AD506 a "zu Demodulation"; AD316 b,
  AD312 b, AD410 b lack a final full stop (added for parallelism); trailing
  spaces / newline in ED122, ED113, AD318 c, AD303 a/b, ND104 c, AD607 c,
  AD617, AD614 dropped; ND106 has a double space.

## Provjera

175 questions checked (all five fields, German from `upstream/main` side by
side with the English); 17 fields changed in 8 questions: 1 meaning,
1 answer plausibility, 15 wording / style (10 of them stem/answer grammar).
No glossary changes: the 24 new rows were checked and are right. Applied
from `pitanja_03.provjera.json` with `--retranslate`: 0 refused, 0 warnings.

The translator's judgement calls stand: ED104 (`$R_1$ = 100 Ω`, as ED105),
ED101 (stray "=" dropped), AD322 (gloss "remote DC feed" for
*Fernspeiseweiche*, no more of a hint than the German word), AD504 / AD506
(*Flanken-Diskriminator* / *Flankendemodulator* → slope detector, bare
*Diskriminator* → discriminator; the AD506 answer set stays four distinct
answers), AD612 (reworded below).

- AD601, AD602 (all five fields): the stems "A VCO is a ..." / "A TCXO is
  a ..." gave "a oscillator ..." with answer d / b; the article moves into
  each answer ("a voltage-controlled oscillator.", "an oscillator that
  is ...").
- AD204: "the impedance curve shown next to the circuit" → "shown next to
  it" (*neben der jeweiligen Schaltung*: each answer pairs a circuit with its
  own curve).
- AD414: "How does the voltage gain … change" → "How is the voltage gain …
  affected"; the German asks *wie verhält sich*, and "change" presupposed
  that answer b ("It remains constant") is wrong.
- AD612 stem: "to prevent the following RF power amplifier stages from
  acting back on it" → "to prevent it from being affected by the following
  RF power amplifier stages" (natural English for *Rückwirkungen*).
- AD612 d: "The RF superimposed on the VFO supply" → "The RF components
  superimposed …" (missing noun); "filtered out" → "filtered", as the German.
- AD203: "Where does the cut-off frequency … lie" → "What is the cut-off
  frequency …" (German *wo liegt*, not English idiom).
- AD313: "Unwanted signals are observed in an amateur radio receiver about
  every 120 kHz" → "In an amateur radio receiver, unwanted signals are found
  at intervals of about 120 kHz".
- ND104 b: "from both poles of the power supply unit" → "from both
  terminals" (*Pol* → terminal, as *Pluspol* → positive terminal).
