# pitanja_09 — translation report

175 questions (frequency ranges BC1, IARU band plans BC2; call signs BD1,
call sign suffixes BD2, country prefixes BD3; operating procedure BE1,
signal reports BE2, contests, pile-ups, DXpeditions and ARDF BE3,
repeaters, beacons and satellites BE4; emergency communications BF1; log
and QSL cards BG1; the start of the regulations part: RR definitions and
Article 25 VA1–VA4, CEPT VB103–VB114), 875 fields; BE204–BE209 have
picture stems. `qbank-prevedi.py`: 0 refused, 0 warnings. 75 fields are
identical to the German (call signs, frequencies, reports, region numbers,
BE104's answers).

## Added to `TRANSLATION_GLOSSARY.md`

- §1.1: *Sendearten* → classes of emission, *Landeskennerliste der ITU*,
  *Gastlizenz*, *CEPT-Regelung* → CEPT arrangement, member countries /
  member states, implementing / participating countries,
  *Gegenseitigkeitsabkommen*, harmonisation, ETSI, ISO (*Organization*),
  *Not- und Katastrophenfunkübungen*, *Bodenkontrollstationen auf der Erde*
  → earth command stations, and the RR 1.56 / 25.2 phrasings used in VA104
  and VA302.
- §1.2: *Frequenzbereichszuweisungsplan* → Frequency Band Allocation Plan,
  *Angehörige der Gaststreitkräfte* → members of the visiting forces,
  *Fernmeldedienst* → telecommunications service.
- §1.3: *Kurzzeitzuteilung*, *Versuchsfunkstelle*, *exterritorial*,
  *Rufzeichennennung*, *Kennung*, *zwei- oder dreistelliges Suffix* →
  two- or three-letter suffix, *Kurzwellenhörer*, call sign suffixes in
  answers unchanged, *gemeldeter Standort*, *Landfahrzeug*,
  *Binnengewässer*, *See- und Binnenschifffahrtsfunk*, *angeordnete
  Logbuchführung*, *Zulassungsklasse N*.
- §2: band-plan words (*Bandanfang/-ende/-mitte*, *Europaverkehr*,
  *Nachbarort*, *Schmalband-FM*, narrowband digital modes), Morse speed
  (*Gebetempo*, *Einheitstempo*), *Fieldday-Contest*, *Standortkenner* →
  grid locator, RST words (*Kurzformel*, *Empfangsrapport*,
  *Zeigerausschlag*, *Tonhöhe* → pitch, *Signalqualität*), ARDF words,
  *begehrte / seltene Station*, *Sprint-Contest*, *Wertung*, repeater words
  (*Auftastton* → tone burst, *Tonruf*, *Sendezeitbegrenzer* → time-out
  timer, *Sprachspeicher*, *ordentliche Übergabe*, *hereinmelden*),
  International Beacon Project, standard-frequency and time-signal
  transmissions, emergency words (*Notfunkmeldung* → emergency message,
  *Hilfeleistungs- / Rettungsorganisation*, *Ersthelfer*, *Unfallstelle*,
  *Notzeichen*), log and QSL words (*Logbuch-Upload*, paper / computer
  log, logging software, *Funkwetter* → propagation conditions,
  *Amateurfunkrunde*), more country names. The *Fuchsjagd* row now allows
  "foxhunt" where the German quotes the colloquial word (BE313).
- §10: band names given beside VHF / UHF / HF / MF (BC101–BC106).

## Added to `DECISIONS.md`

Call sign suffixes in answers stay as the German writes them (BD208,
BD209); RR provisions in the RR's own English wording (VA102–VA303);
English band names beside the abbreviations, *Kurzwelle (KW)* dropped
beside *Short Wave (SW)* (BC101–BC106).

## Judgement calls

- BC101–BC106: "Ultrakurzwelle (UKW)" → "metre waves", "Dezimeterwelle" →
  "decimetre waves" (ITU-R V.431), "Short Wave (SW) oder Kurzwelle (KW)" →
  "short wave (SW)", "Mittelwelle (MW)" → "medium wave (MW)"
  (DECISIONS.md). The four answers stay the same set in every question.
- BC214, BC215, BC217–BC222: "Der IARU-Bandplan empfiehlt diesen Bereich für die Nutzung
  durch ..." → "recommends this range for ..." ("use by satellite
  communication" is not English); *Satellitenfunk* / *Weltraumkommunikation*
  → "satellite communication" / "space communication", kept apart as in
  German (BC219). BC215 *sieht … vor* → "designates".
- BC216, BE407: *Schmalband-FM (Narrow FM)* → "narrowband FM" (bracket
  rule). BC216 c *Kanalabstand* and d *Kanalraster* are both "channel
  spacing" (glossary; the German words are synonyms, the numbers differ).
- BD101, BD107, BD108: *Gaststreitkräfte* → "visiting forces", the English
  legal term for foreign forces stationed in a country.
- BD102 a, BD101 b: *§ 16 Absatz 2 AFuV* → "Section 16(2) AFuV".
- BD208, BD209: "/RB or /Remotebetrieb", "/FB or /Fernbedient", "/F or
  /Fern", "DL1PZ/Ausbildung" unchanged (DECISIONS.md).
- BD212: *der englischen Station G3MM* → "the English station G3MM" (G is
  England's prefix; not "British").
- BD303: *Tschechien* → "the Czech Republic" (the DXCC entity name).
- BD304: the German stem's first sentence asks which *prefixes* are
  assigned to the following *countries*, then gives prefixes and asks for
  countries; translated as it stands (slip noted below). The stray comma
  in "OE, PA, und SM" dropped.
- BE104 c: the German reply "EA6VQ, es ruft Sie DF1KW, bitte kommen." stays
  in German: the station called CQ in English, and the distractor is wrong
  because it answers in German. Translating it would make it a correct
  English reply.
- BE103 b, c: *Bitte QSL! / Bitte QSY!* → "QSL please!" / "QSY please!".
  d: "7R – Algeria" (7R is an Algerian prefix).
- BE111: *Standortkenner* → "grid locator", the English alternative name;
  "Felder (fields) und Quadrate (squares)" → "fields and squares".
- BE113 b, d: the brackets "(Data Link)" and "(Day Light)" stay: they show
  how the distractor reads the letters DL.
- BE115: Q code meanings in the ITU wording (QRZ? "Who is calling me?",
  QRV? "Are you ready?", QSL? "Can you acknowledge receipt?"); QTH? "What
  is your location?" (DECISIONS.md, batch 08).
- BE202: in German every answer spells R, S, T (*Rufzeichen*, *Standort*,
  *Trägerfrequenz* in the distractors). Written so that they still do:
  "R = radio call sign", "S = site", "T = transmit frequency" — otherwise
  only a would fit the letters (NE209 / EF212 reasoning). *Trägerfrequenz*
  → "transmit frequency" is the loosest of the three; "carrier frequency"
  would not start with T. The stem was turned into two sentences.
- BE203: *Tonqualität* → "tone" (the RST T), *Tonhöhe* → "pitch"; "in
  Stufen von 1-5" → "on a scale of 1 to 5".
- BE305: *"pile up"* → "pile-up". BE313: *"Fuchsjagd"* → "foxhunt", the
  colloquial word the question asks about (glossary note extended).
- BE410 d, BG110 c: *VO Funk* → "Radio Regulations (RR)" (glossary).
- BE415: the German glosses before the English expansions are dropped
  ("Satellit mit Amateurfunkstelle (Orbiting Satellite Carrying Amateur
  Radio)" → "Orbiting Satellite Carrying Amateur Radio"): they only
  translate the English (bracket rule). All four answers treated alike.
- BE416, BE412–BE414: *Erde* as the planet → "earth" (lower case, as in
  "back to earth").
- BF101, BF102: *Mayday* → "MAYDAY" (glossary); the made-up "Securité",
  "Distresse", "Prudence" kept as the German writes them.
- BF108: *Notfunkmeldung* → "emergency message"; *16. August* → "16
  August"; "(Ortsdatum)" → "(local date)".
- BG109 a: *weil dieser* → "because that station" (repeating the call sign
  K8PYD would add digits, which the tooling refuses).
- BG111 d: *SWL-Fachanwalt* → "SWL specialist lawyer" (a joke distractor in
  German too). c: *Intruder Monitoring* → "Intruder Watch".
- VA102, VA104, VA201, VA202, VA302, VA303: RR wording (DECISIONS.md).
  VA303 a: *Bodenkontrollstationen auf der Erde* → "earth command
  stations"; "on the earth" is part of the English term already.
- VA103 a: *wie der übrige Amateurfunkdienst* → "as the rest of the amateur
  service"; c *ionisierenden Regionen* → "ionising regions" (faithful; a
  nonsense distractor).
- VA406 b, d: the full glossary forms "Amateur Radio Act (Amateurfunkgesetz,
  AFuG)" / "Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)", because
  the German writes the full names; c "BNetzA", as the German. BE406 c
  likewise for *Amateurfunkverordnung*.
