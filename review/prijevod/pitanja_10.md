# pitanja_10 — translation report

175 questions, the rest of the regulations part: CEPT VB101–VB102; the
Amateur Radio Act VC1; the Amateur Radio Ordinance — general VD1, call signs
VD2, training operation VD3, club stations VD4, repeaters and beacons VD5,
remote stations VD6, frequency ranges and usage parameters VD7; other laws —
TKG VE1, TTDSG VE2, EMVG and interference cases VE3, FuAG VE4, EMVU / BEMFV
VE5, safety regulations VE6, miscellaneous VE7. 875 fields.
`qbank-prevedi.py`: 0 refused, 3 warnings (German in brackets on purpose:
VC104 c, d and VE501 a). 33 fields are identical to the German (power
figures in VD503, VD724, VD728–VD736, VD743).

## Added to `TRANSLATION_GLOSSARY.md`

- §1.1: *Weltraumfunkstelle* → space station, *Sicherheitsfunkdienst* →
  safety service (RR 1.64, 1.59), *EMV-Richtlinie* → EMC Directive.
- §1.2: *Bundes-Immissionsschutzgesetz (BImSchG)* → Federal Immission
  Control Act; *Verordnung zum Gesetz über den Amateurfunk* (the AFuV's
  formal title); *Gesetz über Funkanlagen (FuAG)* (not the real title);
  *Frequenzverordnung (FreqV)*, *Frequenzplan (FreqP)* → Frequency Plan
  (capitalised, also in the AFuG definitions), *Frequenznutzungsplan*,
  *Frequenznutzungsplanaufstellungsverordnung*; *Bundesgesetzblatt*;
  *Physikalisch-Technische Bundesanstalt*, *Bundesanstalt für Post und
  Telekommunikation*, BDBOS, *Bundesamt für Seeschifffahrt und
  Hydrographie* (official English names where they exist);
  *Bauaufsichtsbehörde*, *eingetragener Verein*, *Führungszeugnis*,
  *Volljährigkeit*, sanctions and proceedings (*Beschlagnahmung*,
  *Entzug / Einzug*, *Unbrauchbarmachen*, *Betriebsverbot*,
  *Bußgeld- / Ordnungswidrigkeitenverfahren*, *behördliche
  Abhilfemaßnahmen*), *sachkundige Person*, insurance terms. The EMVG and
  FuAG rows say which form exam questions use (DECISIONS.md).
- §1.3: *Rufzeicheninhaber / Funkamateure der Klasse A*,
  *Hörerrufzeichen ("DE-Reihe")*, the made-up call sign categories of
  VD202, *Zuteilungsurkunde* → assignment document, *Schulstation*,
  *mitbenutzen*, *Betriebssicherheit*, *Bandwacht* → Intruder Watch,
  *Relaisnutzungsgebühr*, *Flug-/Seefunkzeugnis*, *Notfunkübung*, the AFuV
  definition words (*Feldstärkebeobachtung*, *Empfangsversuche*,
  *fernausgelöst*), contributions, *Verträglichkeits- / EMVU-Bescheinigung*,
  *baumustergeprüft*, *Elektromeister / Abnahmeprotokoll*.
- §1.4: *Nachweis zur Begrenzung elektromagnetischer Felder*,
  *Anzeigeformblatt*, *zeichnerische Darstellung*, *Messlabor*,
  *Sendeumschalter*; the EMVU row notes VE501.
- §12: *Kabelverteilanlage*. §1.1 *verschlüsseln*: encrypt in German law.
- §13: *kostenpflichtige Nachprüfung* changed from "inspection subject to a
  fee" (unused so far) to "re-examination subject to a fee", *fachliche
  Nachprüfung* → re-examination of competence.

## Added to `DECISIONS.md`

German statute names in exam questions (English name + German short title +
abbreviation; long formal titles with the abbreviation only; VC101 bare);
*verschlüsseln* → encrypt in German law, encoded in the RR; answers to "What
does the German abbreviation X stand for?" carry the German expansion in
brackets (VE501); *Nachprüfung* → re-examination.

## Judgement calls

- VE501: the four answers to "What does EMVU stand for?" are English with
  the German expansion in brackets (a–c); d, a citizens' initiative, is a
  description and only translated (DECISIONS.md).
- VC104 b–d: "The National Metrology Institute (Physikalisch-Technische
  Bundesanstalt)", "The Federal Institution for Posts and
  Telecommunications (Bundesanstalt für Post und Telekommunikation)", "The
  Federal Agency for Public Safety Digital Radio (Bundesanstalt für den
  Digitalfunk der BOS)" — English names (BDBOS's own) with the German name
  in brackets, as *Kraftfahrt-Bundesamt* (NK308); the BDBOS bracket uses the
  agency's German short name, since the full one is fifteen words.
