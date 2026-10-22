# pitanja_07 — translation report

175 questions (NG301–NG303; EIRP and ERP AG501–AG503, EG501–EG511,
NG401–NG402; the ionosphere AH1, EH1, NH1; HF propagation AH2, EH2, NH201;
propagation above 30 MHz AH3, EH3, NH3; ammeters and voltmeters AI1, EI1,
NI1; VNA AI2, EI2; oscilloscope AI3, EI3; SWR meter AI4, EI4, NI2;
frequency measurement AI5, EI5, NI301; other instruments AI606–AI615),
863 fields (EI102, NI103, NI104 have picture answers, so only their stems
are text). `qbank-prevedi.py`: 0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §2: *Fonie* → voice.
- §9: notes on the EIRP / ERP rows (the German's shortened *äquivalente
  Strahlungsleistung (EIRP)* and *gleichwertige …*; AG501's "equivalent
  (effective) radiated power"); *bezogen auf den Halbwellendipol* →
  "relative to the half-wave dipole", *in einer Richtung* → "in a given
  direction" (RR); *Antennenspeiseleitung* → antenna feeder.
- §10: *Sprungentfernung* (with *Sprungdistanz*) → skip distance;
  *Funkstrecke* → radio path; *Weitverkehrs- / Überseeverbindungen*;
  *Beamrichtung* → beam heading; *höchste brauchbare / nutzbare Frequenz*;
  *höchste durchlässige Frequenz* (distractor); *Abdeckung* → blanketing;
  *Tagesdämpfung*; *Sonnenfleckenmaximum / -minimum*; *Röntgenstrahlung*;
  *Sonneneruption* → solar flare; *Rückstreuung / Backscatter*;
  *Regenscatter*; *Ionisationsspuren von Meteoriten / Meteorbahnen*;
  *leuchtende Nachtwolken* → noctilucent clouds; *Geländeprofil*;
  *quasi-optische Sichtweite*; *Aurora-Erscheinungen / Polarlichter /
  Nordlichter*; *Aurora-Verbindung*; *verbrummt*; *Polarkreis* → Arctic
  Circle; note on *Überreichweiten* (AH304).
- §11: about 30 instrument terms — *Vielfachinstrument / Universalmessgerät*,
  *Gleich- / Wechselspannungsmessgerät*, *Widerstandsmessgerät*,
  *Wechselstromzähler*, *Transistorvoltmeter / True RMS-Voltmeter*,
  *Oszillograf / Speicheroszilloskop*, *Diodentastkopf*,
  *Triggereinrichtung / Triggerschwelle*, *X-/Y-Vorteiler*,
  *Frequenzmarken-Generator*, *Hüllkurvenform*, *Frequenzmessgerät /
  Frequenzmesser* → frequency meter, *Hauptoszillator* (counter) →
  timebase oscillator, *Anzeigegenauigkeit*, *Frequenzgenerator*,
  *Absorptions- / Resonanzwellenmesser*, *SWR-Messbrücke* → SWR bridge,
  *Absolutleistungsmesser*, *Impedanzmessgerät*, *Antennenimpedanzmesser*,
  *Resonanzmessgerät*, *Peilsender*, *Messkopf zur HF-Leistungsmessung*,
  *Breitbandpegelmesser*, *Anpassungsübertrager*, *Messanschluss* (VNA) →
  test port, *Kalibrierung / Nullpunktabgleich*, the VNA short / open /
  matched conditions, *Abschlusswiderstand* (VNA), *Resonanzverlauf*,
  *Frequenzreinheit* → spectral purity, *Erdungswiderstand*,
  *Bakensegment*, *erdnahes Ende* → earthed end, *effektive Leistung* →
  RMS power.

## Added to `DECISIONS.md`

Word subscripts in formulas (`P_{\textrm{Sender}}`) stay German; the
German's shortened "äquivalente Strahlungsleistung (EIRP)" is written as the
full English term; the generic *er* for a radio amateur is recast without a
pronoun or as singular *they*.

## Judgement calls

- AG502, EG502: `P_{\textrm{Sender}}`, `P_{\textrm{Verluste}}`,
  `G_{\textrm{Antenne}}` kept German (see DECISIONS.md); only the prose
  after the formula is translated.
- EG503–EG505: *äquivalente Strahlungsleistung (EIRP)* → "equivalent
  isotropically radiated power (EIRP)"; NG402 drops the German's bracketed
  English expansion, which in English would only repeat itself.
- EG511: *§ 9 BEMFV* → "Section 9 BEMFV" (glossary: § → Section in prose).
- AG501 c, d: worded after RR 1.157 / 1.158 (PEP, mean power), which the
  German paraphrases. EG501 c, d are garbled in German ("average power … and
  its gain") and stay so.
- EH204: *Höchste nutzbare Frequenz* → "Maximum usable frequency", which
  spells MUF; d *Mittlere Nutzfrequenz* → "Mean usable frequency" spells it
  too, so a is not alone (same reasoning as EF212 in DECISIONS.md).
- AH207: *höchste brauchbare Frequenz* → "the highest usable frequency",
  parallel to c "the lowest usable frequency"; AH211 likewise.
- AH206: a "maximum usable frequency (MUF)", d *höchste durchlässige
  Frequenz (LUF)* → "maximum penetration frequency (LUF)", so that a and d
  are built alike, as in German, and neither echoes the stem's "highest"
  alone.
- EH203: stem *Feldstärkeschwund* → "drop in field strength", so it does not
  echo the answer "Fading"; the German stem does not either.
- EH202 c, d: *Rückstreuung (Backscatter)*, *Rauschen (Noise)* → "Backscatter",
  "Noise" — the brackets only give the English word; a and b keep their
  brackets, which add information.
- AH221: stem reordered ("In the ionosphere, … mainly affects ...") so that
  each answer continues it.
- AH216 d is a fragment in German; kept as "From the reverberant sound of
  the contact with Brazil: the radio waves propagated via two opposite
  paths."
- AH216, AH217, AH218, EH217, AH305: the German *er* recast without a
  pronoun, or singular *they* (DECISIONS.md).
- AH217, AH218: *Frankfurt/Main* → Frankfurt am Main; *Tokio* → Tokyo.
- AH101: the German dashes "- je nach Strahlungsintensität -" moved to the
  end of each answer: "…, depending on the intensity of the radiation."
- AH222: answers recast as verbs ("The two signals interfere with each
  other." / "… are reflected." / "The frequency of both signals changes." /
  "Both signals are diffracted."), parallel as in German.
- AH223, EI502, EI503: German answers begin lower case; capitalised.
- AH308 a *flatternden und verbrummten Ton* → "fluttering, buzzing tone"
  (aurora CW); AH220 b *stark verbrummt* → "with heavy hum"; AH305 d
  *verbrummten Ultrakurzwellen* → "hum-modulated VHF waves".
- AH311: *Überreichweiten* → "enhanced propagation"; AH304 → "considerably
  extended ranges".
- AH301 d, EH304 c: *Meteoriten / Meteorbahnen* → "meteors" / "meteor
  trails" (what leaves an ionisation trail is a meteor).
- EH105 d: *Lang-, Mittel- und unteren Kurzwellenbereich* → "long-wave,
  medium-wave and lower short-wave ranges"; elsewhere *Kurzwelle* → HF.
- EH207: *aktuell höchstmöglichen Frequenz (MUF)* → "highest frequency
  currently possible (MUF)", as the German, not the textbook expansion.
- NH305: *Kilometer* → "km" (units after a number as symbols).
- AI509: ranges "… MHz - … MHz" → en dash.
- AI103: the German verb in each answer (*bestimmen*) moves to the stem
  ("… would be determined ..." / "9.75 % too low.").
- AI203, EI501: the article moves from the stem into the answers ("an
  ohmmeter").
- AI105: *effektive Leistung* → "RMS power".
- AI302 b, c: *X-/Y-Vorteiler* → "X/Y prescaler" (glossary *Vorteiler*);
  distractors.
- AI504 a: *Hauptoszillator* of a counter → "timebase oscillator".
- AI608 d: *HF-Dipmeter* → "RF dip oscillator".
- AI609: answers given articles ("A 20 dB, 20 W attenuator", "A 25 m length
  of RG213 (MIL) coaxial cable", …).
- AI606: *erdnahen Ende* → "earthed end".
- AI204, AI206: the German alternates *ohmsche Anteil* / *ohmsche
  Widerstand* between the two capacitive/inductive answers; kept as
  "resistive part" / "ohmic resistance".
- EI101: *hochohmig / niederohmig* of a voltmeter → "a high / low
  resistance".
- EI206 a: *in den Betriebszuständen Kurzschluss, Leerlauf und Anpassung* →
  "in the short-circuit, open-circuit and matched conditions".
- EI404 c: the German repeats *Zwischen* after the stem's *zwischen*;
  dropped.
- Suspected slips in the German, translated faithfully: AH103 b "9 bis 130
  km" (probably 90; kept "9 to 130 km", the tooling keeps numbers);
  AI510 *Ein Transceivers*; AI511 d *temperaturstabiliserten*; AI202 a
  *Netzwerk Analysator*; AH205 c and AI207 d lack a full stop (added);
  AH302 c alone has a full stop (dropped, as a, b, d). Whitespace in the
  German, all dropped: final newline in AH206 b; leading space in AH203 d;
  trailing spaces in AI401 a and in the questions EI103, NI104, AI208,
  AI207, EI405, NI301, AI613, AI608, EI302; double space in AI201 d.
