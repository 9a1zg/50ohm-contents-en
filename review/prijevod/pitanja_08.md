# pitanja_08 — translation report

175 questions (other instruments AI601–AI605, NI401; interference to
electronic equipment AJ1, EJ1, NJ1; unwanted emissions AJ2, EJ2, NJ2;
immunity NK1; protection of persons AK1, EK1, NK201; safety AK2, EK2, NK3;
the start of the operating part: international phonetic alphabet BA1,
operating abbreviations BB1, Q codes BB2), 847 fields (AJ118, AJ208, AJ221,
EJ117, EJ206–EJ208 have picture answers, so only their stems are text).
`qbank-prevedi.py`: 0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §1.2: *Prüf- und Messdienst* (BNetzA), *Hauptzollamt* → main customs
  office, *Kraftfahrt-Bundesamt* → Federal Motor Transport Authority,
  *RTA* / *EMV-Beauftragter des RTA*, *Anhang* of the 26. BImSchV → Annex.
- §1.4: *Schutzabstand*, *Grenzwert im Fall des Personenschutzes /
  Personenschutzgrenzwerte*, *nicht kontrollierbarer Bereich*, *kritischer
  Winkel*, *Fernfeldnäherung / Näherungsformel für die Fernfeldberechnung*,
  *quadratisch gemittelt über 6 Minuten* → RMS value averaged over
  6 minutes, *kurzfristiger Effektivwert / momentaner Spitzenwert*,
  *spezifische Absorptionsrate*, the form *Anzeige ortsfester
  Amateurfunkanlagen*.
- §2: *Durchgang* → over, *aufnehmen* → receive, *formlose Übergabe*,
  *Bestätigungskarte*; Q code meanings (ITU wording); words of other
  spelling alphabets.
- §3: *Wellenwiderstand* of a medium → wave impedance.
- §11: *HF-Tastkopf / Gleichspannungstastkopf*, *Spitzenwertgleichrichter*,
  *Messausgang*, *Dauerleistung*.
- §12: *Mantelwellendrossel* → common-mode choke, *Einfügedämpfung*,
  *Vorstufe* (TV), *Antennenzuführungskabel*, *Leitungsanschlüsse*,
  *hochpermeable Ferritdrossel*, *Klappferritkern* → clip-on ferrite core,
  *Kollektormotor* → commutator motor, *Bimetall-Temperaturregler*,
  *Musik-/Stereoanlage*, *Pfeifstellen*, *Nebenresonanzen*,
  *Schirmungsmaß*, *Phantomsignale*, *parametrische Schwingungen*,
  *Reihenhaus / Häuserzeile / Einfamilienhaus*, *Dachrinne*, *D-Netz*,
  *Betriebsfunk* → private mobile radio, *Fernsehtechniker des
  Fachhandwerks*, *Standrohr* → mast, *Erdungsanlage*, *Blitzschutz-
  Fachkraft*, *Adernkennfarben / grüngelb*, *Ladedrossel* → storage choke,
  fuse characteristics *Flink / Mittelträge / Träge* → fast-acting /
  medium time-lag / time-lag (IEC 60127), *Körperdurchströmung*,
  *Störlichtbogen* → arc fault, medical terms (*Herzkammerflimmern*,
  *stabile Seitenlage*, *Verätzungen*, *Verbrühungen*), vehicle terms
  (*Zulassung* of a vehicle → road approval, *Kabelbaum*, *Kotflügel* →
  wing …).

## Added to `DECISIONS.md`

Q code meanings in the ITU's English wording; spelling-alphabet distractor
words kept as the German writes them (except *Amerika*); a bracket that only
repeats the term in the other language is dropped (dummy load, BB110).

## Judgement calls

- BB201–BB204: Q codes in the ITU wording (DECISIONS.md). BB201 b *Ich habe
  Störungen* → "I have interference", kept apart from QRM "I am being
  interfered with"; *Sie haben Schwankungen Ihrer Zeichen* → "Your signals
  are fluctuating", kept apart from QSB "Your signals are fading" (d).
  BB202 *Haben Sie noch etwas für mich vorliegen?* → "Have you anything more
  for me?"; *die / meine Sendeleistung* kept apart ("transmitter power" /
  "my transmitter power").
- BB203 a, c, d: the German "bestätigen??" (double question mark) is a slip;
  one "?" in English.
- BA101–BA110: answers unchanged except *Amerika* → "America" (BA106);
  *Nordpol*, *Ypsilon*, *Caesar*, *Vulcano* kept (DECISIONS.md).
- BB110: "Received (empfangen)" etc. → "Received", "Repeat", "Report",
  "Readability" — the German glosses only translate the English words;
  *Rapport (Bericht)* → "Report".
- BB107 d *Contestwertung* → "Contest Weighting", so that it still spells
  CW like the other three distractors (NE209 / EF212 reasoning); "scoring"
  would not.