- VB106, VB107, VB113: German *er* recast ("provided the radio amateur has
  no permanent residence there", "the amateur radio rules of the home
  country must be followed"; VB113 answers as imperatives).
- BE109 a: *einige hundert Kilometer* is in words in German too, so "a few
  hundred kilometres" needs no exception.
- Suspected slips in the German, translated faithfully or noted: BC105,
  BC106 *zwischen 300 bis 3000* (mixes *zwischen … und* and *von … bis*);
  BC216 lower-case *ihr Funkgerät*; BC201 *zugute kommen* (old spelling);
  BD211 *Auzubildende*; BD304 stem reversed (prefixes / countries) and
  "PA, und"; BE105 capital *Allgemeinen Anruf*; BE313 d *SWL's*; BE402 d
  *höher die* (missing *als*); VA103 *nach den Begriffsbestimmung*; BF101
  *Securité* is a safety signal, not a distress signal (the distractor is
  wrong either way). Whitespace in the German, all dropped: double spaces
  in BC213, BE203, BE408, VA201 a, VB114; trailing spaces in BE103 b,
  BE313 d, VA101 a–d; trailing newlines in VA103 d; BE103 c '".';
  non-breaking spaces in BC213, BC216, BD101, BD102, BD104, BD106, BD107,
  BE104, BE111, BE114, BE303, BE306, BE402, BE403, BE407, BG104, VA103.

## Provjera

All 175 questions (875 text fields) checked German against English, all five
fields. 25 fields in 16 questions changed (`pitanja_09.provjera.json`,
applied with `--retranslate`: 0 refused, 0 warnings): 0 for meaning, 0 for
answer correctness, 12 for glossary / terminology, 13 for style. One
DECISIONS.md entry reworked, one reference corrected in DECISIONS.md and
glossary §2, one glossary row rewritten.

Changes:

- BC101–BC106, the VHF and UHF answers (12 fields): "Very High Frequency
  (VHF) or metre waves" → "Very High Frequency (VHF)", "Ultra High
  Frequency (UHF) or decimetre waves" → "Ultra High Frequency (UHF)". The
  questions ask which range a band or frequency span belongs to, not for
  the metric names; *UKW* and *Dezimeterwelle* are the German everyday
  names of VHF and UHF and only repeat them in English (UKW → VHF,
  TRANSLATION.md). "Short wave (SW)" and "medium wave (MW)" stay: they are
  everyday English names. answer_a stays the only range that fits in each
  question; the answer set is the same in all six, so the shorter VHF /
  UHF answers do not point to the correct one. DECISIONS.md entry and the
  glossary §10 row rewritten accordingly.
- BC101–BC103 Q: "What is the frequency range in which the 10 m band lies
  called?" → "What is the name of the frequency range in which …" (the
  verb no longer trails after the clause).