- VC101: four bare English titles, as the German gives four bare titles;
  "The Act on Amateur Radio" (glossary, the AFuG's formal title).
- VC118 c *Gesetz über Funkanlagen (FuAG)* → "Act on Radio Equipment
  (FuAG)", faithful to a title the FuAG does not have.
- VD203: *Präfix (Landeskenner)* / *Suffix (Landeskenner)* → "prefix
  (country prefix)" / "suffix (country prefix)" (glossary). In b and d the
  English shows the contradiction on its face ("suffix (country prefix)"),
  where the German *Landeskenner* needs the reader to know what it is; no
  other established English term for *Landeskenner* exists, so kept.
- VD705 a: the German paraphrases RR 5.28–5.30 but says plain *Störungen*;
  the English follows the RR's form ("shall not cause interference to …
  and cannot claim protection from interference from …") without the RR's
  "harmful", which the German does not have. VD704 a likewise.
- VC102 a: the AFuG definition of the amateur service is not RR 1.56 (it
  adds international understanding and relief operations), so it is
  translated faithfully, not in RR wording; *eigene Weiterbildung* → "their
  own further education". VC103: *Zusatzeinrichtungen* → "accessory
  equipment" (glossary, RR 1.61 term, which this AFuG definition follows).
- VC113: the stem takes "is concerned with the amateur service", so each
  answer is only "out of … interest." (the German repeats *mit dem
  Amateurfunkdienst befasst* in every answer).
- VC114: a "commercial purposes" and c "on a commercial basis" both say
  *commercial*, where the German has *gewerblich-wirtschaftlich* /
  *geschäftsmäßig* (both glossary). c is as plainly wrong as in German.
- VD301: stem "It is intended for ..." with four noun phrases; *dient der
  …* has no parallel English verb for all four answers.
- *grundsätzlich*: "as a rule" (VE308 a, d; VD408 d), "in principle"
  (VE404 b), "generally" (VB101 d) — never "always/never", which would
  make the distractors stronger statements than in German.
- VD117–VD119: the defined terms in quotes, as in German ("beacon",
  "repeater", "club station"); VD118 *fernausgelöst* → "when triggered
  remotely"; VD118 b *Erreichbarkeit* → "to make amateur stations easier to
  reach".
- VD103 d *Fernschreiben* → "teleprinting"; VD104 / VD103 a / VC124 d
  *verschlüsseln* → encrypt (DECISIONS.md).
- VD608 c *Bandwacht der Amateurfunkverbände* → "the amateur radio
  societies' Intruder Watch"; VE307 c *Intruder Monitoring* → "Intruder
  Watch" (glossary).
- VD724 *isotrope Strahlungsleistung (EIRP)* and VE507 a, d → "equivalent
  isotropically radiated power" (DECISIONS.md, EIRP); in VE507 d the German
  drops *isotropen*, but with EIRP written out a and d still differ, as in
  German, by "fixed". VD743 *effektive Strahlungsleistung (ERP)* → "effective
  radiated power (ERP)".
- VD725, VD726: *Gewinnfaktor 2,5 bezogen auf den isotropen Kugelstrahler*
  → "a gain of 2.5 (as a power ratio) relative to the isotropic radiator"
  (glossary).
- *Kurzwelle* → HF (VD105 d, VD109 b, VD119 d, VD601 b, VD723 c, d, VE508
  d); *UKW* → VHF (VD601 b, VE303, VE305).
- VD709–VD722: *Anfangs- und Endfrequenz* → "lower and upper band edges".
  VD718 a, d keep the German's "52.00" beside "50.0" (digits unchanged).
- VD735, VD733: *Teilbereich* → segment.
- VD406 c keeps the German's first person ("my personal licence"), as
  VD725 b, VD726 d ("I may not use").
- VC124: *bis zu 5000 bzw. 10000 Euro* → "fines of up to 5000 or 10000
  euros"; the four answers keep the German "(1) …; (2) …; (3) …" lists.
- VC124 c *Unzureichende Rufzeichennennung* → "Giving the call sign
  inadequately" (glossary *Rufzeichennennung*).
- VE204: *Abhören des nichtöffentlich gesprochenen Wortes* → "eavesdropping
  on private (non-public) conversations" (glossary), also VE201; b
  *breitbandiges Abhören des Funkspektrums* → "wideband listening to the
  radio spectrum".
- VE305 *Direkteinstrahlung* → "direct pick-up"; VE306
  *Kabelverteilanlagen* → "cable distribution systems".
- VE703 stem *Bei der ...* → "For the ..."; VE702 *verfügt über eine
  Amateurfunkstelle* → "has an amateur station".
- German generic *er* recast (DECISIONS.md, batch 07): "the radio amateur"
  or passive (VC107 d, VC116 a, VC119–VC120, VD113, VD302, VD404, VD502,
  VD504, VE203, VE301, VE305, VE306, VE511, VE704, VE707 d); VE302 b
  *seiner eigenen Einrichtung* → "the neighbour's own installation".
- VB102 a: the line break inside the answer dropped.
- Suspected slips in the German, translated faithfully or noted: VB102 c
  calls ERC Report 32 *diese Empfehlung*; VC108 c *ab Klassen E*; VC118 c
  the FuAG under a title it does not have; VC124 d trailing ";"; VD204 d
  *aufgrund besonderen historischen Anlass*; VD404 c *dass* for *das*;
  VD406 *Entsprechend des*; VD407 c *eines Amateurfunkzulassung*; VD718
  "50,0 bis 52,00" (mixed decimals); VE302 d lower-case *ihren*; VE401 b
  *AfuV*, VE503 b *AfuG* (written AFuV / AFuG in English); VE405 c *nach
  den Funkanlagengesetzes*; VE515 c *elektromagnetische Grenzwerte*; VE601
  a *anerkannte Regeln*; VE604 c *Normreihe* beside *Normenreihe*; VE702
  "Funkamateur..." without a space; VC121 c "Watt-Wächter" beside VE515
  "Watt Wächter" (each kept as written); VE507 d *äquivalenten
  Strahlungsleistung … EIRP* without *isotropen*. Whitespace in the
  German, all dropped: non-breaking space in VC124 Q; double spaces in
  VC108 d, VC118 b, VC120 d, VD115 a, VD119 c, d, VD305 a (several, plus a
  line break), VD704 d; trailing spaces in VC119 Q, VD407 a, VD720 Q,
  VD727 b, VD737 a, VE201 c, VE301 d; trailing newlines in VC118 b, d; line
  breaks in VB102 a, VD737 Q.