- BB105: answer a repeats *Stationen* after the stem's "Nur Stationen ...";
  dropped in English ("on other continents").
- BB104 a *in mehr als einigen 100 km Entfernung* → "more than a few 100 km
  away": "a few hundred km" is the natural English, but the tooling keeps
  the digits.
- BB103 c, d: German *indirektem / direktem* (case slip) — "By the indirect
  / direct path".
- AJ203: *dritte Oberwelle* → "third overtone (Oberwelle)" as AB402: the
  correct answer is 28.80 MHz = 4 × 7.20 MHz, and b (21.60 MHz) is the third
  harmonic. AJ202 *dritte Harmonische* → "third harmonic".
- AJ204 b *D-Netz-Mobilfunkbereich* → "D-network (GSM) mobile phone band":
  an English reader does not know the German D-network; "900" could not be
  added (tooling). c *UKW-Betriebsfunk-Bereich* → "VHF private mobile radio
  band".
- EJ118: *Mantelwellendrossel* → "choke balun" in the stem, because the
  correct answer is *Gleichtakt-HF-Störsignale* → "common-mode RF
  interference signals"; "common-mode choke" would hand it over (DECISIONS.md
  "no echo"). Elsewhere (AJ115, EJ119) "common-mode choke".
- EJ202: stem "harmonics" and answer a "harmonic filter" echo, where the
  German has *Harmonische* / *Oberwellenfilter*; no other accurate English
  term (and the two German words are synonyms anyway). The article moved
  from the stem into the answers ("an IF filter").
- EJ123: in German, answer a is a finite clause (*schlagen Sie … vor*) and
  b–d infinitives (*zu verwenden*), so a stands out by grammar; in English
  all four are imperatives.
- EJ103 a *Übersteuerung oder störende Beeinflussung* → "overloading or
  interference" (*störende Beeinflussung* → interference, glossary).
- EJ105 b *nur mit effektiver Leistung* → "only with RMS power" (glossary
  *effektive Leistung*); a nonsense distractor in German too.
- AJ105 c *Direktmischung* → "direct conversion" (the established term,
  *Direktmischer* → direct-conversion receiver).
- AJ119 *zum Abblocken von HF-Spannungen* → "for RF decoupling".
- AJ116 d: "the RTA's EMC officer", RTA left unexplained as in German.
- AK115: *äquivalente Strahlungsleistung (ERP)* → "effective radiated power
  (ERP)" (DECISIONS.md, EIRP entry; the abbreviation decides, and the
  result 0.7 V/m is the ERP with 1.64).
- AK103: the formula's `30 Ohm` stays (formulas unchanged); it is German
  inside maths.
- AK104 a: "Dämpfungsfaktor$ D$" → "attenuation factor $D$" (space moved
  outside the maths, same formula). AK110 "$11,5 $dBd" →
  "$11.5$ dBd", EK108 "$7,5 $dBd" → "$7.5$ dBd" likewise.
- AK110: *die Modulationsverfahren FM* (plural article, slip) → "FM as the
  modulation method"; AK106, AK108–AK112, EK108 recast "for the … band and
  the modulation method FM / transmission method RTTY" as "with FM as the
  modulation method" / "with RTTY as the transmission method"; AK107 "in
  FM".
- AK203 a: the German line break inside the sentence dropped.
- EK102: *quadratisch gemittelt* → "RMS value averaged over 6 minutes",
  *kurzfristiger Effektivwert* → "short-term RMS value": both RMS, as the
  German concepts are; EK103 the same.
- EK104: *nachweisen* → "demonstrate" (compliance); *er* recast as "the
  radio amateur" (DECISIONS.md, batch 07).
- EK105: range "3,5 - 3,8 MHz" → en dash; d *"Anzeige ortsfester
  Amateurfunkanlagen" gemäß § 9 BEMFV* → the "Notification of fixed amateur
  radio installations" under Section 9 BEMFV.
- EK204: fuse marked 20 A *"Flink"* → "fast-acting", *Mittelträge / Träge*
  → "medium time-lag" / "time-lag" (IEC 60127 names).
- EK205: imperative "!" → full stop; *grüngelb* → "green-yellow".
- EK210 c, d: *Ein- oder mehrdrähtiger – aber nicht feindrähtiger –* →
  "Solid or stranded – but not fine-stranded –".
- EK211, EK210: *Standrohr* → "mast".
- NK308: *Zulassung eines Kraftfahrzeugs* → "road approval of a motor
  vehicle", so it is not read as the amateur licence; *grundsätzlich* →
  "always" in each answer.
- NK303 d *Verkochungen* (a made-up word) → "Internal boiling".
- NK310 c *Kotflügel* → "front wing" (British).
- NJ102 b, c, NK201 b, c, EJ122, AJ116: German *er* / *sein* for the
  neighbour or the radio amateur recast ("The neighbour should be told …",
  "So that the transmitter can be …") or singular *their*.