- BD104–BD106 Q: "Which category of call sign do call signs belong to that
  begin with …" → "To which category of call sign do call signs beginning
  with … belong?" (the split relative clause read badly).
- BD202 d: "… with a mailbox attached, in Canada." → "… in Canada with a
  mailbox attached." (word order).
- BD201 d: "is working with low power" → "is operating at low power".
- BE118 a: "no faster than I can also receive" → "no faster than I can
  receive myself" (*auch* here means "myself", not "also").
- BE109 a: "Only for stations …" → "Only to stations …" (answers "When
  should you reply?").
- BE307 d: "a list of the stations worked in the amateur radio magazines"
  read as stations worked in magazines; now "a list of the stations
  worked, in the amateur radio magazines".
- BE407 a: "the repeater being used could output the signal distorted" →
  "the repeater in use could put out a distorted signal".
- BF102 Q: "May you use SOS or MAYDAY …" → "Are you permitted to use SOS or
  MAYDAY …" (natural question form).
- DECISIONS.md (Q codes) and glossary §2 (*Bedeutungen der Q-Gruppen*):
  the Q code list was cited as "RR Appendix 14, Rec. ITU-R M.1172". RR
  Appendix 14 is the phonetic alphabet and figure code (the German course
  text itself says so, `buchstabiertafel.md`); the Q codes are Rec. ITU-R
  M.1172, which is incorporated by reference in the RR (ITU's own note on
  M.1172-0). Both now cite M.1172 and say what Appendix 14 is. This also
  backs VA407 a ("Radio Regulations (RR)"), which stays.

Points reviewed and kept:

- BD208, BD209: the German suffix strings stay. "/R or /Remote" and
  "DL1PZ/Trainee" are the actual suffixes and stay correct; "/RB or
  /Remotebetrieb", "/FB or /Fernbedient", "/F or /Fern", "DL1PZ/Ausbildung"
  are strings that would be transmitted and stay exactly as wrong as in
  German — the trap is still whether a German word may be used. English
  "/Training" or "/Remote operation" would invent strings DARC never set.
  The DECISIONS.md entry stands.
- BE202: the German distractors are German expansions that spell R, S, T;
  "radio call sign", "site", "transmit frequency" keep doing that (NE209 /
  EF212 rule). "Transmit frequency" for *Trägerfrequenz* loses "carrier",
  but "carrier frequency" would not spell T and would leave c the only
  distractor that does not fit the letters; the distractor is as wrong as
  in German. Kept.
- BE111: "grid locator" is an established English name of the Maidenhead
  locator and is the stem's third alias, as *Standortkenner* is in German;
  answer a ("fields and squares", the Maidenhead terms) is correct. Kept.
- BE104 c: must stay German. EA6VQ called in English; c is wrong in German
  because it answers in German. Translated, it would be a second correct
  English reply. Kept.
- VA303 a: "earth command stations" is the RR 25.2A term ("control signals
  exchanged between earth command stations and space stations in the
  amateur-satellite service"); "auf der Erde" is contained in it. Correct.
- DECISIONS.md "RR provisions in the RR's own English wording": checked the
  quoted wording against RR 1.56, 1.61, 1.96, 25.2 and 25.2A; correct, and
  VA104 d being the older RR 25.2 wording does not make it right (the
  question asks about the definition in RR 1.56). Kept unchanged.
- BC216 c/d "channel spacing" for both *Kanalabstand* and *Kanalraster*,
  BE415 glosses dropped, BC213 a "preferably", BF107 "exemplary": kept.