- NJ102 d *das örtlich zuständige Hauptzollamt* → "the locally competent
  main customs office".
- EJ212: *AFSK-Signal (Niederfrequenzumtastung)* → "AFSK signal (audio
  frequency-shift keying)".
- EJ201: answers lower case in German; capitalised.
- AK201 b, AI601, AI603: *Ohm* → Ω.
- AK204 b: *100 Watt / 50 Watt* → "100 W / 50 W" (units after a number).
- Suspected slips in the German, translated faithfully or noted: AJ208
  *ünterdrückt*; EJ120 a *Phantomsignale … verschwindet* (singular verb);
  EJ122 lower-case *ihre* for *Ihre*; BB203 "??"; BB105 doubled
  *Stationen*; BB103 *indirektem / direktem*; AK110 plural
  *Modulationsverfahren*. Whitespace in the German, all dropped: leading
  spaces in EJ121 a–c; trailing spaces in AI605 Q, AJ209 Q, EJ108 a,
  AK102 a, BB106 a, BB103 a, b; double spaces in BA101–BA110; non-breaking
  spaces in EJ212 Q and BB108 c, d.

## Provjera

All 175 questions (847 text fields) checked German against English, all five
fields. 7 fields in 5 questions changed (`pitanja_08.provjera.json`,
applied with `--retranslate`: 0 refused): 0 for meaning, 0 for answer
correctness, 7 for style; no question text changed for the glossary. Four
documentation corrections (DECISIONS.md, glossary).

Changes:

- BB104 a: "a few 100 km" → "a few hundred km", with `"iznimke"` in the
  provjera file (the tool now allows it; same value, natural English).
- AJ118 Q: "inserted at a mains lead" → "inserted in a mains lead".
- AJ219 a, c, d: "…, which as unwanted emissions cause …" → "…; as unwanted
  emissions, they cause …" (the embedded phrase read awkwardly).
- EJ213 b: "distortion at reception" → "distortion on reception".
- EK105 d: "submitted before putting into service" (no object) → "before
  the installation is put into service".

Documentation:

- Q codes checked one by one against the text of Rec. ITU-R M.1172: QRV,
  QRN/QRN?, QSB/QSB?, QRT, QRZ?, QSL?, QRO?, QRP?, QSO? (the German omits
  "or by relay", so does the English), QRX?, QRU/QRU?, QSV are the ITU
  wording. QRM is not: M.1172 has "Is my transmission being interfered
  with? / Your transmission is being interfered with". The German *Werden
  Sie gestört? / Ich werde gestört* follows the older wording, "Are you
  being interfered with? / I am being interfered with", which the English
  keeps, because it is what the German says and the distractors in
  BB201/BB204 are built on it. DECISIONS.md and glossary §2 no longer
  present it as the ITU wording; QTH ("location", ITU "position") is now
  also named as an exception.
- DECISIONS.md, brackets entry: EH202 has no dummy load. Its examples are
  *Rückstreuung (Backscatter)* → "Backscatter", and it also keeps a bracket
  that adds information ("(fading)"); the dummy-load examples are AI601–AI603
  and NJ202. Now cited correctly.
- DECISIONS.md, spelling-alphabet entry: many of the distractor words are
  place names (Guatemala, Honolulu, Oslo), not words of another alphabet;
  the reason is reworded. The decision itself stands.
- AK115: "effective radiated power (ERP)" is consistent with the EIRP/ERP
  entry (the abbreviation decides; 7·√100/100 = 0.7 V/m is the ERP formula).
  The glossary's ERP row had no form for plain *äquivalente
  Strahlungsleistung (ERP)*, so it was added there and in the DECISIONS.md
  entry.

Points reviewed and kept:

- EJ118 "choke balun": an established English name for a common-mode choke
  on coax. It no more gives away "common-mode" than the German
  *Mantelwellendrossel* gives away *Gleichtakt*. Kept, as DECISIONS.md "no
  echo" says.
- AJ203 "third overtone (Oberwelle)": as AB402 and DECISIONS.md;
  28.80 MHz = 4 × 7.20 MHz, and b is the third harmonic. Correct.
- BB107 d "Contest Weighting": *Wertung* is scoring rather than weighting,
  but a faithful "scoring" would no longer spell CW like the other
  distractors (Code Word, Calling Wide). Kept, following NE209/EF212.
- EJ123: in German, b–d are bare *zu*-infinitives that do not complete the
  stem grammatically, so a stands out by form only. English cannot copy that
  without writing ungrammatical answers. The four imperatives keep the
  German's content balance: only a involves the neighbour, b–d are
  technical measures. Kept parallel; the German grammar is a slip to note
  for DARC.
- AK115, NK308 "road approval", EJ103 "overloading or interference"
  (glossary *störende Beeinflussung*): kept.
