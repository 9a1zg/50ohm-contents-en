# Translation glossary — German to English

The authoritative terminology for the English translation of 50ohm.de, for
DARC. Where this file and a translator's instinct disagree, this file wins;
where this file is silent, follow the RSGB's usage (Foundation, Intermediate
and Full licence manuals, *RSGB Radio Communication Handbook*) and, for
regulatory terms, the wording of the ITU Radio Regulations (RR). Extend the
file as new terms come up; do not rename or remove entries that translated
text already relies on — change them only together with the text.

The German term list was compiled from the German column of the Croatian
glossary (`50ohm-contents-hr/TRANSLATION_GLOSSARY.md`, German terms only —
none of its decisions) and from the most frequent technical nouns in the
question bank (`contents/questions/fragenkatalog3b.json`, 1750 questions).

## Rules from `TRANSLATION.md`, and the house style that follows from them

- **Faithful, not localised.** This is the German exam in English. The
  licence classes stay **N, E and A**; the Bundesnetzagentur, AFuG, AFuV,
  TKG, EMVG, BEMFV and every other German rule, body and institution stay
  German, under the English names given below. Nothing is adapted to the UK
  or any other country (no Ofcom, no UK licence classes, no UK band edges).
- **British English as used in IARU Region 1 and by the RSGB:**
  *licence* (noun) / *license* (verb), *licensed*, *licensee*; *metre*
  (unit) but *meter* (instrument: SWR meter, S meter, power meter);
  *centre*, *colour*, *programme* (but computer *program*), *analogue*,
  *aluminium*, *grey*, *fibre*, *behaviour*, *neighbour*, *travelling*,
  *modelling*, *analyser*, *polarisation*. Use **-ise** spellings
  (*authorisation*, *organisation*, *stabilisation*, *quantisation*,
  *synchronisation*) — except inside a direct quotation of the ITU RR,
  which spells *authorized*.
- ***mains*** for the public electricity supply (Netz, Netzspannung,
  Netzteil); ***earth*** for Erde / Erdung / Erder (never *ground*, except in
  fixed technical names: *ground wave*, *ground-plane antenna*).
- **Numbers:** decimal point, not comma (`3,5 MHz` → `3.5 MHz`); every
  number stays the same number. A space between number and unit
  (`100 W`, `14.2 MHz`). Band names: `80 m band`, `2 m band`, `70 cm band`
  (no hyphen; German `80 m-Band`).
- **Formulas and symbols stay exactly as in the German**, including German
  subscripts (`U_\mathrm{eff}`, `R_\mathrm{ges}`, `I_\mathrm{C}`); only words
  inside `\text{}` / `\textrm{}` are translated.
- **Call signs, Q codes and international operating abbreviations** (DL1ABC,
  QRV, QSO, CQ, CW, SSB, RST, PEP, EIRP, SWR, PLL, VFO) are not translated.
  **German-only technical abbreviations in running text** are replaced by
  their English equivalents: NF → AF, HF (Hochfrequenz) → RF, ZF → IF,
  KW → HF, UKW → VHF, EMV → EMC, Akku → battery. Abbreviations that name
  German law or bodies (AFuG, AFuV, BNetzA, TKG, TTDSG, EMVG, FuAG, BEMFV,
  EMVU, VDE) stay.
- **German law and institutions:** in the course text, at first use, the
  English name with the German name and abbreviation in brackets —
  *Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)* — then the
  abbreviation alone. **Exam questions stand alone:** where the German
  question writes the full name, use the full form from this glossary;
  where it writes only the abbreviation (BNetzA, AFuV), keep the
  abbreviation alone.
- **Exam questions:** `answer_a` is always the correct answer. Keep it
  correct and b–d wrong; keep the four answers parallel in form (all
  sentences, all noun phrases, same article pattern). A stem ending in `…`
  is continued by its answers — make the English stem end so that each
  answer completes it grammatically.
- **Address:** *Sie* and *du* both become plain *you*.
- **Markup:** DARCdown commands, file names, idents and `%` comments are
  never changed (`README-FORMAT.md`).
- **Capitalisation:** English sentence case for titles and headings
  (*Ohm's law*, *Electric field*), proper names and defined legal titles
  capitalised (*Amateur Radio Act*, *Call Sign Plan*).
- **Call sign** is two words, also when used attributively (*call sign
  holder*, *call sign plan*), as in the ITU RR — not the RSGB's *callsign*.

Columns: **German | English | note**. A note appears only where there is a
real choice or a trap.

## 1. Regulation and licensing

### 1.1 International bodies and instruments

| German | English | Note |
|---|---|---|
| Internationale Fernmeldeunion (ITU) | International Telecommunication Union (ITU) | singular *Telecommunication* |
| Radio Regulations (RR) / Vollzugsordnung für den Funkdienst (VO Funk) | Radio Regulations (RR) | the ITU treaty; keep "(RR)" where the German has it |
| Artikel (RR) | Article | RR Article 25 = "Article 25" |
| Anhang (RR), z. B. Anhang 14 | Appendix (e.g. Appendix 14) | RR has *Appendices*; AFuV has *Annexes* (Anlage) — do not mix |
| Begriffsbestimmung | definition | |
| Region 1 / 2 / 3 (ITU) | Region 1 / 2 / 3 | |
| Funkdienst | radiocommunication service; service | RR term; "a primary service" |
| Amateurfunkdienst | amateur service | RR 1.56; not "amateur radio service" (US usage) |
| Amateurfunkdienst über Satelliten | amateur-satellite service | RR 1.57, hyphenated as in the RR |
| primärer Funkdienst / sekundärer Funkdienst | primary service / secondary service | RR 5.23–5.28 wording |
| auf primärer Basis zugewiesen | allocated on a primary basis | |
| Zuweisung (Frequenzbereichszuweisung) | allocation (of a frequency band to a service) | RR: *allocation* to services, *allotment* to areas, *assignment* to stations |
| Frequenzzuteilung | frequency assignment | German TKG term for authorising a frequency use; not *allocation* |
| Seefunkdienst | maritime mobile service | RR term |
| Küstenfunkstelle | coast station | RR term |
| Luftfahrzeug | aircraft | |
| Wasserfahrzeug | vessel | |
| ISM-Frequenzbereich / ISM-Bereich | ISM band (industrial, scientific and medical) | |
| Bodenkontrollstation | earth command station | RR 25.2A wording |
| Steuersignale | control signals | |
| Verschleierung (zum Zwecke der Verschleierung) | (for the purpose of) obscuring the meaning | RR 25.2A wording; not "concealment" |
| verschlüsseln | encode; encrypt | RR says *encoded*; use *encrypt* only where the German clearly means cryptography — as in German law: AFuG / AFuV *zur Verschleierung … verschlüsseln* → encrypt (VC124, VD103, VD104; DECISIONS.md) |
| ordnungsgemäß befugte Personen | duly authorised persons | |
| ohne finanzielle Interessen / ohne wirtschaftliches Interesse | without pecuniary interest | RR 1.56 wording |
| mit persönlichem Ziel | solely with a personal aim | RR 1.56 wording |
| technische Studien | technical investigations | RR 1.56 wording |
| eigene Ausbildung | self-training | RR 1.56 wording |
| Funkverkehr untereinander | intercommunication | RR 1.56 wording |
| Bemerkungen persönlicher Art | remarks of a personal character | RR 25.2 wording |
| Morseprüfung / Morsequalifikation | Morse test / Morse qualification | |
| nationale Verwaltung | (national) administration | RR term for the national regulator |
| Funkstelle | station | RR 1.61; "radio station" only where needed for clarity |
| Amateurfunkstelle | amateur station | RR 1.96 |
| Zusatzeinrichtungen | accessory equipment | RR 1.61 wording "accessory equipment" |
| Europäische Konferenz der Verwaltungen für Post und Telekommunikation (CEPT) | European Conference of Postal and Telecommunications Administrations (CEPT) | |
| CEPT-Empfehlung T/R 61-01 / T/R 61-02 | CEPT Recommendation T/R 61-01 / T/R 61-02 | |
| ECC-Empfehlung (05)06 | ECC Recommendation (05)06 | |
| ERC-Report 32 | ERC Report 32 | |
| CEPT-Länder / Nicht-CEPT-Länder | CEPT countries / non-CEPT countries | |
| CEPT-Amateurfunkgenehmigung | CEPT radio amateur licence | |
| CEPT-Novice-Amateurfunkgenehmigung | CEPT Novice Radio Amateur Licence | ECC (05)06 name |
| CEPT-Novice-Amateurfunk-Prüfungsbescheinigung | CEPT Novice Radio Amateur Examination Certificate | |
| Novice-Individualgenehmigung | individual novice licence | |
| HAREC (Harmonized Amateur Radio Examination Certificate) | HAREC (Harmonised Amateur Radio Examination Certificate) | the CEPT document title is spelt *Harmonised* |
| HAREC-Bescheinigung | HAREC certificate | |
| harmonisierte Amateurfunk-Prüfungsbescheinigung | harmonised amateur radio examination certificate | |
| gegenseitige Anerkennung | mutual recognition | |
| vorübergehender Betrieb | temporary operation | |
| Gastland | host country | |
| Gastgenehmigung / Gastzulassung | guest licence | |
| fester Wohnsitz | permanent residence | |
| umsetzen (eine Empfehlung) | implement (a recommendation) | |
| IARU (International Amateur Radio Union) | IARU (International Amateur Radio Union) | |
| Intruder Monitoring (IARU-Monitoring-System) | Intruder Watch / IARU Monitoring System | |
| Sendearten (RR) | classes of emission | RR term (VA301) |
| Landeskennerliste der ITU | the ITU's list of country prefixes | BD301 |
| Gastlizenz | guest licence | as *Gastgenehmigung* (VA401) |
| CEPT-Regelung | CEPT arrangement | VB109 |
| Mitgliedsländer (der CEPT) / Mitgliedsstaaten (der EU) | (CEPT) member countries / member states (of the EU) | VB106, VB107 |
| umsetzende Länder / beteiligte Länder | implementing countries / participating countries | VB103, VB104 |
| Gegenseitigkeitsabkommen | reciprocal agreements | VB113 |
| Harmonisierung (der Frequenzzuweisungen) | harmonisation (of frequency allocations) | VB104 |
| ETSI (European Telecommunications Standards Institute) | ETSI (European Telecommunications Standards Institute) | VA101, VA407 |
| Internationale Organisation für Normung (ISO) | International Organization for Standardization (ISO) | proper name, spelt with *-z-* |
| Not- und Katastrophenfunkübungen | emergency and disaster communication exercises | VA302 |
| Bodenkontrollstationen auf der Erde | earth command stations | VA303; "auf der Erde" is already in the English term (RR 25.2A) |
| Mitteilungen im Zusammenhang mit dem definitionsgemäßen Zweck des Amateurfunkdienstes | communications incidental to the purpose of the amateur service as defined | RR 25.2 wording (VA302) |
| Mitteilungen von geringer Bedeutung, die es nicht rechtfertigen, öffentliche Telekommunikationsdienste in Anspruch zu nehmen | messages of minor importance, for which recourse to public telecommunications services is not justified | older RR 25.2 wording, distractor VA104 |
| sich für Funktechnik interessieren | interested in radio technique | RR 1.56 wording (VA104) |
| Weltraumfunkstelle | space station | RR 1.64 (VC115) |
| Sicherheitsfunkdienst | safety service | RR 1.59 (VD704) |
| Richtlinie Elektromagnetische Verträglichkeit von Elektro- und Elektronikprodukten (EMV-Richtlinie) | Directive on the electromagnetic compatibility of electrical and electronic products (EMC Directive) | the EU EMC Directive; *EMC Directive* is its established English short name (VE505) |

### 1.2 German law, bodies and documents

| German | English | Note |
|---|---|---|
| Bundesnetzagentur (BNetzA) | Federal Network Agency (Bundesnetzagentur, BNetzA) | in exam questions: "the Federal Network Agency (BNetzA)" where the German writes the name; "BNetzA" where the German writes only the abbreviation |
| Bundesnetzagentur für Elektrizität, Gas, Telekommunikation, Post und Eisenbahnen | Federal Network Agency for Electricity, Gas, Telecommunications, Post and Railway | full official name, rarely needed |
| Außenstelle (der BNetzA) | (BNetzA) regional office | |
| zuständige Stelle / zuständige Behörde | competent office / competent authority | |
| Funkstörungsannahme (der BNetzA) | (BNetzA) radio interference reporting service | keep "Funkstörungsannahme" in brackets at first mention in course text |
| Prüf- und Messdienst (der BNetzA) | (BNetzA) inspection and measurement service | EK209 |
| Hauptzollamt | main customs office | NJ102 |
| Kraftfahrt-Bundesamt | Federal Motor Transport Authority (Kraftfahrt-Bundesamt) | NK308 |
| Frequenzbereichszuweisungsplan (der Bundesrepublik Deutschland) | Frequency Band Allocation Plan (of the Federal Republic of Germany) | BD301 |
| Angehörige der Gaststreitkräfte | members of the visiting forces | foreign armed forces stationed in Germany; *visiting forces* is the English legal term (BD101, BD107, BD108) |
| Fernmeldedienst | telecommunications service | BE116 |
| Runder Tisch Amateurfunk (RTA) / EMV-Beauftragter des RTA | RTA / the RTA's EMC officer | the German amateur radio associations' round table; in exam questions "RTA" alone, as the German (AJ116) |
| Behörde | authority | |
| Amateurfunkgesetz (AFuG) | Amateur Radio Act (Amateurfunkgesetz, AFuG) | |
| Gesetz über den Amateurfunk | Act on Amateur Radio | the AFuG's formal title; VC101 asks for it, so keep it distinct from "Amateur Radio Act" |
| Amateurfunkverordnung (AFuV) | Amateur Radio Ordinance (Amateurfunkverordnung, AFuV) | *Ordinance*, not *Regulation(s)* (avoids confusion with the RR) |
| Anlage 1 der AFuV | Annex 1 to the AFuV | |
| Telekommunikationsgesetz (TKG) | Telecommunications Act (Telekommunikationsgesetz, TKG) | |
| Telekommunikation-Telemedien-Datenschutz-Gesetz (TTDSG) | Telecommunications and Telemedia Data Protection Act (Telekommunikation-Telemedien-Datenschutz-Gesetz, TTDSG) | renamed TDDDG in 2024; the question bank still says TTDSG — translate what the German says |
| Telekommunikation-Digitale-Dienste-Datenschutz-Gesetz (TDDDG) | Telecommunications Digital Services Data Protection Act (TDDDG) | |
| Gesetz über den Datenschutz und den Schutz der Privatsphäre in der Telekommunikation und bei digitalen Diensten (TDDDG) | Act on Data Protection and the Protection of Privacy in Telecommunications and Digital Services (TDDDG) | the TDDDG's formal title, in a section title of DARC's SWL question set (fragenkatalog_swl.json); a long title takes the abbreviation only, as the EMVG (DECISIONS.md) |
| Gesetz über die elektromagnetische Verträglichkeit von Betriebsmitteln (EMVG) | Act on the Electromagnetic Compatibility of Equipment (Gesetz über die elektromagnetische Verträglichkeit von Betriebsmitteln, EMVG) | short: Electromagnetic Compatibility Act (EMVG); in exam questions, where the German writes the long title, "Act on the Electromagnetic Compatibility of Equipment (EMVG)" without the German title (DECISIONS.md) |
| Gesetz über die elektromagnetische Verträglichkeit von Geräten (EMVG) | Act on the Electromagnetic Compatibility of Devices (EMVG) | older title, used in a catalogue heading; keep *Devices* vs *Equipment* as in the German |
| Gesetz über die Bereitstellung von Funkanlagen auf dem Markt (FuAG) / Funkanlagengesetz | Act on Making Radio Equipment Available on the Market (Funkanlagengesetz, FuAG) / Radio Equipment Act | in exam questions *Funkanlagengesetz (FuAG)* → "Radio Equipment Act (Funkanlagengesetz, FuAG)" (VE4, DECISIONS.md) |
| Verordnung über das Nachweisverfahren zur Begrenzung elektromagnetischer Felder (BEMFV) | Ordinance on the Verification Procedure for Limiting Electromagnetic Fields (BEMFV) | |
| 26. Verordnung zur Durchführung des Bundes-Immissionsschutzgesetzes (26. BImSchV) | 26th Ordinance implementing the Federal Immission Control Act (Ordinance on Electromagnetic Fields, 26. BImSchV) | *immission* is the established English term in German environmental law |
| Anhang 1a / 1b / 3 (26. BImSchV) | Annex 1a / 1b / 3 | annexes of German ordinances are *Annex*, as AFuV *Anlage*; RR *Appendix* is only for the ITU (EK102) |
| Frequenzschutzbeitragsverordnung (FSBeitrV) | Frequency Protection Contribution Ordinance (FSBeitrV) | |
| Frequenzschutzbeitrag | frequency protection contribution | annual fee |
| Besondere Gebührenverordnung BNetzA (BNetzABGebV) | Special Fees Ordinance of the BNetzA (BNetzABGebV) | |
| Gebühren und Beiträge | fees and contributions | |
| Verwaltungs-Vollstreckungsgesetz | Administrative Enforcement Act | |
| Bundes-Immissionsschutzgesetz (BImSchG) | Federal Immission Control Act (BImSchG) | as in the 26. BImSchV row (VD108, VE503, VE511); with the abbreviation also where the German leaves it out (VE511 d) |
| Verordnung zum Gesetz über den Amateurfunk | Ordinance under the Act on Amateur Radio | the AFuV's formal title, beside *Gesetz über den Amateurfunk* (VE505) |
| Gesetz über Funkanlagen (FuAG) | Act on Radio Equipment (FuAG) | not the FuAG's real title; translated as the German writes it (VC118) |
| Frequenzverordnung (FreqV) / Anlage zur Frequenzverordnung | Frequency Ordinance (FreqV) / Annex to the Frequency Ordinance | VD101, VD702 |
| Frequenzplan (FreqP) | Frequency Plan (FreqP) | the BNetzA's plan, capitalised as a named document, also in the AFuG's "im Frequenzplan … ausgewiesenen Frequenzen" (VC102, VC103, VD702); cf. §2 *Frequenzplan* |
| Frequenznutzungsplan | Frequency Usage Plan | the Frequency Plan's former name (VD116) |
| Frequenznutzungsplanaufstellungsverordnung | Ordinance on Drawing Up the Frequency Usage Plan (Frequenznutzungsplanaufstellungsverordnung) | repealed ordinance, distractor VD701; the one-word German title stays in brackets |
| Bundesgesetzblatt (BGBl) | Federal Law Gazette (BGBl) | VD201 |
| Physikalisch-Technische Bundesanstalt | National Metrology Institute (Physikalisch-Technische Bundesanstalt) | as *Kraftfahrt-Bundesamt* (VC104) |
| Bundesanstalt für Post und Telekommunikation | Federal Institution for Posts and Telecommunications (Bundesanstalt für Post und Telekommunikation) | VC104 |
| Bundesanstalt für den Digitalfunk der Behörden und Organisationen mit Sicherheitsaufgaben (BDBOS) | Federal Agency for Public Safety Digital Radio (Bundesanstalt für den Digitalfunk der BOS) | the agency's own English name; German short name in brackets (VC104) |
| Bundesamt für Seeschifffahrt und Hydrographie | Federal Maritime and Hydrographic Agency | the agency's own English name (VE706) |
| Bauaufsichtsbehörde | building control authority | VE603 |
| eingetragener Verein (e. V.) | registered association (e. V.) | VD117, VD401 |
| Führungszeugnis / Personalausweis / Reisepass | certificate of good conduct / identity card / passport | VC105 |
| Volljährigkeit | age of majority | VC108 |
| Ordnungswidrigkeitenverfahren / Bußgeldverfahren | administrative offence proceedings / administrative fine proceedings | VE303, VE304 |
| Betriebsverbot / Betriebseinschränkung | ban on operation / restriction of operation | VE303 |
| Beschlagnahmung | seizure | VC125 |
| Entzug / Einzug (des Amateurfunkzeugnisses) | withdrawal / confiscation (of the amateur radio certificate) | VC123, VC125, VE704 |
| Unbrauchbarmachen | rendering unusable | VC122 |
| kostenpflichtig / gebührenpflichtig | subject to a fee | |
| behördliche Abhilfemaßnahmen | official remedial measures | VE303 |
| Sonderverfügung | special order | VD204 |
| sachkundige Person | competent person | VE201, VE601 |
| Haftpflichtversicherung / Antennenhaftpflichtversicherung / Gruppenversicherung | liability insurance / antenna liability insurance / group insurance | VE707 |
| Grundstückseigentümer | owner of the property | VE707 |
| Strafgesetzbuch (StGB) | Criminal Code (Strafgesetzbuch, StGB) | |
| § 323c StGB (unterlassene Hilfeleistung) | Section 323c StGB (failure to render assistance) | § → "Section" in prose, "§" may stay in citations |
| Abs. (Absatz) | para. (paragraph) / subsection | "§ 3 Abs. 1 AFuG" → "Section 3(1) AFuG" |
| Verfügung 13/2005 | Order 13/2005 | BNetzA order in its Official Gazette |
| Amtsblatt | Official Gazette | |
| Mitteilungen der BNetzA | BNetzA notices | |
| Rufzeichenplan | Call Sign Plan | BNetzA document, capitalised |
| Rufzeichenliste | call sign list | published by the BNetzA |
| Verband der Elektrotechnik Elektronik Informationstechnik (VDE) | VDE (Association for Electrical, Electronic and Information Technologies) | keep "VDE" |
| VDE-Normen / Norm VDE 0855-300 / Normenreihe VDE 0185-305 | VDE standards / standard VDE 0855-300 / series of standards VDE 0185-305 | |
| anerkannte Regeln der Technik | recognised codes of practice (generally accepted rules of engineering) | legal term; use "generally accepted rules of engineering" in AFuV quotations |
| Bundesland | federal state (Land) | "the building regulations of the relevant federal state" |
| Baurecht / baurechtliche Bestimmungen | building law / building regulations | |
| Baugenehmigung | building permit (planning permission) | |
| Bauamt | building authority | |
| Ordnungswidrigkeit | administrative offence | not "misdemeanour" |
| Bußgeld / Geldbuße | (administrative) fine | |
| ahnden | punish (with a fine) | |
| Straftatbestand / Straftat | criminal offence | |
| Widerruf (der Zulassung) | revocation (of the licence) | |
| Außerbetriebnahme | taking out of service; shutdown | |
| Einschränkung des Betriebes | restriction of operation | |
| Antrag / auf Antrag | application / on application | |
| Auflagen | conditions | |
| Fernmeldegeheimnis | secrecy of telecommunications | |
| Abhörverbot | prohibition of interception | |
| Abhören des nichtöffentlich gesprochenen Wortes | eavesdropping on private (non-public) conversations | |
| Nachrichten | messages | |
| Allgemeinheit / unbestimmter Personenkreis | the general public / an unspecified group of people | |
| CE-Kennzeichnung | CE marking | |
| Inverkehrbringen | placing on the market | EU legal wording |
| auf dem Markt bereitstellen | make available on the market | EU legal wording |
| freier Warenverkehr | free movement of goods | |
| Inbetriebnahme | putting into service | |
| grundlegende Anforderungen | essential requirements | EU legal wording |
| Schutzanforderungen | protection requirements | |
| seriengefertigte Geräte | series-produced equipment | |
| Selbstbaugerät / Eigenbaugerät | home-built equipment | |
| Haftung / haften | liability / be liable | |
| Eigentümer | owner | |
| Datenschutz | data protection | |

### 1.3 Licence, call sign and station

| German | English | Note |
|---|---|---|
| Funkamateur | radio amateur | |
| Nicht-Funkamateur | non-amateur; person who is not a radio amateur | |
| Amateurfunk | amateur radio | |
| Amateurfunkprüfung / Prüfung | amateur radio examination / examination | *exam* in informal text |
| fachliche Prüfung | examination of competence | AFuV wording |
| Prüfungsteil | part of the examination | |
| Prüfungsfrage | examination question | |
| Prüfungsfragen im Prüfungsteil: … | Examination questions in the examination part: … | catalogue heading pattern |
| Amateurfunkzeugnis | amateur radio certificate | the BNetzA certificate of competence issued after the exam; not a licence |
| Amateurfunk-Prüfungsbescheinigung / Prüfungsbescheinigung | amateur radio examination certificate / examination certificate | |
| Prüfungsbescheid | examination result notice | |
| Zulassung zur Teilnahme am Amateurfunkdienst | authorisation to participate in the amateur service | the AFuG's personal authorisation; same thing as "Amateurfunkzulassung" |
| Zulassung zum Amateurfunkdienst | authorisation for the amateur service | VD403 variant; keep it distinct only if the German contrasts them |
| Amateurfunkzulassung / Zulassung | amateur radio licence / licence | |
| Zulassungsurkunde | licence document | |
| Zulassungsklasse / Zeugnisklasse | licence class / certificate class | |
| Klasse N / E / A | Class N / E / A | "Zulassung der Klasse A" → "Class A licence"; never renamed Foundation/Intermediate/Full |
| Inhaber einer Zulassung der Klasse A | holder of a Class A licence; Class A licensee | |
| Erteilung | issue (of a licence); grant | |
| Mindestalter | minimum age | |
| übertragbar / nicht übertragbar | transferable / not transferable | |
| Berechtigungsumfang | scope of privileges; privileges | |
| Rufzeichen | call sign | two words; RSGB writes *callsign* |
| Amateurfunkrufzeichen | amateur call sign | |
| personengebundenes Rufzeichen | personal call sign | |
| Klubstation | club station | |
| Klubstationsrufzeichen | club station call sign | |
| Ausbildungsrufzeichen | training call sign | |
| Rufzeichenzuteilung | call sign assignment | |
| Zuteilung | assignment | |
| Rufzeicheninhaber | call sign holder | |
| Rufzeichenzuteilungsart / Rufzeichenart | category of call sign assignment / category of call sign | |
| Rufzeichen für fernbediente und automatisch arbeitende Amateurfunkstellen | call signs for remotely controlled and automatically operating amateur stations | |
| Präfix | prefix | |
| Ziffer | digit | |
| Suffix | suffix | the letters after the digit; see Rufzeichenzusatz |
| Rufzeichenzusatz | call sign suffix (/p, /m, /mm, /am, /T) | Ofcom/RSGB usage; where *Suffix* and *Rufzeichenzusatz* meet in one sentence, write "the suffix /p added to the call sign" |
| Landeskenner | country prefix | the nationality part of the call sign (RR Art. 19); but **country identifier** where it glosses *Präfix* / *Suffix* (VD203): "suffix (country prefix)" would give the wrong answers away |
| Heimatrufzeichen | home call sign | |
| vorangestellt | placed in front; prefixed | "DL/ is prefixed" |
| Stationsverantwortlicher / verantwortlicher Funkamateur | responsible radio amateur (station manager) | |
| Leiter einer Gruppe | leader of a group | |
| Mitglied / Nichtmitglied | member / non-member | |
| Betreiber | operator (of a station or installation) | for remote stations: "the operator of the remote station" |
| Amateurfunkstation | amateur station | same as Amateurfunkstelle |
| Amateurfunkanlage | amateur radio installation; amateur radio equipment | |
| Funkanlage | radio equipment; radio installation | FuAG: *radio equipment* |
| Sendefunkanlage / Sendeanlage | transmitting equipment; transmitter | |
| Empfangsfunkanlage | receiving equipment | |
| Antennenanlage | antenna installation | |
| ortsfest | fixed | "ortsfeste Amateurfunkstelle" → "fixed amateur station" |
| vorübergehend ortsfest (/p) | at a temporary fixed location (portable) | |
| mobil (/m) | mobile | |
| maritim mobil (/mm) | maritime mobile | |
| an Bord eines Luftfahrzeugs (/am) | aeronautical mobile; on board an aircraft | |
| Schiffsführer | master (of the ship) | |
| Luftfahrzeugführer | pilot in command | |
| Standort | location; site | |
| Standortänderung | change of location | |
| anzeigen (der BNetzA) | notify (the BNetzA) | |
| Betriebsmeldung | operating notification | |
| Ausbildungsfunkbetrieb / Ausbildungsfunkverkehr | training operation | supervised transmissions by trainees under the instructor's call sign |
| Ausbilder | instructor | |
| Auszubildender | trainee | |
| Trainee (/T, /Trainee) | trainee | the suffix itself stays "/T" / "/Trainee" |
| unmittelbare Anleitung und Aufsicht | direct guidance and supervision | |
| Relaisfunkstelle | repeater (station) | AFuV definition; "Relaisfunkstellen und Funkbaken" → "repeaters and beacons" |
| Funkbake / Bake | beacon | |
| fernbedient | remotely controlled | |
| automatisch arbeitend | automatically operating; unattended | |
| Remote-Station | remote station | |
| Remote-Betrieb | remote operation | |
| mittelbare / unmittelbare Kontrolle | indirect / direct control | |
| Nutzungsrecht | right of use | |
| Ansprechpartner | contact person | |
| Kontaktdaten | contact details | |
| Frequenznutzung | frequency use | |
| Frequenznutzungsparameter | frequency usage parameters | |
| Frequenzbereich | frequency range; band | in band-edge questions "frequency range"; "frequency band" where the German means the band |
| Amateurfunkband / Band | amateur band / band | |
| Amateurfunkfrequenzen | amateur frequencies | |
| ausgewiesene Frequenzen | designated frequencies | |
| Anfangs- und Endfrequenz | lower and upper band edge; start and end frequency | |
| Teilbereich | segment; sub-band | |
| belegte Bandbreite | occupied bandwidth | RR 1.153 |
| Leistungsgrenze | power limit | |
| Senderausgangsleistung | transmitter output power | |
| maximal zulässig | maximum permitted | |
| Not- und Katastrophenfälle | emergencies and disasters | "in Not- und Katastrophenfällen" → "in emergencies and disasters" |
| Nachrichtenübermittlung an Dritte / Nachrichten für Dritte | third-party traffic; passing messages for third parties | RSGB term *third-party traffic* |
| Dritte | third parties | |
| gewerblich-wirtschaftliche Zwecke | commercial purposes | |
| geschäftsmäßiges Erbringen von Telekommunikationsdiensten | providing telecommunications services on a commercial basis | |
| Völkerverständigung | international understanding; international goodwill | |
| Unterstützung von Hilfsaktionen | supporting relief operations | |
| experimentelle und technisch-wissenschaftliche Studien | experimental and technical-scientific studies | |
| Weiterbildung | further education; self-training | |
| persönliche Neigung | personal interest | |
| offene Sprache | plain language | |
| Sprachverschlüsselung | voice encryption | |
| Not-, Dringlichkeits- und Sicherheitszeichen | distress, urgency and safety signals | RR terms; MAYDAY, PAN PAN, SÉCURITÉ unchanged |
| unmodulierter / ungetasteter Träger | unmodulated / unkeyed carrier | |
| Abgleicharbeiten | alignment work | |
| freies Abstrahlen | unrestricted radiation | |
| unerwünschte Aussendungen | unwanted emissions | RR 1.146 |
| geringstmögliches Maß | the lowest possible level | |
| Logbuch / Stationstagebuch | log / station log (logbook) | |
| auf Verlangen / auf Anforderung (der BNetzA) | at the request of (the BNetzA) / on demand | |
| technische Unterlagen | technical documentation | |
| frequenztechnische Fragen | questions of frequency engineering | |
| Störungsursachen | causes of interference | |
| unverzüglich | without delay | |
| schriftlich oder elektronisch | in writing or electronically | |
| Anschrift | (postal) address | |
| widersprechen | object | "unless the holder has objected" |
| Sondergenehmigung | special permit | |
| Ausnahmen | exceptions | |
| Rahmenbedingungen | (general) conditions; framework | |
| Kurzzeitzuteilung | short-term assignment | of a call sign (BD102) |
| Versuchsfunkstelle | experimental radio station | BD102 |
| exterritorial / exterritorialer Standort | extraterritorial / extraterritorial location | BD107, BD108; cf. *exterritoriale Station* (§14) |
| Rufzeichennennung | giving the call sign | "Wie muss die Rufzeichennennung von DL9MJ … erfolgen?" → "How must the call sign of DL9MJ be given …?" (BD213, BD214) |
| Kennung | identifier | BD109 |
| zwei- oder dreistelliges Suffix | two- or three-letter suffix | BD104, BD106, BE306 |
| Kurzwellenhörer | short-wave listener | BD105 |
| Rufzeichenzusätze in Antworten (/Ausbildung, /Remotebetrieb, /Fernbedient, /Fern) | unchanged | strings added to a call sign, kept as the German writes them, like the call sign itself (BD208, BD209; DECISIONS.md) |
| gemeldeter Standort | notified location | BD207 |
| Landfahrzeug | land vehicle | BD203, BD206 |
| Binnengewässer | inland waters | BD204, BD205 |
| See- und Binnenschifffahrtsfunk | maritime and inland waterway radio service | BD205 |
| angeordnete Logbuchführung | (where) keeping a log has been ordered | BG102, BG103 |
| Zulassungsklasse N | licence class N | VB105 |
| Rufzeicheninhaber der Klasse A / Funkamateure der Klasse A | Class A call sign holders / Class A radio amateurs | VD603, VD727–VD737 |
| Hörerrufzeichen ("DE-Reihe") | listener call sign ("DE series") | VD102 |
| Familienrufzeichen / Contestrufzeichen / Mobilfunkrufzeichen | family call signs / contest call signs / mobile radio call signs | made-up categories in VD202 |
| Zuteilungsurkunde | assignment document | VD609; cf. *Zulassungsurkunde* → licence document |
| Schulstation | school station | VD305, VD306 |
| (Rufzeichen) mitbenutzen | share (a call sign) | VD404 |
| Betriebssicherheit (Remote-Station) | operational safety | VD605 |
| Bandwacht (der Amateurfunkverbände) | Intruder Watch | the societies' monitoring service, part of the IARU Monitoring System, as *Intruder Monitoring* (VD608) |
| Relaisnutzungsgebühr | repeater usage fee | VD504 |
| Flugfunkzeugnis / Seefunkzeugnis | aeronautical / maritime radio operator's certificate | VD115 |
| Notfunkübung | emergency communications exercise | VC110 |
| Feldstärkebeobachtung / Empfangsversuche | observing field strength / reception tests | AFuV definition of *Funkbake* (VD119) |
| fernausgelöst | when triggered remotely | AFuV definition of *Relaisfunkstelle* (VD118) |
| Frequenznutzungsbeiträge / Zuteilungsbeiträge | frequency usage contributions / assignment contributions | VD108, VE701 |
| Verträglichkeitsbescheinigung / EMVU-Bescheinigung | compatibility certificate / EMVU certificate | VC106, VC118 |
| baumustergeprüft | type-tested | VC118 |
| zertifizierter Elektromeister / Abnahmeprotokoll | certified master electrician / acceptance report | VC118 |

### 1.4 EMF exposure (EMVU / BEMFV)

| German | English | Note |
|---|---|---|
| EMVU (elektromagnetische Verträglichkeit in der Umwelt / elektromagnetische Umweltverträglichkeit) | EMVU (electromagnetic compatibility with the environment) | i.e. human exposure to RF fields; keep the German abbreviation; VE501 asks what it stands for, and its answers give the English with the German expansion in brackets (DECISIONS.md) |
| Schutz von Personen in elektromagnetischen Feldern | protection of persons in electromagnetic fields | |
| Personenschutz | protection of persons | |
| Sachschutz | protection of property | |
| aktive Körperhilfen | active implants (active medical implants) | e.g. pacemakers |
| Herzschrittmacher | pacemaker | |
| Sicherheitsabstand | safety distance | |
| Personenschutz-Sicherheitsabstand / Personenschutzabstand | safety distance for the protection of persons | |
| Schutzabstand | safety distance | AK101 |
| Grenzwert im Fall des Personenschutzes / Personenschutzgrenzwerte | limit for the protection of persons / limits for the protection of persons | AK106–AK112, EK104 |
| nicht kontrollierbarer Bereich / kritischer Winkel | area that is not controllable / critical angle | AK105 |
| Fernfeldnäherung / Näherungsformel für die Fernfeldberechnung | far-field approximation / far-field approximation formula | EK105–EK107 |
| quadratisch gemittelt über 6 Minuten | RMS value averaged over 6 minutes | EK102, EK103 |
| kurzfristiger Effektivwert / momentaner Spitzenwert / Momentanwert | short-term RMS value / instantaneous peak value / instantaneous value | EK102, EK103 |
| spezifische Absorptionsrate | specific absorption rate (SAR) | EK101 |
| Anzeige ortsfester Amateurfunkanlagen | "Notification of fixed amateur radio installations" | the BNetzA form under Section 9 BEMFV (EK105) |
| standortbezogener Sicherheitsabstand | site-specific safety distance | |
| kontrollierbarer Bereich | controllable area | the area under the operator's control |
| Anzeige (BEMFV) | notification | trap: *Anzeige* is also a meter reading / display, see §11 |
| Anzeigeverfahren | notification procedure | |
| Nachweisverfahren | verification procedure | |
| Standortbescheinigung | site certificate | |
| Bewertungsverfahren / vereinfachtes Bewertungsverfahren | assessment procedure / simplified assessment procedure | |
| Watt Wächter | Watt Wächter (BNetzA calculation tool) | proper name, keep |
| Feldstärkemessung | field-strength measurement | |
| Fernfeldberechnung / Nahfeldberechnung | far-field calculation / near-field calculation | |
| Grenzwert / Grenzwerte | limit / limit values | |
| Dokumentation | documentation; records | |
| Lageplan | site plan | |
| Bauzeichnung | construction drawing | |
| Bemaßung | dimensions | |
| Antennendiagramm | antenna (radiation) pattern | |
| Gesamtleistung | total power | |
| Nachweis zur Begrenzung elektromagnetischer Felder | verification for limiting electromagnetic fields | as *Nachweisverfahren* (VE515) |
| Anzeigeformblatt / zeichnerische Darstellung | notification form / drawing | VE512, VE513 |
| (zertifiziertes) Messlabor | (certified) measurement laboratory | VE504, VE506 |
| (mechanischer) Sendeumschalter | (mechanical) transmit changeover switch | VE518 |

## 2. Operating

| German | English | Note |
|---|---|---|
| Betrieb / Funkbetrieb | operation; operating | |
| Sendebetrieb | transmitting; transmission | |
| Amateurfunkverkehr / Funkverkehr | amateur radio communication / radio communication; traffic | |
| Abwicklung des Amateurfunkverkehrs | conduct of amateur radio communication | catalogue heading |
| Betriebsabwicklung | operating procedure(s) | |
| betriebliche Kenntnisse | operating knowledge | parallel to *technical knowledge* and *knowledge of regulations* |
| Kenntnisse von Vorschriften | knowledge of regulations | |
| technische Kenntnisse | technical knowledge | |
| Funkverbindung / Verbindung | contact (QSO) | not "radio connection"; in circuits *Verbindung* = connection |
| Direktverbindung | direct contact | as opposed to via a repeater |
| Gegenstation | the other station; the station worked | |
| QSO-Partner / Funkpartner | the other station | NF112, AF102 |
| Funkrunde | net | RSGB term for a scheduled round of stations (NE402) |
| Funkgerät | radio; transceiver | |
| Amateurfunkgerät | amateur radio equipment; amateur transceiver | |
| Funkstation / Station | station | |
| Anruf | call | |
| allgemeiner Anruf (CQ) | general call (CQ) | |
| gezielter Anruf | directed call | |
| Anruffrequenz | calling frequency | |
| Aktivitätszentrum | centre of activity | British *centre* |
| Antwort / antworten | reply; answer | |
| Durchgang | over | one station's turn in a contact (BB101, BB109, BB110) |
| aufnehmen (ein Signal, eine Q-Gruppe) | receive; copy | "Wie verhalten Sie sich, wenn Sie … aufnehmen?" → "What do you do when you receive …?" (BB205, BB206) |
| formlose Übergabe | informal handover | BK (BB108) |
| Bestätigungskarte | confirmation card | QSL card in plain words (BB205, BB206) |
| Rapport | (signal) report | |
| RST-System | RST system | |
| Lesbarkeit | readability | |
| Signalstärke | signal strength | |
| Tonqualität / Ton | tone (quality) | |
| Signalbeurteilung | signal reports | catalogue heading |
| S-Meter / S-Meter-Anzeige | S meter / S-meter reading | |
| S-Stufe | S unit | "eine S-Stufe = 6 dB" → "one S unit" |
| Buchstabieralphabet / Buchstabiertafel | phonetic alphabet | RSGB term |
| internationales Buchstabieralphabet | international phonetic alphabet | lower case, so it is not taken for the linguists' IPA; the words themselves (Alfa, Juliett, X-ray) keep the ITU spelling |
| Wörter anderer Buchstabieralphabete (Nordpol, Ypsilon, Caesar …) | unchanged | distractors in BA101–BA110 are words of other spelling alphabets (German DIN 5009, old international and wartime alphabets); kept as the German writes them, except *Amerika* → America, since the German otherwise uses the English spellings (Denmark, Italy, Madagascar) |
| buchstabieren | spell (out) | |
| Stroke (/) | stroke | "Delta Lima 4 Stroke portable" unchanged |
| betriebliche Abkürzungen | operating abbreviations | |
| Abkürzung | abbreviation | |
| Q-Gruppen / Q-Schlüssel | Q codes | |
| Bedeutungen der Q-Gruppen | Q code meanings | written in the established English wording of the ITU Q code list (Rec. ITU-R M.1172, incorporated by reference in the RR; not RR Appendix 14, which is the phonetic alphabet and figure code) where the German gives the German wording: QRV "I am ready.", QRM "I am being interfered with.", QRM? "Are you being interfered with?" (the older wording the German follows; current M.1172 has "Your transmission is being interfered with" / "Is my transmission being interfered with?", see DECISIONS.md), QRN "I am troubled by static.", QSB? "Are my signals fading?", QRT "Stop sending.", QRZ? "Who is calling me?", QSL? "Can you acknowledge receipt?", QRO? "Shall I increase transmitter power?", QSO? "Can you communicate with ... direct?", QRX? "When will you call me again?", QRU "I have nothing for you." / QRU? "Have you anything for me?"; QTH "My location is ..." (*Standort* → location; ITU "My position is …"). Made-up distractors faithfully (BB201–BB204) |
| Morsetelegrafie / Telegrafie | Morse telegraphy / telegraphy (CW) | |
| Morsezeichen / Morsecode | Morse characters / Morse code | |
| Telefonie / Sprechfunk | telephony; voice | "SSB-Telefonie" → "SSB telephony"; "FM-Sprechfunk" → "FM voice" |
| Fonie / Fonie-Signale | voice; voice signals | beside CW (AH308) |
| Funkfernschreiben (RTTY) | radioteletype (RTTY) | |
| Bandplan / IARU-Bandplan | band plan / IARU band plan | |
| Frequenzplan | frequency plan | |
| Contest | contest | |
| Ausschreibung (Contest) | contest rules | |
| Pile-Up | pile-up | |
| Split-Betrieb | split operation | |
| Listenbetrieb | list operation | |
| DX / DX-Pedition | DX / DXpedition | |
| DX-Cluster | DX cluster | |
| Fuchsjagd / ARDF | direction finding (ARDF); foxhunt | RSGB: *ARDF* or *DF hunt*; use "foxhunt" only in informal course text and where the German quotes the colloquial word itself ("Was verstehen Funkamateure unter einer "Fuchsjagd" (ARDF …)?", BE313) |
| Fuchs | fox; hidden transmitter | |
| Relaisfunkstelle / Relais / Repeater | repeater | |
| Ablage / Frequenzablage | (repeater) shift; offset | |
| Eingabefrequenz / Ausgabefrequenz | input frequency / output frequency | repeater sense |
| Baken | beacons | |
| Satellit / Amateurfunksatellit | satellite / amateur satellite | |
| Transponder | transponder | |
| Uplink / Downlink | uplink / downlink | |
| Digipeater | digipeater | |
| Linkstrecke | link | |
| Crossband-Betrieb | crossband operation | |
| Doppeln | doubling | two stations transmitting at once |
| Notfunk / Notfunkverkehr | emergency communications | |
| Nachrichtenverkehr | message handling; traffic | |
| Naturkatastrophen | natural disasters | |
| Notfall / Notmeldung / Notruf | emergency / distress message / distress call | |
| Hilfeleistung | assistance | |
| QSL-Karte | QSL card | |
| QSL-Vermittlung / QSL-Büro | QSL bureau | |
| Logbuch / Stationstagebuch | log / station log | "Stationstagebuch und QSL-Karten" → "Station log and QSL cards" |
| Hörerkennzeichen / SWL | short-wave listener identifier / SWL | |
| Diplom | award | operating awards, not diplomas |
| Bandanfang / Bandende / Bandmitte | bottom of the band / top of the band / middle of the band | BC204 |
| Europaverkehr | contacts within Europe | BC202, BC203 |
| Nachbarort | neighbouring town | BC214–BC222 |
| Schmalband-FM (Narrow FM) | narrowband FM | the bracket only repeats the English and is dropped (BC216, BE407) |
| schmalbandige digitale Übertragungsverfahren | narrowband digital modes | IARU band plan (BC214, BC219–BC222) |
| Gebetempo / Einheitstempo | sending speed / standard speed | Morse (BE117, BE118); WPM, CPM unchanged |
| Fieldday-Contest | Field Day contest | BE116 |
| Full-Duplex-Betrieb | full-duplex operation | BE116 |
| Aufruf weiterer Stationen | inviting further stations to call | QRZ? in pile-ups (BE115) |
| Standortkenner | grid locator | the English alternative name of the Maidenhead locator (BE111) |
| Kurzformel (RST) | short code | BE201 |
| Empfangsrapport | reception report | BE207–BE209 |
| Anzeigeinstrument / Zeigerausschlag | meter / needle deflection | BE204–BE206 |
| Tonhöhe / Signalqualität | pitch / signal quality | distractors beside *Tonqualität* → tone (BE203) |
| Funkpeilwettbewerb / Peilempfänger / Kleinsender | radio direction-finding competition / direction-finding receiver / small transmitter | BE313 |
| Peilzwecke | direction-finding purposes | BD109 |
| Aktivitätswoche | activity week | BE312 |
| begehrte Station / seltene Station | sought-after station / rare station | BE306, BE307, BE309 |
| Split-Verkehr | split operation | as *Split-Betrieb* (BE308) |
| Sprint-Contest | sprint contest | BE304 |
| Wertung (Contest) / gewertet werden | score / count | BE303, BE304 |
| Amateurfunkzeitschriften | amateur radio magazines | BE307 |
| Auftastton | tone burst | 1750 Hz (BE101, BE404) |
| Tonruf | tone call | BE401 |
| Sendezeitbegrenzer | time-out timer | BE405 |
| Sprachspeicher (Relaisfunkstelle) | voice memory | BE406 |
| ordentliche Übergabe | proper handover | BE405 |
| sich hereinmelden (in eine Funkrunde) | join (a net) | BE404 |
| Mobil- und Portabelstationen | mobile and portable stations | BE406 |
| Internationales Bakenprojekt (IBP) | International Beacon Project (IBP) | BE410 |
| Bakensender | beacon transmitter | BE416 |
| Umsetzer (an Bord eines Satelliten) | converter | BE416, as §8 *Umsetzer* |
| Zeitzeichen- und Normalfrequenzaussendungen | standard-frequency and time-signal transmissions | RR term order (BE410) |
| Aktivitätszentrum für Notfunkverkehr | centre of activity for emergency communications | IARU (BF109) |
| Notfunkmeldung | emergency message | BF108; *Notmeldung* stays *distress message* |
| Hilfeleistungsorganisation / Rettungsorganisation | relief organisation / rescue organisation | BF106, BF108 |
| Ersthelfer / Unfallstelle | first-aider / scene of the accident | BF103 |
| Mobiltelefonnetz | mobile phone network | BF103 |
| Notzeichen | distress signals | BF101, BF103; German "Mayday" → MAYDAY, as §13 |
| Logbuch-Upload / elektronische QSL-Karte | log upload / electronic QSL card | BG111 |
| Papierlogbuch / Computer-Logbuch / Logbuchsoftware | paper log / computer log / logging software | BG102, BG103 |
| Funkwetter | propagation conditions | BG105 |
| Amateurfunkrunde | amateur radio net | BG104 |
| ortsgebundene Funkwettbewerbe | fixed-location radio contests | BG104 |
| Uhrzeit / Zeitpunkt | time | |
| Ortsdatum / Ortszeit | local date / local time | |
| koordinierte Weltzeit (UTC) | Coordinated Universal Time (UTC) | |
| Mitteleuropäische Zeit (MEZ) | Central European Time (CET) | |
| Mitteleuropäische Sommerzeit (MESZ) | Central European Summer Time (CEST) | |
| Maidenhead-Locator / Locator | Maidenhead locator / locator | |
| Field / Square / Subsquare | field / square / subsquare | |
| Großkreis / kurzer Weg / langer Weg | great circle / short path / long path | |
| Azimut / Elevation | azimuth / elevation | |
| Rotor / Rotorsteuerung | rotator / rotator controller | British *rotator* |
| Beam-Karte | great-circle map (beam heading map) | |
| Wasserfalldiagramm / Wasserfall-Darstellung | waterfall display | |
| Amplitudenspektrum | (amplitude) spectrum display | |
| Mikrofon | microphone | |
| PTT | PTT | |
| VOX | VOX | |
| Skimmer / Reverse Beacon Network | skimmer / Reverse Beacon Network | |
| Hotspot | hotspot | |
| Sprechgruppe / Talkgroup | talkgroup | |
| CB-Funk | CB radio | |
| Deutschland | Germany | |
| Österreich / Schweiz | Austria / Switzerland | |
| Niederlande / Belgien | the Netherlands / Belgium | |
| Dänemark / Schweden / Polen / Spanien | Denmark / Sweden / Poland / Spain | |
| Kanada / Australien / Brasilien | Canada / Australia / Brazil | |
| Vereinigte Staaten von Amerika (USA) | United States of America (USA); the USA | |
| Frankreich / Italien / Luxemburg / Finnland / Schottland / Israel | France / Italy / Luxembourg / Finland / Scotland / Israel | |
| Slowakei / Slowenien / Tschechien | Slovakia / Slovenia / the Czech Republic | |
| China / Japan / Indien / Südkorea / Taiwan | China / Japan / India / South Korea / Taiwan | |
| Neuseeland / Argentinien | New Zealand / Argentina | |
| Ausland / im Ausland | abroad | |

## 3. Electrical basics, quantities and mathematics

| German | English | Note |
|---|---|---|
| Größe (physikalische) | quantity | not "size" |
| Größen und Einheiten | quantities and units | |
| Einheit | unit | |
| Einheitenvorsatz | unit prefix | |
| Zehnerpotenz | power of ten | |
| Wert / Betrag | value / magnitude | |
| Bezugsgröße / Bezug | reference quantity / reference | |
| Formel / Formelsammlung | formula / formula sheet | |
| gegeben / gesucht | given / required (to find) | worked-solution labels |
| Lösungsweg | solution; method | |
| Kehrwert | reciprocal | |
| Verhältnis | ratio | |
| Faktor | factor | |
| Prozentsatz | percentage | |
| Logarithmus (dekadisch / natürlich) | logarithm (common / natural) | |
| Dezibel (dB) / Bel | decibel (dB) / bel | |
| Pegel | level | |
| Binäres Zahlensystem / Dualsystem | binary number system | |
| Dualzahl / Binärzahl | binary number | |
| Dezimalsystem / Dezimalzahl | decimal system / decimal number | |
| Stellenwert | place value | |
| Ladung / Elektrizitätsmenge | charge / quantity of electricity | |
| Ladungsträger | charge carrier | |
| Elektronen | electrons | |
| Spannung | voltage | RSGB uses *voltage*; *potential difference* only where the German says Potentialdifferenz |
| Strom / Stromstärke | current | trap: *Strom* in "Stromversorgung" = power (supply) |
| Gleichstrom / Wechselstrom | direct current (DC) / alternating current (AC) | |
| Gleichspannung / Wechselspannung | DC voltage / AC voltage | |
| Widerstand (Größe) | resistance | trap: the component is a *resistor*, see §4 |
| Gleichstromwiderstand / ohmscher Widerstand | DC resistance / ohmic resistance | AC203 |
| Wechselstromwiderstand | impedance; AC resistance | "impedance" for an ideal C or L (EC202, EC303); "AC resistance" where the German contrasts it with *Gleichstromwiderstand* (AC203) |
| induktiver Widerstand | inductive reactance | |
| Leitwert | conductance | |
| Leistung | power | |
| Energie / Arbeit | energy / work | |
| Wattstunde / Kilowattstunde | watt-hour / kilowatt-hour | |
| Amperestunde (Ah) | ampere-hour (Ah) | |
| Amperesekunde (As) | ampere-second (As) | |
| Coulomb / Joule / Watt / Volt / Ampere / Ohm / Farad / Henry / Hertz | coulomb / joule / watt / volt / ampere / ohm / farad / henry / hertz | lower case as unit names |
| Ohmsches Gesetz | Ohm's law | |
| Proportionalitätsfaktor | constant of proportionality | |
| Stromkreis | circuit | "Der Stromkreis" → "The circuit" |
| technische / physikalische Stromrichtung | conventional current flow / electron flow | |
| Verbraucher | load | not "consumer" |
| Leiter | conductor | |
| Nichtleiter / Isolator | non-conductor / insulator | trap: English *isolator* is a switch or a microwave device |
| Halbleiter | semiconductor | |
| Leitfähigkeit | conductivity | |
| spezifischer Widerstand | resistivity | |
| Querschnitt | cross-sectional area | |
| Temperaturkoeffizient | temperature coefficient | |
| Raumtemperatur | room temperature | |
| Kupfer / Aluminium / Silizium / Germanium | copper / aluminium / silicon / germanium | British *aluminium*; *silicon* not *silicone* |
| Silber / Gold / Zinn / Zink / Wolfram / Chrom / Eisen / Messing / Bronze | silver / gold / tin / zinc / tungsten / chromium / iron / brass / bronze | trap: *Wolfram* is *tungsten* |
| Porzellan / Polyethylen / Polystyrol / Polyvinylchlorid / Polytetrafluorethylen / Kork | porcelain / polyethylene / polystyrene / polyvinyl chloride / polytetrafluoroethylene / cork | |
| Bor / Phosphor / Bismut / Tellur | boron / phosphorus / bismuth / tellurium | |
| Spannungsquelle / Stromquelle | voltage source / current source | |
| Strom- und Spannungsquellen | current and voltage sources | |
| Konstantstromquelle | constant-current source | |
| Ersatzschaltbild | equivalent circuit | |
| Innenwiderstand | internal resistance | |
| Leerlauf / Leerlaufspannung | open circuit / open-circuit voltage | |
| Klemmenspannung | terminal voltage | |
| Kurzschluss / Kurzschlussstrom | short circuit / short-circuit current | |
| Leistungsanpassung / Spannungsanpassung / Stromanpassung | power matching / voltage matching / current matching | |
| Pluspol / Minuspol | positive terminal / negative terminal | |
| Klemme | terminal | |
| Batterie / Akku (Akkumulator) | battery / rechargeable battery | |
| Nennkapazität (Akku) | rated capacity | |
| Solarzelle / Photovoltaikmodul | solar cell / photovoltaic (PV) module | |
| Feld | field | |
| elektrisches Feld | electric field | "Elektrisches Feld" → "Electric field" |
| magnetisches Feld / Magnetfeld | magnetic field | |
| elektromagnetisches Feld | electromagnetic field | |
| Feldstärke | field strength | |
| Feldlinien | field lines | |
| homogenes Feld | uniform field | |
| E-Feldkomponente / H-Feldkomponente | E-field component / H-field component | |
| Dielektrikum | dielectric | |
| Durchschlagsfestigkeit | dielectric strength | |
| Induktion | induction | |
| Gegeninduktion | mutual induction | |
| Stromdichte | current density | |
| Momentaufnahme | snapshot | |
| Ausbreitungsrichtung | direction of propagation | |
| Ausbreitungsgeschwindigkeit | velocity of propagation | |
| Lichtgeschwindigkeit | speed of light | |
| Freiraum | free space | |
| Feldwellenwiderstand (des Freiraums) | impedance of free space | 377 Ω |
| Wellenwiderstand (eines Mediums) | wave impedance (of the medium) | AK102; for a line *Wellenwiderstand* stays *characteristic impedance* (§9) |
| Schwingung | oscillation | |
| Sinusförmige Signale / Nichtsinusförmige Signale | sinusoidal signals / non-sinusoidal signals | |
| Sinusschwingung / Rechteck- / Dreieck- / Sägezahnschwingung | sine wave / square wave / triangular wave / sawtooth wave | |
| Rechtecksignal | square-wave signal | |
| Amplitude | amplitude | |
| Periode / Periodendauer | period | |
| Frequenz | frequency | |
| Kreisfrequenz | angular frequency | |
| Wellenlänge | wavelength | |
| Halbwelle | half cycle | not "half wave" for a sine wave; *half-wave* for antennas and rectifiers |
| Phase / Phasenwinkel / Phasenverschiebung | phase / phase angle / phase shift (phase difference) | |
| gleichphasig / gegenphasig | in phase / in antiphase | |
| Spitzenwert / Scheitelwert | peak value | |
| Spitze-Spitze-Wert | peak-to-peak value | |
| Effektivwert | RMS value | *root-mean-square* |
| Mittelwert | mean (average) value | |
| Augenblickswert | instantaneous value | |
| Grundschwingung / Grundfrequenz | fundamental / fundamental frequency | |
| Harmonische | harmonic | |
| Oberschwingung / Oberwelle | harmonic | trap: the German *n-te Oberwelle* is the *(n+1)th harmonic* (AB402: "third Oberwelle" = fourth harmonic). Where the German contrasts the two words, write "the third overtone (Oberwelle)" vs "the fourth harmonic" |
| Oberschwingungsanteil / Oberwellenanteil | harmonic content | |
| Vielfache (ganzzahlige) | (integer) multiples | |
| Teile (einer Frequenz) / Unterschwingungen | submultiples (of a frequency) / subharmonics | AB401, AB403 |
| Wirkleistung / Blindleistung / Scheinleistung | real (active) power / reactive power / apparent power | |
| Gleichstromverstärkung / Stromverstärkung | DC current gain / current gain | transistor |
| Verlustleistung | power dissipation; power loss | |
| Wirkungsgrad | efficiency | |
| Wärme | heat | |
| Zeitkonstante | time constant | |
| eingeschwungener Zustand | steady state | |
| Schwebung | beat | |

## 4. Components

| German | English | Note |
|---|---|---|
| Bauteil / Bauelement | component | |
| Schaltzeichen | circuit symbol | |
| Schaltplan / Schaltbild | circuit diagram | British; not "schematic" in formal text |
| Widerstand (Bauteil) | resistor | trap: the quantity is *resistance* |
| Widerstandswert | resistance value | |
| Farbring / Farbcode | colour band / colour code | British *colour* |
| Toleranz | tolerance | |
| Normreihe (E-Reihe) | preferred-value series (E series) | |
| Belastbarkeit / Nennleistung | power rating | |
| Einzelbelastbarkeit | individual power rating | ED107 |
| Strombelastbarkeit | current rating | AD325 (inductor of a bias tee) |
| Belastungsnennwert | power rating | EB514 |
| Drahtwiderstand | wirewound resistor | |
| Hochlastwiderstand / Präzisionswiderstand | high-power resistor / precision resistor | |
| induktionsarm | low-inductance | |
| gewendelt / ungewendelt (Schichtwiderstand) | spiral-cut / without a spiral cut | film resistors trimmed with a helical groove; matters for dummy loads (EC106, EC107) |
| Kennzeichnung (SMD-Widerstand) | marking | "mit der Kennzeichnung 223" → "marked 223" |
| Kohleschichtwiderstand | carbon-film resistor | |
| Metallschichtwiderstand | metal-film resistor | |
| Metalloxidschichtwiderstand | metal-oxide resistor | |
| SMD-Widerstand | SMD resistor (surface-mount) | |
| Potentiometer | potentiometer | |
| Trimmer / Trimmpotentiometer | preset (trimmer) | |
| Kaltleiter (PTC) | PTC thermistor | |
| Heißleiter (NTC) | NTC thermistor | |
| LDR (Fotowiderstand) | light-dependent resistor (LDR) | |
| VDR (Varistor) | varistor (VDR) | |
| Lastwiderstand | load resistor | |
| Vorwiderstand | series resistor; dropping resistor | for meters: *multiplier* |
| Kondensator | capacitor | |
| Kapazität | capacitance | trap: also "capacity" of a battery (Ah) |
| Plattenkondensator | parallel-plate capacitor | |
| Elektrolytkondensator (Elko) | electrolytic capacitor | |
| Keramikkondensator / Folienkondensator / Luftkondensator | ceramic / film / air-spaced capacitor | |
| Aluminium- / Tantal-Elektrolytkondensator | aluminium / tantalum electrolytic capacitor | |
| Drehkondensator | variable capacitor | |
| Styroflexkondensator | polystyrene (Styroflex) capacitor | |
| Plattenabstand / Plattenfläche | plate spacing / plate area | |
| Dielektrizitätszahl / Dielektrizitätskonstante | relative permittivity / permittivity (dielectric constant) | |
| Kondensatorgüte / Spulengüte | Q of the capacitor / Q of the inductor | |
| Verlustfaktor | dissipation factor; loss tangent (tan δ) | |
| Spannungsfestigkeit | voltage rating | |
| Metallbeläge (Kondensator) | metal foils (electrodes) | wound capacitors |
| Spule | inductor; coil | *inductor* for the component, *coil* for the physical winding |
| Induktivität | inductance | |
| Windung / Windungszahl | turn / number of turns | |
| Wicklung | winding | |
| Kern / Eisenkern / Ferritkern / Ringkern | core / iron core / ferrite core / toroidal core (toroid) | |
| Luftspule | air-cored inductor | |
| Wickellänge | winding length | |
| Abschirmbecher | screening can | |
| Eigeninduktivität | self-inductance | parasitic inductance of a component |
| Induktivitätskonstante (A_L-Wert) | inductance factor (A_L value) | |
| Drossel / HF-Drossel | choke / RF choke | |
| Übertrager | transformer; signal transformer | where the German contrasts it with *Transformator*: *signal transformer* vs *power transformer* ("Übertrager und Transformatoren" → "Signal and power transformers") |
| Transformator | transformer; power transformer | |
| Primärwicklung / Sekundärwicklung | primary winding / secondary winding | |
| Übersetzungsverhältnis ($ü$) | transformation ratio | the symbol $ü$ stays; as the bank renders *Transformationsverhältnis* for the same ratio (EC401, AD303, AD304), which the course text calls *Übersetzungsverhältnis* (uebertrager_1, gleichrichter_2) |
| Windungsverhältnis / Windungszahlenverhältnis | turns ratio | AC305, AC306, AD306 |
| Transformationsverhältnis | transformation ratio | |
| Autotransformator / Spartransformator | autotransformer | |
| Mittelanzapfung / Anzapfung | centre tap / tap | British *centre* |
| Diode | diode | |
| Halbleiterdiode | semiconductor diode | |
| PN-Übergang / Grenzschicht | PN junction / junction | where the text speaks of the *Grenzschicht* growing or shrinking with the reverse voltage (varactor diode: oszillator_vco, schwingkreis_2 slides), it is the depletion layer at the junction → *depletion layer*, as *Sperrschicht* |
| Sperrschicht | depletion layer | |
| Verarmungszone | depletion region | AB109; kept apart from *Sperrschicht* (depletion layer) because the German uses a different word |
| N-Seite / P-Seite (N-Teil / P-Teil) | N-type side / P-type side | |
| Dotierung | doping | |
| Dotierungsatome / Fremdatome | dopant atoms / foreign (impurity) atoms | |
| N-leitend / P-leitend (Halbleitermaterial) | N-type / P-type (semiconductor material) | |
| Elektronenlöcher / Löcher | holes | |
| Atommangel / Überschuss (Elektronen) | deficiency / excess (of electrons) | holes / free electrons |
| Anode / Kathode | anode / cathode | |
| Durchlassrichtung / Sperrrichtung | forward direction (forward bias) / reverse direction (reverse bias) | |
| Durchlassspannung / Flussspannung | forward voltage | |
| Sperrspannung | reverse voltage | |
| Durchbruchspannung | breakdown voltage | |
| Schwellspannung | threshold voltage | diode |
| Kennlinie | characteristic (curve) | |
| Siliziumdiode / Germaniumdiode / Schottkydiode | silicon diode / germanium diode / Schottky diode | |
| Z-Diode / Zenerdiode | Zener diode | |
| Kapazitätsdiode | varactor (variable-capacitance diode) | |
| Varicap | varicap | "Kapazitätsdiode (Varicap)" → "varactor diode (varicap)" |
| Freilaufdiode | freewheeling diode | |
| Fotodiode / Optokoppler | photodiode / optocoupler | |
| Leuchtdiode (LED) | light-emitting diode (LED) | |
| Gleichrichterdiode | rectifier diode | |
| Transistor | transistor | |
| Bipolartransistor | bipolar transistor (BJT) | |
| NPN / PNP | NPN / PNP | |
| Basis / Emitter / Kollektor | base / emitter / collector | |
| n-dotiert / p-dotiert | n-doped / p-doped | lower case as in the German |
| Basisstrom / Kollektorstrom | base current / collector current | |
| Basis-Emitter-Spannung | base-emitter voltage | |
| Feldeffekttransistor (FET) | field-effect transistor (FET) | |
| Sperrschicht-FET (N-Kanal / P-Kanal) | junction FET (JFET), N-channel / P-channel | |
| MOSFET / LDMOS | MOSFET / LDMOS | |
| Power-MOS-FET / Dual-Gate-MOS-FET | power MOSFET / dual-gate MOSFET | |
| Gate / Source / Drain | gate / source / drain | |
| Drainstrom / Gate-Source-Spannung | drain current / gate-source voltage | |
| selbstsperrend / selbstleitend | enhancement-mode / depletion-mode | trap: literal "self-blocking" is wrong |
| Massepotential | chassis potential; 0 V (common) | |
| Integrierte Schaltkreise (IC) | integrated circuits (ICs) | |
| Halbleitersubstrat | semiconductor substrate | |
| vergossene Schaltung | potted circuit | |
| Operationsverstärker | operational amplifier (op-amp) | |
| MMIC | MMIC (monolithic microwave integrated circuit) | |
| Spannungsregler (linear) / Festspannungsregler | (linear) voltage regulator / fixed voltage regulator | |
| Quarz | crystal | *quartz crystal* only for the material |
| Röhre / Elektronenröhre | valve (thermionic valve) | British *valve*, not *tube* |
| Gasentladungsröhre / Gasableiter | gas discharge tube (GDT) | fixed English name; *tube* here |
| Relais (Bauteil) | relay | trap: *Relais* in operating = repeater |
| Schalter | switch | |
| Sicherung | fuse | |
| Feinsicherung / Schmelzsicherung | miniature fuse / fuse | |
| Kühlkörper | heatsink | |
| Gehäuse / Metallgehäuse / Kunststoffgehäuse | case; enclosure / metal case / plastic case | |
| Leiterplatte | printed circuit board (PCB) | |
| Lampe / Leuchtmittel | lamp / lamp (light source) | |
| Lautsprecher / Kopfhörer | loudspeaker / headphones | |
| Steckverbinder | connector | |
| Stecker / Buchse | plug / socket | |
| BNC / N / SMA / PL-259 / SO-239 | BNC / N / SMA / PL-259 / SO-239 | unchanged |
| Masse (Schaltzeichen) | chassis | trap: in symbol questions *Masse* and *Erde* are separate answers → *chassis* vs *earth* |
| Erde (Schaltzeichen) | earth | |
| Antenne (Schaltzeichen) | antenna | |

## 5. Circuits

| German | English | Note |
|---|---|---|
| Schaltung | circuit | |
| Reihenschaltung / Serienschaltung | series connection; series circuit | |
| Parallelschaltung | parallel connection; parallel circuit | |
| Reihen- und Parallelschaltung | series and parallel connection | |
| Gesamtwiderstand / Gesamtkapazität | total resistance / total capacitance | |
| Spannungsteiler (belastet / unbelastet) | potential divider (loaded / unloaded) | British *potential divider*; *voltage divider* also understood |
| Teilspannung | partial voltage | the voltage across one resistor of a divider (ED103) |
| Brückenschaltung / Wheatstone-Brücke | bridge circuit / Wheatstone bridge | |
| Brückenzweig | bridge diagonal | the branch between the two dividers, where the meter sits |
| Blindwiderstand | reactance | |
| induktiver / kapazitiver Blindwiderstand | inductive / capacitive reactance | |
| Wirkwiderstand | resistance (resistive part) | |
| Scheinwiderstand / Impedanz | impedance | |
| Blindanteil / Wirkanteil | reactive part / resistive (real) part | |
| Verlustwiderstand | loss resistance | |
| Schwingkreis | tuned circuit; resonant circuit | RSGB: *tuned circuit* |
| Reihenschwingkreis | series tuned circuit | |
| Parallelschwingkreis | parallel tuned circuit | |
| Schwingkreise und Filter | tuned circuits and filters | |
| Resonanz / Resonanzfrequenz | resonance / resonant frequency | |
| Resonanzkurve | resonance curve | |
| Übertragungskurve | response curve | band-pass filter curves (AD227, AD228) |
| Impedanzfrequenzgang | impedance-versus-frequency response | ED205, ED206 |
| Höcker- / Sattelspannung | peak / dip voltage | ripple of an over-coupled band-pass filter: "Welligkeit von 3 dB (Höcker- zu Sattelspannung)" → "a ripple of 3 dB (peak-to-dip voltage)" (AD229) |
| Güte / Gütefaktor | Q factor; Q | |
| Bandbreite | bandwidth | |
| Grenzfrequenz | cut-off frequency | |
| Filter | filter | |
| Tiefpass / Tiefpassfilter | low-pass filter | |
| Hochpass / Hochpassfilter | high-pass filter | |
| Bandpass / Bandpassfilter / Bandfilter | band-pass filter | |
| Bandsperre / Bandstoppfilter | band-stop filter | |
| Sperrkreis | rejector (parallel-resonant trap) | RSGB *rejector circuit*; in antennas: *trap* |
| Saugkreis | acceptor (series-resonant trap) | RSGB *acceptor circuit* |
| Notchfilter / Kerbfilter | notch filter | |
| Quarzfilter | crystal filter | |
| Keramikfilter | ceramic filter | |
| Oberwellenfilter | harmonic filter | |
| Pi-Filter / Collins-Filter | pi network (pi filter) | |
| Filtercharakteristik / Flankensteilheit | filter response / skirt steepness (roll-off) | |
| Durchlassdämpfung | passband loss (insertion loss) | |
| Diplexer | diplexer | |
| Kopplung (lose / kritisch / überkritisch) | coupling (loose / critical / over-critical) | |
| Koppelkondensator | coupling capacitor | |
| Wechselstromkopplung / Gleichspannungsentkopplung | AC coupling / DC blocking | AD412 |
| Abblockkondensator / Entkoppelkondensator | decoupling capacitor; bypass capacitor | |
| Strom- und Spannungsversorgung | power supplies | catalogue heading |
| Stromversorgung / Spannungsversorgung | power supply | |
| Netzteil / Netzgerät | (mains) power supply unit (PSU) | |
| Steckernetzteil | plug-in power supply (wall adaptor) | |
| Schaltnetzteil | switch-mode power supply (SMPS) | |
| linear geregeltes Netzteil | linear (regulated) power supply | |
| Gleichrichter / Gleichrichtung | rectifier / rectification | |
| Einweggleichrichter | half-wave rectifier | |
| Vollweggleichrichter (Mittelpunktschaltung) | full-wave (centre-tap) rectifier | |
| Brückengleichrichter | bridge rectifier | |
| Ladekondensator | reservoir capacitor | RSGB term |
| Siebkondensator / Glättungskondensator | smoothing capacitor | |
| Siebung / Siebglied | smoothing / smoothing filter | |
| Brummspannung / Restwelligkeit | ripple voltage / ripple | |
| Spannungsstabilisierung | voltage stabilisation | |
| Stabilisierungsschaltung (mit Z-Diode) | (Zener) stabiliser circuit | |
| Spannungserhöhung | voltage step-up | |
| Längstransistor | series pass transistor | |
| Spannungswandler / DC/DC-Wandler | DC–DC converter | |
| Step-Up-Wandler / Step-Down-Wandler | boost converter / buck converter | |
| Schaltfrequenz | switching frequency | |
| Fernspeiseweiche / Bias-T | bias tee | |
| Spannungskonstanz | voltage stability | of a DC source under load (ED301) |
| Brummfrequenz | hum frequency | ripple frequency at a PSU output (AD309); *Restwelligkeit* stays *ripple* |
| Überspannungsableiter | surge arrester | |
| Unterbrechungsfreie Spannungsversorgung (USV) | uninterruptible power supply (UPS) | AF708 |
| galvanische Trennung | galvanic isolation | |
| Versorgungsspannung / Betriebsspannung | supply voltage / operating voltage | |
| Verstärker | amplifier | |
| Verstärkung / Verstärkungsfaktor | gain / gain factor | |
| Spannungsverstärkung / Leistungsverstärkung | voltage gain / power gain | |
| Emitterschaltung | common-emitter circuit | |
| Kollektorschaltung (Emitterfolger) | common-collector circuit (emitter follower) | |
| Basisschaltung | common-base circuit | |
| Sourceschaltung / Drainschaltung / Gateschaltung | common-source / common-drain / common-gate circuit | |
| Arbeitspunkt / Arbeitspunkteinstellung | operating point (bias point) / biasing | |
| Arbeitswiderstand | load resistance | collector/drain load (AF422) |
| Basisspannungsteiler | base potential divider | |
| Emitterwiderstand | emitter resistor | |
| Basisvorspannung / Vorspannung | base bias / bias | |
| Ruhestrom | quiescent current | |
| A-Betrieb / B-Betrieb / AB-Betrieb / C-Betrieb | class A / class B / class AB / class C operation | |
| Gegentaktschaltung / Gegentaktendstufe | push-pull circuit / push-pull output stage | |
| Gegenkopplung / Mitkopplung / Rückkopplung | negative feedback / positive feedback / feedback | |
| Phasenumkehrstufe | phase inverter stage | |
| Stromgegenkopplung / Spannungsgegenkopplung | negative current feedback / negative voltage feedback | |
| Eingangsimpedanz / Ausgangsimpedanz | input impedance / output impedance | |
| Eingangswiderstand / Ausgangswiderstand | input resistance / output resistance | |
| Eingang / Ausgang | input / output | |
| Eingangssignal / Ausgangssignal | input signal / output signal | |
| Treiberstufe | driver stage | |
| Stufe | stage | |
| Verzerrung | distortion | |
| Übersteuerung | overdriving; overload | |
| Begrenzung / Begrenzer | limiting / limiter | |
| Linearität / linear | linearity / linear | |
| Eigenschwingungen / wilde Schwingungen / parasitäre Schwingungen | self-oscillation / parasitic oscillations | |
| Schwingungseinsatz | start of oscillation | AF409 |
| Oszillator | oscillator | |
| Schwingungserzeuger | generator of oscillations | ND201, ED501, ED506; kept apart from *signal generator* (*Messsender*) |
| Schwingbedingung | condition for oscillation | |
| ungedämpfte Schwingungen | sustained (undamped) oscillations | AD613 |
| Schleifenverstärkung | loop gain | |
| Audion / Audionschaltung | regenerative detector (audion) | AD616 |
| Tongenerator | tone generator | |
| Dreipunktschaltung (Colpitts / Hartley) | three-point oscillator (Colpitts / Hartley) | |
| LC-Oszillator | LC oscillator | |
| Quarzoszillator | crystal oscillator | |
| VFO / VCO | VFO (variable-frequency oscillator) / VCO (voltage-controlled oscillator) | |
| XO / TCXO / OCXO / GPSDO | XO / TCXO / OCXO / GPSDO | |
| Frequenzstabilität / Langzeitstabilität | frequency stability / long-term stability | |
| Phasenregelkreis / Phasenregelschleife (PLL) | phase-locked loop (PLL) | |
| Phasenvergleicher | phase detector (phase comparator) | |
| Schleifenfilter | loop filter | |
| Frequenzteiler / Teiler | frequency divider / divider | |
| Teilerverhältnis | division ratio | PLL divider (AD704) |
| Frequenzsynthesizer | frequency synthesiser | British *-ise* |
| Regelschleife | control loop | AD702 |
| Quarzgenerator | crystal oscillator | AD705 |
| Referenzsignal / Referenzoszillator | reference signal / reference oscillator | |
| eingerastet | locked | |
| Direkte Digitale Synthese (DDS) | direct digital synthesis (DDS) | |
| Phasenakkumulator | phase accumulator | |
| Frequenzvervielfacher / Vervielfacher | frequency multiplier / multiplier | |
| Verachtfacher / Vervielfachungskombination | eight-times multiplier / sequence of multipliers | AF301, AF314; *eight-times* in words, as the German has no digit |
| Dämpfungsglied | attenuator | |
| symmetrisches Dämpfungsglied | symmetrical attenuator | equal input and output impedance (AD805, AD806); trap: not *balanced*, which is *symmetrisch* for feeders (§9) |
| Dämpfung | attenuation; loss | *damping* only for oscillations |
| Modulator / Demodulator | modulator / demodulator | |
| Mischer / Mischstufe | mixer / mixer stage | |
| Abwärtsmischer | down-converter | "PLL-Abwärtsmischer" → "PLL down-converter" (AD505) |
| Mischprodukt / Mischung | mixing product / mixing | |
| Balancemischer / Ringmischer | balanced mixer / ring mixer (double-balanced mixer) | |
| Eintakt-Transistormischer / Dualtransistormischer | single-ended transistor mixer / dual-transistor mixer | AF213, AF214 |
| Treiber | driver | |
| Pufferstufe | buffer stage | |

## 6. Receivers and transmitters

| German | English | Note |
|---|---|---|
| Sender | transmitter | |
| Empfänger | receiver | |
| Transceiver / Sendeempfänger | transceiver | |
| Sender und Empfänger | transmitters and receivers | catalogue heading |
| Empfängerstufen / Senderstufen | receiver stages / transmitter stages | |
| Blockschaltbild / Blockdiagramm | block diagram | |
| Baugruppe / Block | module; block | |
| Geradeausempfänger | tuned radio frequency (TRF) receiver | |
| Detektorempfänger | crystal set | |
| Direktüberlagerungsempfänger / Direktmischer | direct-conversion receiver | |
| digitaler Direktempfänger | digital direct-sampling receiver | AF620 |
| Empfangszweig / Sendezweig | receive path / transmit path | |
| Durchlasskurve | passband curve | AF207 |
| Antennenvorverstärker | antenna preamplifier | |
| Überlagerungsempfänger / Superhet | superheterodyne receiver (superhet) | |
| Einfachsuper / Doppelsuper | single-conversion superhet / double-conversion superhet | |
| Zwischenfrequenz (ZF) | intermediate frequency (IF) | |
| ZF-Verstärker / ZF-Filter | IF amplifier / IF filter | |
| Spiegelfrequenz | image frequency | |
| Spiegelfrequenzunterdrückung | image rejection | |
| Trennschärfe / Selektivität | selectivity | |
| Nahselektion | close-in selectivity | |
| Spiegelselektion | image rejection | same as *Spiegelfrequenzunterdrückung* (AF113) |
| Kanalabstand / Kanalraster | channel spacing | "im 12,5 kHz Kanalraster" → "with 12.5 kHz channel spacing" (AE310) |
| Nachbarkanalstörungen | adjacent-channel interference | |
| Begrenzerverstärker | limiting amplifier (limiter) | FM receiver (AF226) |
| Vorstufenrauschen | noise of the input stage | |
| Empfängerstummschaltung | receiver muting (squelch) | AF225 |
| Passband-Tuning | passband tuning | |
| Satellitenempfangsanlage | satellite receiving system | |
| Fernspeisespannung | remote supply voltage | DC fed up the coax to an LNB (AF230); cf. *Fernspeiseweiche* → bias tee |
| Handfunkgerät | handheld transceiver (handheld) | |
| Datenanschluss (DATA, 9600-Port) | data port (9600 port) | NF115 |
| Drehwinkelgeber (Encoder) | rotary encoder | |
| Empfindlichkeit | sensitivity | |
| Grenzempfindlichkeit | minimum discernible signal (MDS) | the receiver spec, a distractor in AF221 |
| Großsignalfestigkeit | strong-signal performance (large-signal handling) | |
| Intercept-Punkt (IP3) | (third-order) intercept point (IP3) | |
| Interception Point IP$_3$ | intercept point IP$_3$ | the German's own spelling in AF221; English has only *intercept point* |
| Kreuzmodulation | cross-modulation | |
| Intermodulation | intermodulation | |
| Blocking / Zustopfen | blocking | |
| Vorverstärker | preamplifier (preamp) | |
| Vorselektion / Preselektor | preselector | |
| Roofing-Filter | roofing filter | |
| Rauschen / Eigenrauschen | noise / internal noise | |
| Rauschzahl | noise factor (linear) / noise figure (in dB) | trap: German *Rauschzahl* covers both; AF229 "Rauschzahl F = 2" is a noise factor, AF228 "Rauschzahl von 1,8 dB" a noise figure |
| Rauschmaß | noise figure (dB) | |
| Signal-Rausch-Verhältnis (SNR) | signal-to-noise ratio (SNR) | |
| Nutzsignal | wanted signal | |
| Störsignal | unwanted signal; interfering signal | |
| Produktdetektor | product detector | |
| Hüllkurvendemodulator | envelope detector | |
| Flankendiskriminator | slope detector | |
| Flankendemodulator / Flanken-Diskriminator | slope detector | same thing as *Flankendiskriminator*; a bare *Diskriminator* stays *discriminator* (AD504, AD506) |
| BFO / Hilfsträgeroszillator | beat frequency oscillator (BFO) / carrier insertion oscillator | |
| Hilfsträger / Hilfsträgererzeugung | auxiliary carrier / generating an auxiliary carrier | EF209 (the BFO's job) |
| Automatische Verstärkungsregelung (AGC / AVR) / Regelspannung | automatic gain control (AGC) / AGC voltage | |
| ALC (Automatic Level Control) | automatic level control (ALC) | |
| Pegelregelung | level control | |
| RF-Gain / HF-Verstärkungsregler | RF gain (control) | |
| Rauschsperre / Squelch | squelch | |
| Noise-Blanker / Störaustaster | noise blanker | "NF-Störaustaster" → "AF noise blanker" (EF211) |
| Rauschunterdrückung(sverfahren) (Noise Reduction) | noise reduction (NR) | DSP function (EF213) |
| Clarifier | clarifier | |
| Gleichlauf / Gleichlaufsteuerung | ganging (tracking) / ganging control | of ganged tuned circuits; EF212 "Automatische Gleichlaufsteuerung" → "Automatic ganging control" (see DECISIONS.md) |
| RIT | RIT (receiver incremental tuning) | |
| Lautstärke | volume | |
| Display / Anzeige | display | |
| NF-Verstärker | audio-frequency (AF) amplifier | NF → AF |
| HF-Verstärker | RF amplifier | HF (Hochfrequenz) → RF |
| HF-Leistungsverstärker / Leistungsverstärker (PA) | RF power amplifier / power amplifier (PA) | |
| Endstufe / Senderendstufe | output stage; power amplifier (PA) | |
| Endstufenröhre / Endstufentransistor | output valve / output transistor | AF401 |
| Ausgangsanpassschaltung / Ausgangsfilter | output matching circuit / output filter | AF403 |
| Stromzufuhr (im Sender) | power feed | EF405 |
| Wärmeleistung (in Wärme umgesetzt) | power dissipated as heat | AF427 |
| Linearverstärker / Linear-Endstufe | linear amplifier | |
| Schaltendstufe / Klasse-E-Verstärker | switching amplifier / class E amplifier | |
| Ausgangsleistung / HF-Ausgangsleistung | output power / RF output power | |
| Eingangsleistung | input power | |
| Senderausgang | transmitter output | |
| Nebenaussendungen / Nebenprodukte | spurious emissions / spurious products | RR 1.145 |
| Außerbandaussendungen | out-of-band emissions | RR 1.144 |
| Splatter | splatter | |
| Tastklicks | key clicks | |
| Chirp | chirp | |
| Mikrofonverstärker / Sprachprozessor / Kompressor | microphone amplifier / speech processor / compressor | |
| Konverter / Transverter | converter / transverter | "Konverter und Transverter" → "Converters and transverters" |
| LNB (Low Noise Block) | LNB (low-noise block downconverter) | |
| Digitale Signalverarbeitung (DSP) | digital signal processing (DSP) | |
| Signalprozessor | (digital) signal processor | |
| SDR (Software Defined Radio) | software-defined radio (SDR) | |
| CAT-Schnittstelle | CAT interface | |
| Schnittstelle | interface | |
| Computer / Rechner | computer | |
| Remote-Interface / Steuersignale | remote interface / control signals | |
| Bedienteil | control unit | the operator-side unit in remote operation (AF701) |
| Remote-Tuner | remote tuner | |
| Kontrollseite / Remoteseite | control site / remote site | AF707; not *remote end*, which is *Gegenstelle* (§8) |
| IP-Steckdose | IP-controlled mains socket | |
| Watchdog | watchdog | |

## 7. Modulation and transmission modes

| German | English | Note |
|---|---|---|
| Modulation / Modulationsverfahren / Modulationsart | modulation / modulation method / mode | *Modulationsart* on a transceiver = *mode* |
| Modulation allgemein | modulation in general | |
| Übertragungsverfahren | transmission method; mode | "Modulations- und Übertragungsverfahren" → "Modulation and transmission methods" |
| Träger / Trägerfrequenz / Trägersignal | carrier / carrier frequency / carrier signal | |
| Modulationssignal / Modulationsfrequenz | modulating signal / modulating frequency | |
| Amplitudenmodulation (AM) | amplitude modulation (AM) | |
| Modulationsgrad | modulation depth | AM; expressed in % |
| Übermodulation | overmodulation | |
| Hüllkurve / Modulationshüllkurve | envelope / modulation envelope | |
| Seitenband / oberes (USB) / unteres (LSB) | sideband / upper (USB) / lower (LSB) | |
| Einseitenbandmodulation (SSB) | single-sideband modulation (SSB) | |
| Zweiseitenband (DSB) | double sideband (DSB) | |
| Trägerunterdrückung | carrier suppression | |
| Balancemodulator | balanced modulator | |
| Seitenbandunterdrückung | sideband suppression | |
| Frequenzmodulation (FM) | frequency modulation (FM) | |
| Phasenmodulation (PM) | phase modulation (PM) | |
| Winkelmodulation | angle modulation | |
| Frequenzhub / Hub | (frequency) deviation | |
| Spitzenhub | peak deviation | |
| unterdrücktes Zweiseitenband-Trägersignal | double-sideband suppressed-carrier (DSB-SC) signal | AE206 |
| Splatter-Erscheinungen / Seitenband-Splatter | splatter / sideband splatter | |
| Einton- / Zweiton-Testsignal | single-tone / two-tone test signal | |
| Modulationsindex | modulation index | |
| Carson-Formel / Carson-Bandbreite | Carson's rule / Carson bandwidth | |
| Preemphasis / Deemphasis | pre-emphasis / de-emphasis | |
| CW (Tastfunk) / Tastung | CW / keying | |
| Spitzenleistung (PEP) / Hüllkurvenspitzenleistung | peak envelope power (PEP) | |
| mittlere Leistung | mean power | RR term *mean power* |
| Zweitonsignal | two-tone (test) signal | |
| Ein- oder Zweitonaussteuerung | single-tone or two-tone drive | PEP measurement (EF402) |
| Telefonie | telephony | |
| Amateurfernsehen (ATV) | amateur television (ATV) | |
| SSTV (Slow Scan Television) | slow-scan television (SSTV) | |
| Standbilder / bewegte Bilder | still pictures / moving pictures | |
| Polarmodulation | polar modulation | |

## 8. Digital techniques

| German | English | Note |
|---|---|---|
| Digitale Übertragungsverfahren | digital transmission methods; digital modes | catalogue heading "Digital transmission methods", parallel to its parent "Modulation and transmission methods" |
| Digimode / Digimodes | digital mode / data modes | |
| Bit / Byte / MBit | bit / byte / Mbit | |
| Datenübertragungsrate / Bitrate | data rate / bit rate | |
| Symbol / Symbolrate | symbol / symbol rate | |
| Baud | baud | |
| Datenmenge | amount of data | |
| Datenpaket / Datenstrom | data packet / data stream | |
| Umtastung | keying; shift keying | |
| Amplitudenumtastung (ASK) / On-Off-Keying | amplitude-shift keying (ASK) / on-off keying (OOK) | |
| Frequenzumtastung (FSK) / AFSK | frequency-shift keying (FSK) / AFSK | |
| Phasenumtastung (PSK) / BPSK / QPSK | phase-shift keying (PSK) / BPSK / QPSK | |
| Quadraturamplitudenmodulation (QAM) | quadrature amplitude modulation (QAM) | |
| OFDM | orthogonal frequency-division multiplexing (OFDM) | |
| Konstellationsdiagramm | constellation diagram | |
| I/Q (Inphase- / Quadraturkomponente) | I/Q (in-phase / quadrature component) | |
| Q-Anteil | Q component | |
| Mapping / Mapper | mapping / mapper | |
| Gray-Code | Gray code | |
| Intersymbolinterferenz | intersymbol interference (ISI) | |
| Shannon-Hartley-Gesetz | Shannon–Hartley theorem | |
| AWGN (weißes gaußsches Rauschen) | additive white Gaussian noise (AWGN) | |
| Kanal / Übertragungskanal | channel / transmission channel | |
| Quellencodierung / Kanalcodierung | source coding / channel coding | |
| Redundanz | redundancy | |
| Prüfbit / Paritätsbit | check bit / parity bit | |
| Paritätsprüfung | parity check | |
| Prüfsumme / Prüfsummenverfahren | checksum / checksum method | |
| Nutzdaten | user data (payload) | AE412 |
| CRC (zyklische Redundanzprüfung) | cyclic redundancy check (CRC) | |
| Vorwärtsfehlerkorrektur (FEC) | forward error correction (FEC) | |
| Fehlerkorrektur / Fehlererkennung | error correction / error detection | |
| Synchronisation | synchronisation | |
| Vielfachzugriff / TDMA / FDMA / CDMA | multiple access / TDMA / FDMA / CDMA | |
| Zeitmultiplexverfahren (TDMA) / Frequenzmultiplexverfahren (FDMA) / Codemultiplexverfahren (CDMA) | time-division / frequency-division / code-division multiple access (TDMA / FDMA / CDMA) | where the German gives the *…MA* abbreviation, expand it as the abbreviation reads (EE409–EE411); without it, *…multiplexing* (§14) |
| Spreizcodierung | spreading code(s) | CDMA (EE411) |
| Kanalstörung | channel impairment | AE422 |
| Umschaltgeschwindigkeit (zwischen Symbolen) | speed of switching (between symbols) | AE415 |
| Zeitschlitz | time slot | |
| Color Code (DMR) | colour code (DMR) | British spelling in prose; "Color Code" when quoting a DMR menu item |
| DMR / D-STAR / C4FM / FT8 / PSK31 / Olivia / RTTY | unchanged | mode names stay |
| Digital Voice (DV) | digital voice (DV) | |
| digitaler Sprechfunk / digitales Amateurfunkfernsehen (DATV) | digital voice / digital amateur television (DATV) | |
| Paketvermittlung | packet switching | |
| paketvermitteltes Netz / Paketweiterleitung | packet-switched network / packet forwarding | EE412 |
| Internetprotokoll (IP) | Internet Protocol (IP) | capitalised as a proper name, though *the internet* is lower case |
| Teilnetz / Standardgateway / Gegenstelle (IP) | subnet / default gateway / remote end (peer) | EE413; *Gegenstelle* is not *remote station*, which is the remotely controlled *Remote-Station* (§1.3) |
| Stationskennung (DMR-ID) / Reflektor | station identifier (DMR ID) / reflector | digital voice networks (NE402) |
| Netzwerk / Router / Subnetzmaske | network / router / subnet mask | |
| Internet | the internet | lower case in British usage |
| Abtastung / abtasten | sampling / sample | |
| Abtastrate / Samplingrate | sampling rate | |
| Sample / Samples | sample / samples | |
| Abtasttheorem (Nyquist) | sampling theorem (Nyquist) | |
| Aliasing / Antialiasingfilter | aliasing / anti-aliasing filter | |
| Alias-Effekt / Anti-Alias-Filter | aliasing (effect) / anti-aliasing filter | "Unter dem Alias-Effekt werden Fehler verstanden" → "The term aliasing refers to errors" (AF617) |
| Abtastratengenerator | sampling clock generator | AF620 |
| Abtastergebnis | sampled result | |
| Taktzittern (Jitter) | clock jitter | AF621 |
| Schrittweite (D/A-Umsetzer) | step size | between voltage levels (AF610, AF611) |
| Amplitudengang / Frequenzgang | amplitude response / frequency response | |
| Quantisierung | quantisation | |
| Raummultiplexing | space-division multiplexing | AF605 |
| Auflösung (Bit) | resolution | |
| Wertebereich | (value) range | |
| A/D-Umsetzer (ADC) | analogue-to-digital converter (ADC) | British *analogue* |
| D/A-Umsetzer (DAC) | digital-to-analogue converter (DAC) | |
| Umsetzer | converter | |
| Fourier-Transformation / FFT | Fourier transform / FFT | |
| Zeitbereich / Frequenzbereich | time domain / frequency domain | trap: *Frequenzbereich* in regulation = frequency range |
| Frequenzspektrum | (frequency) spectrum | |
| digitales Filter / FIR / IIR | digital filter / FIR / IIR | |
| Latenz | latency | |
| Takt / Taktgenerator | clock / clock generator | |
| FPGA | FPGA | |
| Software / Programm | software / program | computer *program*, not *programme* |

## 9. Antennas and feeders

| German | English | Note |
|---|---|---|
| Antenne | antenna | plural *antennas*; not *aerial* |
| Antennen und Übertragungsleitungen | antennas and transmission lines | catalogue heading |
| Antennenmerkmale | antenna characteristics | |
| Strahler / Strahlerelement | radiator / radiating element (driven element) | |
| Dipol / Dipol-Antenne | dipole | |
| Halbwellendipol / λ/2-Dipol | half-wave dipole | |
| mittengespeister Dipol | centre-fed dipole | |
| Faltdipol | folded dipole | |
| Viertelwellenstrahler / λ/4-Vertikalantenne | quarter-wave radiator / quarter-wave vertical | |
| Vertikalantenne | vertical antenna (vertical) | |
| Groundplane-Antenne | ground-plane antenna | fixed name; *ground* allowed here |
| Radials / Gegengewicht | radials / counterpoise | |
| Marconi-Antenne | Marconi antenna | |
| Endgespeiste Antenne (End-Fed) | end-fed antenna | |
| Langdrahtantenne | long-wire antenna | |
| Windom-Antenne | Windom antenna (off-centre-fed dipole) | |
| G5RV / W3DZZ / Zeppelin-Antenne | G5RV / W3DZZ / Zepp antenna | |
| Delta-Loop-Antenne / Quad-Antenne | delta loop / quad | |
| Cubical-Quad-Antenne | cubical quad antenna | |
| magnetische Ringantenne | magnetic loop antenna | EG105 |
| Ferritantenne / Ferritstabantenne | ferrite antenna / ferrite rod antenna | |
| Patchantenne / Schlitzantenne | patch antenna / slot antenna | |
| Sperrtopfantenne | sleeve dipole | coaxial sleeve antenna, a VHF/UHF vertical whose λ/4 sleeve (*Sperrtopf*) acts as balun/choke (EG107) |
| Winkeldipol | inverted-V dipole | EG103 |
| Schleifendipol | folded dipole | a common German synonym of *Faltdipol*; English has one term. AG423 b/d are wrong because of the 60 Ω and what the arrangement does, not because of the word |
| Ringdipol | ring dipole | AG225 |
| Saugkreis-Dipol | acceptor-circuit dipole | distractor beside *Sperrkreis-Dipol* → trap dipole (AG109) |
| Gleichwellenfilter | common-frequency filter | made-up distractor beside *Oberwellenfilter* (AG109); *Gleichwelle* is *common frequency* in English (Gleichwellenfunk → common-frequency broadcasting) |
| Dreiband-Dipol | three-band dipole | |
| Kurzwellenbeam | HF beam | |
| Magnetic-Loop-Antenne | magnetic loop (small transmitting loop) | |
| Ganzwellen-Schleifenantenne | full-wave loop | |
| Yagi-Uda-Antenne | Yagi-Uda antenna (Yagi) | |
| Richtantenne | directional antenna; beam | |
| Rundstrahler | omnidirectional antenna | |
| Kreuzyagi | crossed Yagi | |
| Direktor / Reflektor | director / reflector | |
| parasitäre Elemente | parasitic elements | |
| Boom / Boomlänge | boom / boom length | |
| Parabolantenne / Parabolspiegel | parabolic dish / parabolic reflector | |
| Offsetspiegel | offset dish | |
| rotationssymmetrischer Parabolspiegel | rotationally symmetrical parabolic dish | AG127 |
| Erreger / Erregerantenne | feed; feed antenna | |
| Hornstrahler | horn antenna | |
| Helixantenne | helical antenna (helix) | |
| Mehrbandantenne / Multibandantenne | multiband antenna | |
| Zweibandantenne | dual-band antenna | as *Zweiband-Dipol* (§14) |
| Monobandantenne | monoband antenna | |
| Trap (Sperrkreis in Antenne) | trap | |
| Verlängerungsspule | loading coil | |
| Fußpunktspule | base loading coil | |
| elektrische Verlängerung / Verkürzung | electrical lengthening / shortening | |
| Magnetfußantenne | magnetic-mount antenna (mag-mount) | |
| Isotropstrahler / Kugelstrahler / isotroper Strahler | isotropic radiator | |
| Gewinn / Antennengewinn | gain / antenna gain | |
| Gewinnfaktor | gain (as a power ratio) | VD725: "Gewinnfaktor 2,5" → "a gain of 2.5 (as a power ratio)" |
| dBi / dBd | dBi / dBd | |
| Strahlungsdiagramm / Richtdiagramm | radiation pattern | |
| Hauptkeule / Nebenkeule / Rückkeule | main lobe / side lobe / back lobe | |
| Hauptstrahlrichtung | direction of maximum radiation | |
| Vor-Rück-Verhältnis | front-to-back ratio | |
| Öffnungswinkel / Halbwertsbreite | beamwidth / half-power (-3 dB) beamwidth | "Halbwertsbreite (Öffnungswinkel)" → "half-power beamwidth (beam angle)" (AG221) |
| Horizontaldiagramm | horizontal radiation pattern | |
| Strahlungsdichte | power density | power flux density in W/m² (AG219), as in RSGB EMC/exposure texts |
| Abstrahlwinkel / Erhebungswinkel | angle of radiation; elevation angle | RSGB *take-off angle* in propagation context |
| Abstrahlung / Strahlung | radiation | |
| Polarisation (horizontal / vertikal / zirkular) | polarisation (horizontal / vertical / circular) | British *-isation* |
| rechtsdrehend / linksdrehend; rechtszirkular / linkszirkular (Polarisation) | right-hand circular / left-hand circular (polarisation) | |
| Polarisationsdrehung | polarisation rotation (Faraday rotation) | |
| Strahlungsleistung | radiated power | |
| äquivalente isotrope Strahlungsleistung (EIRP) | equivalent isotropically radiated power (EIRP) | keep "EIRP" as the German does; also for the German's shortened "äquivalente Strahlungsleistung (EIRP)" (EG503–EG505) and "gleichwertige isotrope Strahlungsleistung" (NG402) |
| effektive Strahlungsleistung (ERP) / äquivalente (effektive) Strahlungsleistung (ERP) | effective radiated power (ERP) / equivalent (effective) radiated power (ERP) | AG501 keeps the German's bracket; plain *äquivalente Strahlungsleistung (ERP)* → effective radiated power (ERP), the abbreviation decides (AK115, DECISIONS.md) |
| bezogen auf den Halbwellendipol / den isotropen Strahler | relative to the half-wave dipole / the isotropic radiator | "in einer Richtung" → "in a given direction" (RR 1.161, 1.162) |
| Antennenspeiseleitung | antenna feeder | RR "antenna transmission line" (AG501 c, d) |
| Strahlungsleistung (EIRP und ERP) | radiated power (EIRP and ERP) | catalogue heading |
| Antenneneingangsleistung | power at the antenna input | |
| Fußpunktwiderstand / Fußpunktimpedanz / Speisewiderstand | feed-point impedance (feed-point resistance) | |
| Eingangswiderstand (Antenne) | input impedance | as *Fußpunktwiderstand*: an antenna's input is reactive off resonance (AG207 "rein kapazitiver Eingangswiderstand"); EG209, EG211 |
| Speisepunkt / Einspeisepunkt | feed point | |
| Strombauch / Spannungsbauch | current maximum (antinode) / voltage maximum (antinode) | where the German pairs *Bauch* and *Knoten* (EG203–EG205): *antinode* / *node* |
| Stromknoten / Spannungsknoten | current minimum (node) / voltage minimum (node) | |
| Stromverteilung / Stromkurve | current distribution | |
| Erregung / Erregerfrequenz | excitation; feeding / operating frequency | AG203: "Erregung auf 28 MHz" → "fed at 28 MHz"; *Erregerfrequenz* → "operating frequency" (AG111–AG113, AG203–AG206), not "feed frequency", which is not English usage |
| Resonanzlänge | resonant length | |
| Verkürzungsfaktor (Antenne) | end-effect correction factor (shortening factor) | trap: for cables the same German word = *velocity factor*. In exam questions written *shortening factor* (AG101–AG105, EG202). EG201, whose correct answer defines it for a line, is the cable sense: *velocity factor* |
| Verkürzungsfaktor (Kabel) | velocity factor | |
| Übertragungsleitung / Leitung | transmission line / line | |
| Speiseleitung / Antennenleitung / Antennenkabel | feeder; feed line | RSGB *feeder* |
| Koaxialkabel / Koaxkabel | coaxial cable (coax) | |
| Innenleiter / Außenleiter (Schirm) | inner conductor / outer conductor (braid, screen) | British *screen* |
| Abschirmung | screening; shield | British *screening* |
| PE-Schaumkabel / Polyethylen / PTFE | foam polyethylene cable / polyethylene / PTFE | |
| Zweidrahtleitung / Hühnerleiter / Paralleldrahtleitung | twin feeder; open-wire feeder (ladder line) | AG311: *Zweidrahtleitung* → twin feeder; AG418: *Hühnerleiter* → ladder line; AG305, AG313: *(offene) Paralleldrahtleitung* → open-wire line |
| Stege / Spreizer (Zweidrahtleitung) | spacers | AG311, EG305 |
| Flachbandkabel | ribbon feeder | "300 Ohm-Flachbandkabel" → "300 Ω ribbon feeder" (AG416, AG417) |
| Transformationsleitung | transformer section | the λ/4 matching line (AG417, AG418), as *Transformationsstück* |
| Leitungsstück (Stub) | length of line (stub) | AG420 |
| Voll-PE / PE-Schaum / Massivschirm / Abschirmgeflecht | solid PE / foam PE / solid screen / braided screen | cable descriptions (AG302, AG308–AG310, AG307) |
| symmetrisch / unsymmetrisch | balanced / unbalanced | |
| Wellenwiderstand | characteristic impedance | |
| Kabeldämpfung / Kabelverluste | cable loss (attenuation) | |
| Kabeldämpfungsdiagramm | cable attenuation chart | |
| Leitungsende / offenes / kurzgeschlossenes Ende | end of the line / open-circuit / short-circuit end | |
| Lecherleitung | Lecher line | |
| Viertelwellen-Transformator (λ/4-Leitung) | quarter-wave transformer | |
| Verzögerungsleitung / Transformationsstück | delay line / transformer section | AG126 |
| Anpassung | matching | |
| Fehlanpassung | mismatch | |
| Anpassung, Transformation, Symmetrierung und Mantelwellen | matching, impedance transformation, balancing and common-mode currents | catalogue heading |
| Impedanztransformation | impedance transformation | |
| Symmetrierung / Symmetrierglied | balancing / balun | |
| Balun / Un-Un | balun / unun | |
| Umwegleitung | half-wave coaxial balun (delay-line balun) | where λ/2 is given or *Balun* stands beside it: "$\lambda$/2 delay line" / "half-wave delay line" (AG420, AG423, AG424) |
| Mantelwellen | common-mode currents | the "sheath waves" on the outside of the braid; RSGB *common-mode current*. *sheath currents* where the correct answer is *Gleichtaktanteile* and would echo the stem (AG425, AG426) |
| Mantelstrom | sheath current | the current on the outside of the braid (EG404, AG428) |
| Mantelwellensperre (MWS) | common-mode choke (choke balun) | keep "MWS" where the drawing label uses it |
| stromkompensierte Drossel | common-mode choke | AG426: "current-compensated choke" (literal, a current EMC term), because the correct answer is "common-mode components" |
| Spannungs-Balun | voltage balun | AG428, AG429 |
| Gleichtakt / Gegentakt | common mode / differential mode | |
| Gleichtaktanteil / Gegentaktanteil | common-mode component / differential-mode component | |
| Antennenanpassgerät / Antennentuner | antenna tuning unit (ATU); antenna tuner | RSGB *ATU* |
| Anpassglied / Anpassnetzwerk | matching network | |
| Stehwellenverhältnis (SWR, VSWR) | standing wave ratio (SWR) | |
| Reflexion / Reflexionsfaktor | reflection / reflection coefficient | |
| Rückflussdämpfung | return loss | |
| vorlaufende / rücklaufende Welle (Leistung) | forward / reflected wave (power) | |
| stehende Welle | standing wave | |
| Skineffekt | skin effect | |
| Hohlleiter | waveguide | |
| Mast / Antennenmast / Gittermast | mast / antenna mast / lattice tower | |
| Windlast | wind load | |
| Abspannung | guying (guy wires) | AF706 |
| Dachständer | roof-mounted mains overhead-line support | German distribution detail; describe as needed |
| Freileitung / Hochspannungsleitung | overhead line / high-voltage line | |

## 10. Propagation

| German | English | Note |
|---|---|---|
| Wellenausbreitung / Ausbreitung | propagation | |
| Wellenausbreitung und Ionosphäre | propagation and the ionosphere | |
| Ausbreitungsbedingungen | propagation conditions | |
| Kurzwelle (KW) | short wave; HF | "auf Kurzwelle" → "on HF"; "Kurzwellenausbreitung" → "HF propagation" |
| Kurzwellenbereich / Kurzwellenbänder | HF range / HF bands | |
| Mittelwelle / Langwelle | medium wave (MF) / long wave (LF) | |
| Ultrakurzwelle (UKW) | very high frequency (VHF) | in broadcast context "UKW-Rundfunk" → "FM broadcast (VHF)" |
| Bereichsnamen neben VHF / UHF / HF / MF: Ultrakurzwelle (UKW) / Dezimeterwelle / Kurzwelle (KW) / Mittelwelle (MW) | (dropped) / (dropped) / short wave (SW) / medium wave (MW) | where the German pairs the English band name with the German one (BC101–BC106): the German name only repeats the English one and is dropped, as in the bracket rule — "Very High Frequency (VHF)", "Ultra High Frequency (UHF)"; the everyday English names that exist are kept: "High Frequency (HF), Short Wave (SW) oder Kurzwelle (KW)" → "High Frequency (HF) or short wave (SW)", "Medium Frequency (MF) oder Mittelwelle (MW)" → "Medium Frequency (MF) or medium wave (MW)". Not "metre / decimetre waves" (DECISIONS.md) |
| Dezimeterwelle (UHF) | decimetre wave (UHF) | |
| Mikrowellen | microwaves | |
| oberhalb 30 MHz | above 30 MHz | |
| Ionosphäre | ionosphere | |
| D-Region / E-Region / F-Region (F1, F2) | D region / E region / F region (F1, F2) | the German deliberately says *Region*; RSGB often says *layer* — keep *region* for consistency |
| Schicht | layer | |
| Ionisation / Rekombination | ionisation / recombination | |
| Absorption | absorption | |
| Raumwelle | sky wave | |
| Bodenwelle | ground wave | fixed term; *ground* allowed here |
| direkte Welle / Sichtverbindung | direct wave / line of sight | |
| tote Zone | skip zone | |
| Sprung / Sprungdistanz / Sprungentfernung | hop / skip distance | "mit einem Sprung (Hop)" → "in one hop" |
| Funkstrecke | radio path | MUF/LUF "für eine Funkstrecke" (AH208, AH210, AH211) |
| Weitverkehrsverbindungen / Überseeverbindungen | long-distance contacts / intercontinental contacts | |
| Beamrichtung | beam heading | AH217, AH218 |
| höchste brauchbare / nutzbare Frequenz | maximum usable frequency (MUF) | "highest usable frequency" where an answer describes it in words beside "lowest usable frequency" (AH207, AH211); "Höchste nutzbare Frequenz" as the expansion of MUF → "Maximum usable frequency" (EH204) |
| höchste durchlässige Frequenz | maximum transmission frequency | made-up distractor labelled "(LUF)" (AH206); not *penetration frequency*, which in English is a real name for the critical frequency (distractor c) |
| Abdeckung (durch die F1-Region) | blanketing | AH107 |
| Tagesdämpfung | daytime attenuation | EH210 |
| Sonnenfleckenmaximum / Sonnenfleckenminimum | sunspot maximum / sunspot minimum | "im Sonnenfleckenmaximum" → "at sunspot maximum" |
| Röntgenstrahlung / UV-Strahlung | X-ray radiation / UV radiation | |
| Sonneneruption | solar flare | |
| Fernausbreitung | long-distance propagation (DX propagation) | |
| NVIS (Near Vertical Incidence Skywave) | NVIS (near vertical incidence skywave) | the German writes *Incident* (AG125); English has *incidence* |
| kritische Frequenz (foF2) | critical frequency (foF2) | |
| MUF / LUF / FOT | MUF / LUF / FOT | maximum usable / lowest usable / optimum working frequency |
| Einfallswinkel / Einstrahlung (in die Ionosphäre) | angle of incidence / incidence | trap: *Einstrahlung* in EMC means radiated pick-up. Where the German angle is an elevation ("Einstrahlung … unter einem Winkel von 90 °" = vertical, AH205), write "radiated into the ionosphere at an angle of", not "angle of incidence", which English propagation texts measure from the vertical |
| Brechung / Refraktion | refraction | |
| Reflexion | reflection | |
| Beugung | diffraction | |
| Streuung / Scatter | scatter | |
| Rückstreuung / Backscatter | backscatter | EH202: "Rückstreuung (Backscatter)" → "Backscatter", the bracket only gives the English word |
| Rainscatter / Regenscatter / Aircraft-Scatter / Meteorscatter | rain scatter / aircraft scatter / meteor scatter | |
| Ionisationsspuren von Meteoriten / Meteorbahnen | ionisation trails of meteors / meteor trails | *meteors*, not *meteorites*, for what leaves the trail (AH301, EH304) |
| leuchtende Nachtwolken (NLCs) | noctilucent clouds (NLCs) | NH306 |
| Geländeprofil | terrain profile | NH303 |
| quasi-optische Sichtweite | quasi-optical line-of-sight range | NH302: the range is what increases |
| Troposphäre | troposphere | |
| troposphärische Ausbreitung / Überreichweiten | tropospheric propagation / enhanced (anomalous) propagation | "beträchtliche Überreichweiten erzielen" → "achieve considerably extended ranges" (AH304) |
| Inversionswetterlage / Inversionsschicht | temperature inversion / inversion layer | |
| Ducting / Duct | ducting / duct | |
| Sporadic-E (Es) | sporadic E (Es) | |
| Aurora / Polarlicht | aurora | |
| Aurora-Erscheinungen / Polarlichter / Nordlichter | auroral phenomena / aurorae / northern lights | |
| Aurora-Verbindung | aurora contact | |
| verbrummt (Aurora-Signal) | buzzing | one rendering wherever the German has *verbrummt*: "flatternder und verbrummter Ton" → "fluttering, buzzing tone" (AH308); "stark verbrummt empfangen" → "received with a heavy buzz" (AH220); "verbrummte Ultrakurzwellen" → "buzzing VHF waves" (AH305). Not *hum*, which reads as mains hum |
| Polarkreis | Arctic Circle | |
| Erdmagnetfeld | geomagnetic field | |
| Funkhorizont / Horizont | radio horizon / horizon | |
| Erdkrümmung | curvature of the earth | |
| Erdoberfläche | earth's surface | |
| Atmosphäre | atmosphere | |
| Mehrwegeausbreitung | multipath propagation | |
| Fading / Schwund | fading | |
| Flatterfading | flutter fading | |
| Sonne / Sonnenaktivität | sun / solar activity | |
| Sonnenfleckenzyklus / Sonnenflecken | sunspot cycle / sunspots | |
| Sonnenfleckenrelativzahl | sunspot number | |
| solarer Flux | solar flux | |
| Sonnenwind / Flares | solar wind / solar flares | |
| Mögel-Dellinger-Effekt | Mögel–Dellinger effect (sudden ionospheric disturbance, SID) | keep the German-usage name |
| Greyline / Dämmerungszone | grey line | British *grey* |
| Tag / Nacht / Nachtstunden | day / night / night-time hours | |
| Ionosonde | ionosonde | |

## 11. Measurement

| German | English | Note |
|---|---|---|
| Messung / Messen | measurement / measuring | |
| Messungen und Messinstrumente | measurements and measuring instruments | catalogue heading |
| Messgerät / Messinstrument | meter; measuring instrument | *meter* (instrument) vs *metre* (unit) |
| Messmittel | measuring equipment | |
| Messobjekt | device under test (DUT) | |
| Strommessgerät / Amperemeter | ammeter | |
| Spannungsmessgerät / Voltmeter | voltmeter | |
| Strom- und Spannungsmessgeräte | ammeters and voltmeters | catalogue heading |
| Vielfachmessgerät / Multimeter | multimeter | |
| Zeigerinstrument / Analoginstrument | moving-coil meter; analogue meter | |
| Messbereich | (measuring) range | |
| Nebenwiderstand (Shunt) | shunt | |
| Vorwiderstand (Messgerät) | multiplier (series resistor) | |
| Messgenauigkeit / Genauigkeit | accuracy | |
| Auflösung | resolution | |
| Anzeige (Messgerät) | reading; indication | trap: *Anzeige* in BEMFV = notification |
| Skalenteil / Division | division | |
| Parallaxenfehler | parallax error | |
| Oszilloskop / Oszillogramm | oscilloscope / oscillogram (trace) | |
| Schirmbild | screen display (oscilloscope screen) | |
| Tastkopf | probe | "10:1 Tastkopf" → "10:1 probe" |
| Zeitbasis | timebase | |
| Trigger | trigger | |
| Vektorieller Netzwerkanalysator (VNA) | vector network analyser (VNA) | British *analyser* |
| Netzwerkanalysator | network analyser | |
| Spektrumanalysator | spectrum analyser | |
| Stehwellenmessgerät / SWR-Meter | SWR meter | |
| Leistungsmesser / Power-Meter | power meter | |
| Frequenzmessung | frequency measurement | |
| Frequenzzähler | frequency counter | |
| Torzeit | gate time | |
| Vorteiler | prescaler | frequency counter; on an oscilloscope *X-/Y-Vorteiler* → X/Y attenuator |
| Absorptionsfrequenzmesser | absorption wavemeter | RSGB term |
| Dipmeter | dip oscillator (dip meter) | |
| Feldstärkeanzeiger / Feldstärkemessgerät | field-strength meter | |
| Dummy Load / künstliche Antenne / Abschlusswiderstand | dummy load / termination | |
| Sonstige Messgeräte und Messmittel | other measuring instruments and equipment | catalogue heading |
| Rauschgenerator / Signalgenerator | noise generator / signal generator | |
| Messsender (Messender) | signal generator | |
| Messbrücke | measuring bridge | |
| Kreuzzeigerinstrument | cross-needle meter | |
| Thermoumformer | thermocouple converter | "Messgerät mit Thermoumformer" → "meter with a thermocouple converter" (AI105) |
| Zweitontest | two-tone test | |
| ppm | ppm | |
| Vielfachinstrument / Universalmessgerät | multimeter | as *Vielfachmessgerät* |
| Gleichspannungsmessgerät / Wechselspannungsmessgerät | DC voltmeter / AC voltmeter | |
| Widerstandsmessgerät / Ohmmeter | ohmmeter | |
| Wechselstromzähler | AC electricity meter | the household energy meter; distractor (EI501) |
| Transistorvoltmeter / True RMS-Voltmeter | transistor voltmeter / true-RMS voltmeter | |
| Oszillograf / Speicheroszilloskop | oscillograph / storage oscilloscope | |
| Diodentastkopf | diode probe | |
| HF-Tastkopf / Gleichspannungstastkopf | RF probe / DC probe | AI604, AI605 |
| Spitzenwertgleichrichter / Messausgang | peak rectifier / measurement output | AI602 |
| Dauerleistung (künstliche Antenne) | continuous power | AI601 |
| Triggereinrichtung / Triggerschwelle | trigger circuit / trigger threshold | |
| X-Vorteiler / Y-Vorteiler (Oszilloskop) | X attenuator / Y attenuator | the scope's input attenuators (AI302), not a prescaler; *Vorteiler* of a frequency counter is the *prescaler* (AI504) |
| Frequenzmarken-Generator | frequency marker generator | |
| Hüllkurvenform | envelope shape | |
| Frequenzmessgerät / Frequenzmesser | frequency meter | kept apart from *Frequenzzähler* → frequency counter, where the German uses both |
| Hauptoszillator (Frequenzzähler) | timebase oscillator | the counter's reference (AI504) |
| Anzeigegenauigkeit | display accuracy | |
| Frequenzgenerator | signal generator | "Quarzofen- oder GPS-synchronisierter Frequenzgenerator" → "signal generator stabilised by a crystal oven or synchronised to GPS" (AI511) |
| Absorptionswellenmesser / Resonanzwellenmesser | absorption wavemeter / resonance wavemeter | |
| SWR-Messbrücke | SWR bridge | |
| Absolutleistungsmesser / Impedanzmessgerät | absolute power meter / impedance meter | |
| Antennenimpedanzmesser / Resonanzmessgerät | antenna impedance meter / resonance meter | |
| Peilsender | direction-finding transmitter | AI613 |
| Messkopf zur HF-Leistungsmessung | measuring head for RF power measurement | AI608 |
| Breitbandpegelmesser | broadband level meter | |
| Anpassungsübertrager | matching transformer | |
| Messanschluss / Messeingang (VNA) | test port | |
| Kalibrierung / Nullpunktabgleich | calibration / zero adjustment | |
| Betriebszustände Kurzschluss, Leerlauf und Anpassung | short-circuit, open-circuit and matched conditions | VNA check (EI206) |
| Abschlusswiderstand (VNA, Richtkoppler) | terminating resistor; termination | EI206, AI401 |
| Resonanzverlauf | resonance curve | AI207, AI208 |
| Frequenzreinheit | spectral purity | |
| Erdungswiderstand | earth resistance | |
| Bakensegment | beacon segment | AI510 |
| erdnahes Ende (künstliche Antenne) | earthed end | AI606 |
| effektive Leistung | RMS power | AI105 |

## 12. EMC and safety

| German | English | Note |
|---|---|---|
| elektromagnetische Verträglichkeit (EMV) | electromagnetic compatibility (EMC) | |
| Störung / Störungen | interference | uncountable; "Störungen" → "interference" |
| Funkstörung | radio interference | |
| störende Beeinflussung / Beeinträchtigung | interference / impairment | |
| Störemissionen | interference emissions | |
| Störfestigkeit | immunity | |
| Störungen elektronischer Geräte | interference to electronic equipment | |
| Störquelle | source of interference | |
| Bürstenmotor (schlecht entstört) | (poorly suppressed) brush motor | |
| Ursachen / Abhilfe / Abhilfemaßnahmen | causes / remedies / remedial measures | |
| Einstrahlung | radiated pick-up; direct pick-up | RSGB *breakthrough* for the effect on consumer equipment |
| Einströmung | conducted pick-up (via leads) | |
| Direkteinstrahlung | direct pick-up | |
| Mantelwellendrossel | common-mode choke | as *Mantelwellensperre*; EJ118 "choke balun", because its correct answer is "common-mode RF interference signals" (no echo, DECISIONS.md) |
| Einfügedämpfung | insertion loss | AJ114 |
| Vorstufe (eines Fernsehgeräts) | input stage | AJ109 |
| Antennenzuführungskabel / Fernseh-Antennenzuführungskabel | antenna feed cable / television antenna feed cable | AJ113, EJ118 |
| Leitungsanschlüsse (eines Geräts) | cable connections | AJ112 |
| hochpermeable Ferritdrossel | high-permeability ferrite choke | AJ112 |
| Klappferritkern | clip-on ferrite core | AJ217 |
| Kollektormotor | commutator motor | trap: not *collector*; EJ112 |
| Bimetall-Temperaturregler | bimetallic thermostat | EJ112 |
| Musik-Anlage / Stereoanlage | hi-fi system / stereo system | EJ113, EJ114 |
| Pfeifstellen | whistles (birdies) | EJ107 |
| Nebenresonanzen | spurious resonances | AJ214 |
| Schirmungsmaß | screening attenuation | EK208 |
| Phantomsignale / parametrische Schwingungen | phantom signals / parametric oscillations | EJ120, EJ121 |
| Reihenhaus / Häuserzeile / Einfamilienhaus | terraced house / row of houses / detached house | EJ110, EJ115 |
| Dachrinne / Schornstein | gutter / chimney | EJ110 |
| D-Netz | D-network (GSM) | German GSM 900 network; "D-Netz-Mobilfunkbereich" → "D-network (GSM) mobile phone band" (AJ204) |
| Betriebsfunk / UKW-Betriebsfunk | private mobile radio (PMR) / VHF private mobile radio | AJ204 |
| Fernsehtechniker des Fachhandwerks | qualified television technician | EJ124 |
| Beeinflussung von Rundfunk- / Fernsehempfang und Unterhaltungselektronik durch Einstrahlung | breakthrough | RSGB term for a strong wanted signal upsetting consumer electronics (an immunity problem, not a fault of the transmitter) |
| Rundfunkempfang / Fernsehempfang | broadcast reception / television reception | |
| Rundfunkempfänger / Fernsehgerät | broadcast receiver / television set | |
| Kabelfernsehen | cable television | |
| Kabelverteilanlage | cable distribution system | VE306 |
| Türsprechanlage | door intercom | |
| Haushalt | household | |
| Nachbar / nachbarschaftlicher Frieden | neighbour / good relations with the neighbours | British *neighbour* |
| vorschriftsmäßig (betrieben) | in compliance with the regulations | |
| Netz / Stromnetz | mains | not "grid" or "network" in this sense |
| Netzspannung / Netzkabel / Netzfilter | mains voltage / mains lead / mains filter | British *lead* for a cable with plugs |
| Steckdose | (mains) socket | not "outlet" |
| Schutzkontaktstecker (Schuko) | Schuko plug (earthed plug) | |
| Schutzkontakt | earthing contact | ND109: "Schutzkontakt-Stecker (Schuko-Stecker)" → "earthed plug (Schuko plug)" |
| Schutzleiter (PE) / Außenleiter (L) / Neutralleiter (N) | protective earth conductor (PE) / line conductor (L) / neutral conductor (N) | |
| Schutzklasse I / II | protection class I / II | |
| Fehlerstromschutzschalter (FI / RCD) | residual current device (RCD) | British term |
| Leitungsschutzschalter | miniature circuit breaker (MCB) | |
| Erde / Erdung / Erder | earth / earthing / earth electrode | never *ground* |
| Erdungsleitung | earthing conductor | |
| Schutzerdung | protective earthing | |
| Haupterdungsschiene | main earthing terminal (MET) | British wiring-regulations term |
| Potentialausgleich | equipotential bonding | |
| Blitzschutz | lightning protection | |
| Blitzschutzsystem / Blitzschutzanlage | lightning protection system (LPS) | |
| Blitzerdung | lightning earthing | |
| Überspannung / Überspannungsschutz | overvoltage (surge) / surge protection | |
| Standrohr (Antenne) | (antenna) mast | the pipe mast on a roof (EK210, EK211) |
| Erdungsanlage | earthing system | EK209, EK210 |
| Blitzschutz-Fachkraft | lightning protection specialist | EK211 |
| Adernkennfarben / grüngelb | core identification colours / green-yellow | EK205 |
| Ladedrossel (Schaltnetzteil) | storage choke | EK203 |
| Auslösecharakteristik "Flink" / "Mittelträge" / "Träge" | "fast-acting" / "medium time-lag" / "time-lag" | IEC 60127 fuse characteristics (EK204) |
| Körperdurchströmung / Elektrounfall | current flowing through the body / electrical accident | NK302–NK304 |
| Störlichtbogen | arc fault | NK302 |
| Herzrhythmusstörungen / Herzkammerflimmern | cardiac arrhythmias / ventricular fibrillation | NK303, NK304 |
| stabile Seitenlage | recovery position | NK304 |
| Verbrennungen / Verätzungen / Verbrühungen | burns / chemical burns / scalds | NK303, NK306 |
| Kurzschlussstrombegrenzung / thermische Abschaltung | short-circuit current limiting / thermal shutdown | PSU safety features (ND108) |
| statische Aufladung | static charge | |
| Ableitwiderstand | bleeder resistor (static drain) | |
| Berührungsspannung | touch voltage | |
| Stromschlag / elektrischer Schlag | electric shock | |
| Lebensgefahr | danger to life | |
| Lichtbogen | arc | |
| Elektrofachkraft | qualified electrician | |
| Sicherheitsvorschriften / Sicherheit | safety regulations / safety | |
| Schutz von Personen | protection of persons | |
| Personen- und Sachschutz | protection of persons and property | |
| Elektromagnetische Verträglichkeit, Anwendung, Personen- und Sachschutz | electromagnetic compatibility, application, protection of persons and property | catalogue heading |
| Isolierung | insulation | |
| Kfz / Fahrzeug / Fahrzeugbatterie / Bordnetz | vehicle / vehicle battery / vehicle electrical system | |
| Zulassung (eines Kraftfahrzeugs) | road approval (of a motor vehicle) | not *licence*, which is the amateur *Zulassung* (NK308) |
| Kabelbaum / Motorraum / Kotflügel / Stoßstange / Armaturenbrett | wiring harness / engine compartment / wing / bumper / dashboard | British car terms (NK309, NK310) |
| Verpolung | reverse polarity | |
| Überlastung | overload | |

## 13. Other frequent words in the question bank

Compounds and general words that recur in the questions; most follow from
the entries above, listed so that they are rendered the same way every time.

| German | English | Note |
|---|---|---|
| Hochfrequenz (HF) | radio frequency (RF) | trap: German *HF* = RF; English *HF* = short wave (3–30 MHz) |
| Hochfrequenzschwingung / HF-Signal | RF oscillation / RF signal | |
| Niederfrequenz (NF) / NF-Signal | audio frequency (AF) / AF (audio) signal | |
| NF-Bandbreite / HF-Bandbreite | audio bandwidth / RF bandwidth | |
| Funkwellen | radio waves | |
| Sendeleistung | transmit power; transmitter power | |
| Sendefrequenz / Empfangsfrequenz | transmit frequency / receive frequency | |
| Betriebsfrequenz / Arbeitsfrequenz / Nutzfrequenz | operating frequency / working frequency / wanted frequency | |
| Oszillatorfrequenz / Oszillatorsignal | oscillator frequency / oscillator signal | |
| Signalfrequenz | signal frequency | |
| Frequenzaufbereitung | frequency generation (frequency synthesis) | |
| Sendesignal / Empfangssignal | transmitted signal / received signal | |
| Sendeantenne / Empfangsantenne | transmitting antenna / receiving antenna | |
| Amateurfunkantenne | amateur antenna | |
| Antennenanschluss / Antenneneingang | antenna socket / antenna input | |
| Antennenimpedanz | antenna impedance | |
| Senderichtung | direction of transmission (beam direction) | "entgegengesetzt zur Senderichtung" → "in the opposite direction to the beam" |
| Sendezweig / Empfangsteil | transmit path / receive section | |
| Verstärkerstufen | amplifier stages | |
| Empfängereingang | receiver input | |
| Ausgangsspannung / Eingangsspannung | output voltage / input voltage | |
| Kollektorspannung | collector voltage | |
| Gleichspannungsquelle / Gleichspannungsversorgung | DC voltage source / DC supply | |
| zweipolig (Versorgungsleitung) | two-conductor; "has two conductors" | ND103, ND104 |
| Mobilfunktransceiver / Mobilfunk-Transceiver | mobile transceiver | not *mobile phone* |
| Masseleitung | chassis lead | AD612; cf. *Masse* → chassis (§4) |
| Leistungsaufnahme / Stromaufnahme / Stromentnahme | power consumption (power drawn) / current drawn | |
| häusliche Spannungsversorgung / Stromversorgung (230 V) | domestic mains supply (230 V) | |
| Wechselspannungsverstärkung | AC voltage gain | |
| Spannungsschwankung | voltage fluctuation | |
| Schaltungspunkt | point in the circuit; node | |
| Beschaltung | external circuitry | |
| Lötstelle (fehlerhafte) | (faulty) solder joint | |
| Leuchtanzeige | indicator light | |
| Stromgewinnung | electricity generation | |
| Heizwendel | heating coil | |
| Anschluss / Anschlüsse | terminal; connection / terminals; leads (of a component) | |
| Transistoranschlüsse | transistor terminals (leads) | |
| Isolierschicht-FET (MOSFET) | insulated-gate FET (IGFET, MOSFET) | |
| Halbleitergrundstoff | base semiconductor material | |
| Grenzfläche | boundary (interface) | |
| Spulenwert / Kondensatorwert | inductor value / capacitor value | |
| Kupferdraht / Draht | copper wire / wire | |
| Durchmesser | diameter | |
| Länge / Höhe | length / height | *Höhe über Grund* → height above ground — the one fixed phrase where *ground* is natural; *above the earth's surface* also fine |
| Entfernung / Abstand | distance / spacing | |
| Entkopplung | decoupling | |
| Richtkoppler | directional coupler | |
| Widerstandstransformation | impedance (resistance) transformation | |
| Phasendrehung | phase reversal; phase rotation | |
| Koaxialleitung / Leitungseingang | coaxial line / line input | |
| Spiegelkörper (paraboloid geformter) | (paraboloidal) reflector | |
| Feed (Erreger) | feed | |
| Fuchs-Antenne | Fuchs antenna | proper name (Joseph Fuchs, end-fed half-wave); trap: not *fox* |
| Raumwellenausbreitung / Kurzwellenausbreitung | sky-wave propagation / HF propagation | |
| Überhorizontverbindungen | beyond-the-horizon contacts | |
| Ionisationsgrad / Ionisationserscheinungen | degree of ionisation / ionisation phenomena | |
| Fluxwerte | (solar) flux values | |
| Strahlungsintensität / Strahlungsenergie | radiation intensity / radiated energy | |
| Störwahrscheinlichkeit | likelihood of interference | |
| Gebäudeerdungsanlage / Erdleitung | building earthing system / earth lead | |
| Auslösecharakteristik | tripping characteristic | fuses, circuit breakers |
| Satellitenfunk / Satellitenkommunikation / Weltraumkommunikation | satellite communication / space communication | |
| Funkgespräch | (voice) contact; conversation | |
| Amateurfunkvereinigung / Amateurfunkverband | amateur radio society / national amateur radio society | e.g. DARC, RSGB |
| Deutscher Amateur-Radio-Club (DARC) | Deutscher Amateur-Radio-Club (DARC) | name stays German |
| Amateurfunkliteratur | amateur radio literature | |
| Behörden und Organisationen mit Sicherheitsaufgaben (BOS) | authorities and organisations with security tasks (BOS) | German public-safety radio users (police, fire, rescue); keep "BOS" |
| Polizei / Feuerwehr / Rettungsdienst / Rettungsleitstelle | police / fire brigade / rescue service / emergency control centre | British *fire brigade* |
| Flugfunkdienst / Seefunkdienst | aeronautical mobile service / maritime mobile service | |
| Mayday | MAYDAY | |
| Bundesrepublik Deutschland | Federal Republic of Germany | |
| Irland / Estland / Armenien / Ukraine / Südafrika / Philippinen | Ireland / Estonia / Armenia / Ukraine / South Africa / the Philippines | |
| kostenpflichtige / gebührenpflichtige Nachprüfung / fachliche Nachprüfung | re-examination subject to a fee / re-examination of competence | a sanction in VC122, VC123, VC125, VE704; *fachliche* makes it a re-test, and the bare word is the same sanction (DECISIONS.md) |
| Wortlaut | wording | "nach dem Wortlaut der AFuV" → "according to the wording of the AFuV" |
| Regelwerk | set of rules; regulations | |
| im Sinne des … | within the meaning of … | legal phrasing |
| Voraussetzung | prerequisite; condition | |
| Aussage | statement | "Welche Aussage ist richtig?" → "Which statement is correct?" |
| Darstellung / Abbildung / Bild / Skizze | diagram / figure / picture / sketch | "Die Darstellung zeigt …" → "The diagram shows …" |
| Draufsicht | plan view | |
| Korrekturfaktor | correction factor | |
| Auswahlantworten | answer options | |
| Farbton / Helligkeit | colour (hue) / brightness | waterfall display |
| zeitgleich | simultaneously | |
| ca. / zirka / etwa | approximately; about | |
| höchstens / mindestens | at most / at least | |
| Erhöhung / Verringerung | increase / reduction | |
| Einhaltung | compliance (with) | |
| Erdoberfläche mittlerer Leitfähigkeit / Erdboden | ground of average conductivity / the ground | soil under an antenna (AG223, AG224); *earth* stays for earthing |
| Dämpfungsmaß | attenuation | in dB (EG309, EG310) |
| Kabelkanal | cable duct | |
| Spannungsüberschlag | flashover | |
| Dachboden | loft | British |
| Cinch (Stecker) | RCA (phono) | German trade name for the RCA connector (NG206) |
| Pertinax | Pertinax | trade name of SRBP laminate; kept |
| HF-Übertrager (Balun) | RF transformer (balun) | AG422 |

## 14. Further terms from the course text, drawings and slides

Terms that occur mostly outside the question bank (course sections,
solutions, drawing labels, slides, site chrome). Placeholder call signs in
the German (DL1PZ, DO7PR, DM4EAX/p …) stay exactly as they are.

| German | English | Note |
|---|---|---|
| statisches Feld / Streufeld | static field / stray field | |
| Nahfeld (reaktives / strahlendes) / Fernfeld | near field (reactive / radiating) / far field | |
| Maxwellsche Gleichungen | Maxwell's equations | |
| Verschiebungsstrom | displacement current | |
| Äther | (luminiferous) aether | historical |
| Wellenberg / Wellental | crest / trough | |
| Elektromagnetisches Spektrum | electromagnetic spectrum | |
| Höhenstrahlung / Terahertzstrahlung | cosmic radiation / terahertz radiation | |
| Wickelkondensator | wound (rolled) capacitor | |
| Zylinderspule / Ringkernspule | solenoid / toroidal inductor | |
| Primärwindung / Sekundärwindung | primary turn(s) / secondary turn(s) | usually *primary / secondary winding* |
| Eigenkapazität / Wicklungskapazität | self-capacitance / inter-winding capacitance | |
| Spule ohne Kern / mit Eisenkern / mit Ferritkern / veränderliche Spule | air-cored / iron-cored / ferrite-cored / variable inductor | symbol-chart labels |
| HF-Trenntrafo / Übertrager (ü = 1:n) | RF isolating transformer / transformer (ratio 1:n) | |
| Fertigungstoleranz | manufacturing tolerance | |
| Multiplikator (Farbcode) | multiplier | |
| Schleifkontakt / Anschlag (Potentiometer) | wiper / end stop | |
| Durchkontaktierung | via (plated-through hole) | |
| Mittelabgriff | centre tap | |
| Knickspannung | knee voltage | |
| PN-Grenzschicht / Diffusion | PN junction / diffusion | |
| Basis-Emitter-Übergang | base-emitter junction | |
| antiparallel geschaltete Dioden | diodes in inverse parallel (back-to-back) | |
| HF-Diode | RF diode | |
| durchgesteuert | fully on (saturated) | transistor |
| Leitungsverluste (MOSFET) | conduction losses | |
| Querwiderstand | lower divider resistor | the base-divider resistor ($R_2$) that carries the divider current (AC517, AC518); not *bleeder resistor*, which is *Ableitwiderstand* (§12) |
| Querstrom | divider current | current through the lower resistor of a base potential divider |
| Bias-Netzwerk | bias network | |
| kapazitiver Teiler | capacitive divider | |
| Eingangsanpassung / Ausgangsanpassung | input matching / output matching | |
| Impedanzanpassung | impedance matching | |
| hochohmig / niederohmig | high-impedance (high-resistance) / low-impedance (low-resistance) | |
| Reale Spannungsquelle / reales Messgerät | real (practical) voltage source / real (practical) meter | |
| Bezugsklemme / Bezugsleitung | reference terminal / reference conductor | |
| Kurzschluss- und Verpolungsgefahr | risk of short circuit and reverse polarity | |
| Sicherungshalter / Flachstecksicherung | fuseholder / blade fuse | |
| Netzanschlusskabel | mains lead | |
| Sicherheitsaufschlag | safety margin | |
| Low-Drop-Spannungsregler | low-dropout (LDO) regulator | |
| Impulsbreitenmodulator / Pulsbreite / Impulsdauer | pulse-width modulator / pulse width / pulse duration | |
| Drosselspule | choke | |
| Ferrit-Perle | ferrite bead | |
| Verstärkerklasse (A / B / AB / C) | amplifier class (A / B / AB / C) | |
| Transistorendstufe / Röhrenendstufe | transistor PA / valve PA | British *valve* |
| Hüllkurvenverstärker | envelope amplifier | |
| Aussteuerung | drive (level) | |
| Kompression / Sättigung | compression / saturation | |
| Steuerkennlinie | transfer characteristic | |
| Dreifachsuper / Mehrfachsuper | triple-conversion / multiple-conversion superhet | |
| Doppeldiodenmischer / additiver Diodenmischer | two-diode mixer / additive diode mixer | |
| High-Level-Ringmischer / Polwender | high-level ring mixer / polarity reverser (commutator) | |
| Powersweep / Zweitontest | power sweep / two-tone test | |
| Abschwächer | attenuator | same as Dämpfungsglied |
| breitbandiges Dämpfungsglied | broadband attenuator | |
| Auto-Notch-Filter | automatic notch filter | |
| Zündfunken | ignition sparks | |
| Leitkreis | series pass circuit (*Leitkreis*) | a series tuned circuit in series with the signal path, which passes its resonant frequency (drawing 1039): the counterpart of the *Saugkreis* (acceptor) among the band-pass circuits. English has no established name; the German word is given in brackets at first mention (schwingkreis_1). Corrected from "coupled-circuit band-pass filter", which no text had used |
| Tuning Word / Lookup-Tabelle | tuning word / look-up table | |
| Mittenfrequenz | centre frequency | |
| Frequenzauflösung | frequency resolution | |
| Gibbs-Phänomen | Gibbs phenomenon | |
| Laufzeit / Pufferspeicher / Jitter / Clipping | delay / buffer / jitter / clipping | |
| zeitkontinuierlich / zeitdiskret | continuous-time / discrete-time | |
| wertkontinuierlich / wertdiskret | continuous-value / discrete-value (quantised) | |
| Digitalisierung | digitisation | |
| Rekonstruktionsfilter | reconstruction filter | |
| Quellencodierer / Kanalcodierer / Kanaldecodierer / Quellendecodierer | source encoder / channel encoder / channel decoder / source decoder | |
| Sende- und Empfangsketten | transmit and receive chains | |
| Gerade / ungerade Parität | even / odd parity | |
| Hamming-Code | Hamming code | |
| Zeitmultiplex / Frequenzmultiplex / Codemultiplex | time-division / frequency-division / code-division multiplexing | |
| Übersprechen | crosstalk | |
| Netzanteil / Hostanteil | network part / host part | IP addresses |
| Fernschreiber | teleprinter | |
| Eintonsignal | single-tone signal | |
| Equalizer / Dynamikkompressor / Dynamikumfang | equaliser / compressor / dynamic range | British *equaliser* |
| NF-Sprachprozessor | audio speech processor | |
| Sendepegel | transmit level | |
| FM-Hub / Hubbegrenzung / Hubeinstellung | FM deviation / deviation limiting / deviation setting | |
| Steckverbindungs-System / Kontaktstift / Federkontakte | connector series / contact pin / spring contacts | |
| Löten / Crimpen / Bajonettverschluss / Schraubverbindung | soldering / crimping / bayonet coupling / screw coupling | |
| Überwurfmutter / Rändelung / Sechskant | coupling nut / knurling / hexagon | |
| Erdnagel / Erdspieß | earth spike (earth rod) | |
| Freisprecheinrichtung | hands-free kit | |
| Bordnetzspannung | vehicle supply voltage | |
| Zweiband-Dipol / Sperrkreis-Dipol | dual-band dipole / trap dipole | |
| Fuchskreis | Fuchs matching circuit | *Fuchs circuit* after the first mention in a file; *Fuchsantenne* → Fuchs antenna (antennenformen_2, antennenformen_3) |
| Verlängerungsfaktor (Loop) | lengthening factor | |
| Strahlungsrichtung / Strahlengang | direction of radiation / radiation path | |
| Winkeldämpfung | off-axis attenuation | |
| Dämpfungsfaktor | attenuation factor | |
| SAT-Spiegel | satellite dish | |
| Gitterturm | lattice tower | |
| Rayleigh-Streuung | Rayleigh scattering | |
| Fata Morgana | mirage | |
| Doppler-Spread | Doppler spread | |
| Short Skip / Twilight-DX | short skip / twilight DX | |
| Shortwave Fade-Out | short-wave fade-out (SWF) | |
| mittabstandstreue Azimutalprojektion | azimuthal equidistant projection | |
| Sonnenlicht / Sommer / Winter | sunlight / summer / winter | |
| Einzelzuteilung / Allgemeinzuteilung | individual assignment / general assignment | |
| exterritoriale Station | extraterritorial station | |
| Selbsterklärung | self-declaration | |
| 5 Sicherheitsregeln der Elektrotechnik | five safety rules (of electrical work) | German DIN VDE 0105 rules |
| Isolierhandschuhe | insulating gloves | |
| Blitzschutzkonzept / Blitzschutzfachkraft | lightning protection concept / lightning protection specialist | |
| Nachbargrundstück | neighbouring property | |
| Pflicht zur Hilfeleistung | duty to render assistance | |
| 5 W-Fragen | the 5 Ws | emergency-message checklist; in the course *Wo / Wer / Was / Wie viele / Warten* → *Where / Who / What / How many / Wait* (for questions), not the journalists' who, what, where, when, why; the digit kept as the German writes it (notfunk) |
| Rapportsystem RSV | RSV report system | |
| Mobilfuchsjagd | mobile direction finding | |
| DX Century Club (DXCC) / CQ DX | DXCC / CQ DX | |
| QSL-Manager / Callbook / ADIF | QSL manager / callbook / ADIF | |
| Ausbildungspate | mentor | |
| Ortsverband (DARC) | (DARC) local club | |
| Aufstockungskurs | upgrade course | |
| Kurse vor Ort / Selbststudium | local courses / self-study | |
| Präsentation / Folie / Referentenansicht / Vollbild | presentation / slide / presenter view / full screen | |
| Start / Suche / Infos | Home / Search / About | site navigation |
| Eselsbrücke | mnemonic | |
| Grundrechenarten / Dreisatz | the four basic arithmetic operations / the rule of three | school maths the course assumes (erste_schritte); UK schools also say *unitary method* |
| Kofferwort | portmanteau (word) | |
| PTT-Taste / Handmikrofon | PTT button / hand microphone | *button*, as NF108 |
| Abbildung / Bild / Tabelle [ref:…] | Figure / Table [ref:…] | capitalised before a numbered reference (DECISIONS.md) |
| Aussprache (Buchstabiertafel) | pronunciation | the column uses the ITU's English respelling, RR Appendix 14 (DECISIONS.md) |
| hier ist / von (in a call) / bitte kommen / und hört | this is / this is / over / listening | voice procedure in `<qso>` (BE102, BE103; DECISIONS.md) |
| Ist diese Frequenz frei? | Is this frequency in use? | BE105 *besetzt* → "in use" |
| Wer zuerst kommt, mahlt zuerst | first come, first served | |
| Lesbarkeit / Verständlichkeit | readability / intelligibility | RST R value |
| nicht lesbar / zeitweise lesbar / mit Schwierigkeiten lesbar / ohne Schwierigkeiten lesbar / einwandfrei lesbar | unreadable / readable at times / readable with difficulty / readable without difficulty / perfectly readable | RST R scale (rst) |
| einwandfrei / unverständlich (Signal) | perfect / unintelligible | RST examples; BE204 "perfectly" |
| Empfangspegelanzeige / Empfangspegel | received-signal-level indicator / received signal level | the S meter (NF301) |
| über Stufe 9 (S-Meter) | above S9 | "9+20dB" unchanged |
| Flugfunk / Seefunk | aeronautical radio / maritime radio | informal service names in course text |
| Flug- und Seefunkstellen | aeronautical and maritime radio stations | |
| zugelassenes CB-Funk-Gerät | approved CB radio | |
| Verschleierungsverfahren | methods of obscuring the content | as *Verschleierung* (§1.1), VD103 "to obscure the content" |
| digitale Kodierungen | digital encodings | |
| Taxi-Funk / Absprachen in einem Unternehmen | taxi radio / coordination within a business | gewerblich |
| Zusatz "/T" (Ausbildungsfunk) | suffix "/T" | as *Rufzeichenzusatz* (§1.3), VD306 |
| Lösungsweg / Lösung über Ausschlussverfahren | solution / solution by elimination | |
| Hausaufgaben | homework | |
| Koordinatensystem / Achse / Nulllinie | coordinate system / axis / zero line | |
| Sinuskurve / Sägezahnkurve | sine curve / sawtooth | |
| Balkenanzeige / Sieben-Segment-Anzeige | bar graph / seven-segment display | |
| Bedien- und Anzeigefeld | control and display panel | |
| Starkes Signal / Schwaches Signal | strong signal / weak signal | |
| Sammelschiene | busbar | |
| Plastikgehäuse / Metalllegierung / Keramikdielektrikum | plastic case / metal alloy / ceramic dielectric | |
| Windkraftwerk | wind turbine | gleich_und_wechselspannung |
| Einheitenvorzeichen / Einheitenpräfix | unit prefix | the course's variants of *Einheitenvorsatz* (§3) |
| Periode oder auch Periodendauer | period or periodic time | where the German gives both names (amplitude_periode); *Periodendauer* alone stays *period* (§3) |
| Ort (Achsenbeschriftung einer Momentaufnahme) | position | the x-axis label of a snapshot, against $t$ on an oscillogram (funkwellen); the drawing keeps "Ort" until the drawings are done |
| Hochzahl / Exponent | superscript number / exponent | |
| technisch-wissenschaftlicher Taschenrechner | scientific calculator | |
| Exponentialschreibweise / Zehnerpotenz-Schreibweise | exponential notation / power-of-ten notation | |
| zugeschnittene Größengleichung | tailored quantity equation | DIN 1313 term for an equation that fixes the units of its values ($f[[\unit{\mega\hertz}]] = 300/\lambda[[\unit{\meter}]]$); English has no settled name, and the course defines it (formeln_umstellen) |
| Grundeinheiten | base units | |
| (eine Formel nach x) umstellen / sich herauskürzen | rearrange (a formula for x) / cancel out | |
| über das Band drehen | tune across the band | |
| Amplitudenspektrum (Funkgerätedisplay) | amplitude spectrum (spectrum display) | course text keeps *amplitude spectrum*, as NI401, and glosses it once with NF104's "spectrum display" (wasserfall) |
| Langwelle (LW) / Mittelwelle (MW) in the frequency-range table | long wave (LW) / medium wave (MW) | written "(Long Wave)", "(Medium Wave)" in the table, title case like its other names; the German everyday names *Kurzwelle (KW)*, *Ultrakurzwelle (UKW)*, *Dezimeterwelle* beside the English names are dropped there, as in BC101–BC106 (DECISIONS.md) |
| Verordnung über den Amateurfunk (AFuV) | Amateur Radio Ordinance (Amateurfunkverordnung, AFuV) | the course text's informal title for the AFuV (frequenzzuteilung); not the formal title *Verordnung zum Gesetz über den Amateurfunk* (§1.2) |
| Nutzungsbestimmungen | conditions of use | VD702 "detailed conditions of use" |
| Nutzungsrechte (primäre / sekundäre) | (primary / secondary) rights of use | |
| Verfügungen und Mitteilungen (der BNetzA) | orders and notices | as *Verfügung* and *Mitteilungen der BNetzA* (§1.2) |
| Küstenfunk / Küstenfunkdienst | coast radio / coast radio service | informal, beside the RR *coast station* (§1.1) |
| Garagentoröffner / Funkwetterstation / Autoschlüssel / Wegfahrsperre / Reifendrucksensor | garage door opener / wireless weather station / car key / immobiliser / tyre pressure sensor | ISM devices; British *tyre*, *immobiliser* |
| Interessenvertretung | representing the interests (of) | |
| geordnetes Nebeneinander der Betriebsarten | orderly coexistence of the modes | IARU |
| Selbstregulierung | self-regulation | |
| Funkpartner finden (CQ) | find someone to talk to | where the German means finding a station to have a contact with at all, not *the other station* of a contact (iaru_bandplan_2m) |
| Telefonie-Direktverbindung | direct telephony contact | as BC214 |
| Bandplan-Bezeichnungen in Klammern ("beacons", "repeater input" …) | dropped where they only repeat the English term; kept where they differ ("FM calling", "digital voice calling", "CW") | the IARU band plan is in English, so the German glosses its labels (DECISIONS.md) |
| *center of activity* (Bandplan-Bezeichnung) | centre of activity (*center of activity* in the band plan) | British spelling in prose; the label is quoted as printed |
| Überreichweiten (Kurstext) | enhanced propagation | index "Enhanced propagation"; *erheblich größere Reichweiten* → considerably greater ranges; cf. §10 (troposphaere, wellenausbreitung) |
| Wetterschicht | weather layer | the troposphere (troposphaere) |
| Inversionswetterlage / troposphärische Inversionsbildung / Inversionsschicht | temperature inversion / formation of tropospheric inversions / inversion layer | NH304 "Formation of tropospheric inversions" |
| Überhorizontverbindungen | beyond-the-horizon contacts | EH302, AH309 |
| Ducting (vom englischen *duct* …) | ducting (from *duct*, meaning roughly a pipe, channel or guide) | the gloss explains the English word and stays; it does not translate it back (troposphaere_3) |
| Beugung / Streuung / Reflexion / Brechung oder Refraktion | diffraction / scattering / reflection / refraction | *Brechung oder Refraktion* is one English word; *gebrochen (refraktiert)* → "bent (refracted)"; *zurückbrechen* → bend back |
| gleichgerichtete Streuung | scattering in a single direction | the slides' definition of reflection (troposphaere_2) |
| Hochatmosphäre / Atmosphärenschichten | upper atmosphere / layers of the atmosphere | |
| Atomrümpfe | positive ions | what free electrons recombine with (ionosphaere_2) |
| gemäßigte Breiten | temperate latitudes | |
| Schicht / Region (Ionosphäre) | layer / region | each as the German writes it, as the text itself distinguishes them (DECISIONS.md) |
| sporadische E-Schicht (Es) / Sporadic-E-Bedingungen | sporadic E layer (Es) / sporadic E conditions | lower-case *sporadic*, as §10 |
| Sonnenzyklus (elfjähriger) | (eleven-year) solar cycle | NH201, EH107 |
| Aktivitätsmaximum / Aktivitätsminimum | activity maximum / activity minimum | solar activity |
| Polarlichter / Aurora- oder Polarlichterscheinung | aurorae / aurora (polar lights) | as §10 |
| flatternd / verbrummt (Aurora-Signal) | fluttering / buzzing | AH308; §10 *verbrummt* |
| Doppler-Spread / Signalrapport | Doppler spread / signal report | aurora_1 |
| Interferenz / Summensignal / Laufzeit (Funkwelle) | interference / sum signal / propagation time | mehrwegeausbreitung, fading |
| Multipath-Effekte / Faraday-Rotation | multipath effects / Faraday rotation | ionosphaere_3 |
| Abstrahlwinkel (Wellenausbreitung) / flach / steil abstrahlen | angle of radiation / radiate at a low angle / radiate steeply | as EH208, AH208, AH209, never "flat"; *Je flacher die Abstrahlung* → "the lower the angle of radiation" |
| Sprung (oder englisch Hop) | hop | the bracket only gives the English word and is dropped (sprungdistanz_1) |
| Short Skip (engl. short skip = "kurzer Sprung") | short skip | gloss dropped (sporadic_e_2) |
| Fading (Schwund) / Schwund, Fading oder QSB | fading / fading or QSB | *Schwund* only repeats *fading* in German and is dropped |
| Ionosphärenmessstation / Ionosonde (Juliusruh) | ionospheric measuring station / ionosonde (at Juliusruh) | |
| Formelzeichen | symbol | the symbols themselves ($f_\text{k}$, $f_\text{krit}$) stay |
| FOT (frequency of optimal transmission, optimale Sendefrequenz) | FOT (frequency of optimum transmission, optimum working frequency) | AH206 "optimum working frequency (f$_{opt}$, FOT)"; the German's English expansion corrected to the usual *optimum* (muf_luf_2) |
| kommerzielle Frequenzplanung | commercial frequency planning | |
| Rauschflur | noise floor | |
| Magnetstürme | magnetic storms | |
| Raumstation ISS | International Space Station (ISS) | |
| Notfunk-Ausbildungswochenende | emergency communications training weekend | photo caption (aurora_1) |
| Lang- und Mittelwelle (Bodenwelle) | long and medium wave | bodenwelle; *Kurzwelle* → HF, as §10 |
| Bodenbeschaffenheit / leitfähiger Boden | nature of the ground / conductive ground | bodenwelle |
| Stadtbereich (Kommunikation im) | (communication) within a city | bodenwelle slides |
| Tag-/Nachtgrenze / Tag- und Nacht-Gleiche | boundary between day and night / equinox | greyline |
| Greyline-DX / Twilight-DX | grey-line DX / twilight DX | British *grey*, as §10 *grey line* |
| Skip-Distanz | skip distance | as *Sprungdistanz* (§10) |
| Strahlungsausbrüche / Plasma-Flares | bursts of radiation / plasma flares | moegel_dellinger_effekt; slides *Sonneneruptionen mit Plasma-Flares* → "solar eruptions with plasma flares", not *solar flares*, so the two words stay apart |
| Radio Blackouts | radio blackouts | |
| Sonneneruption der Klasse X9.0 / aktive Sonnenfleckenregion | solar flare of class X9.0 / active sunspot region | |
| Türöffnertag der Sendung mit der Maus / Maus-Stationen | Door Opener Day (*Türöffnertag*) of the children's television programme *Die Sendung mit der Maus* / Maus stations | the programme's name stays German; *children's television programme* tells the English reader what it is (moegel_dellinger_effekt) |
| Drehwinkel (Richtantenne) | (beam) heading | as AH217, AH218 "beam heading"; *über zwei Drehrichtungen* → "with two different headings" (langer_kurzer_weg_2 slides) |
| Richtantennen (engl. Beams) | directional antennas (beams) | the bracket stays: *beam* is a different English word and explains *beam heading map*, the glossary's bracket for *Beam-Karte* (langer_kurzer_weg_2) |
| Regenscatter (Rainscatter) / Englisch *Rainscatter* | rain scatter | the English name in brackets, and the slide bullet that only gives it, are dropped (scatter) |
| Flatterfading (flutter fading) | flutter fading | the English gloss beside it is dropped (scatter slides); AH223 |
| Verbindungslinie zwischen Sender und Empfänger | line between the transmitter and the receiver | aircraft scatter |
| Dämmerung | twilight | backscatter |
| personengebundene Rufzeichen (Amtssprache) / persönliche Rufzeichen | personal call signs | where the course contrasts the everyday and the official German word, the official one is quoted in German with a literal gloss: "personengebundene Rufzeichen" (call signs tied to the person) (rufzeichenaufbau) |
| Klasse N (Entry Level License) / Klasse E (Novice) / Klasse A (Advanced) | Class N (Entry Level Licence) / Class E (Novice) / Class A (Advanced) | the German's English labels kept, in British spelling (persoenliche_rufzeichen) |
| Wunschrufzeichen | preferred call sign | |
| Webabfrage (der BNetzA) | (BNetzA) online search | the call sign search on the BNetzA website |
| Notfunkklubstation | emergency communications club station | |
| Sonderstation / Sonderrufzeichen | special event station / special event call sign | RSGB usage |
| Aktivierer / Sammler | activator / collector | special event stations |
| Heimatstandort | home location | the location in the licence document |
| Halteleinen | tethers | balloons (rufzeichenzusaetze) |
| 12-Meilen-Zone | 12-mile zone | |
| Rufzeichenzusätze gesprochen: Mobil / Portabel / Maritim Mobil / Aeronautisch Mobil | Mobile / Portable / Maritime Mobile / Aeronautical Mobile | spoken examples in English voice procedure, digits in English, ITU code words (*Foxtrott* → Foxtrot, *Oskar* → Oscar) (DECISIONS.md) |
| besetzt / unbesetzt (Station) | attended / unattended | |
| ununterbrochene, mittelbare und vollständige Kontrolle | continuous, indirect and complete control | AFuV definition of remote operation (§2 Nr. 6a → Section 2 no. 6a) |
| Netzabschaltung | switching off the mains supply | safe state of a remote station |
| § 16 Absatz 2 Satz 2 AFuV | Section 16(2) sentence 2 AFuV | |
| Frequenzablage / Ablage (Relais) | repeater shift / shift | as §2 *Ablage* |
| Relaissteuerung | repeater controller | crossband operation |
| Wide-FM / Schmalband-FM (Narrow-FM) / FM-W / FM-N | wide FM / narrowband FM / FM-W / FM-N | display labels unchanged; bracket dropped as §2 *Schmalband-FM* |
| Subton mit CTCSS | CTCSS subtone | |
| Repeaterverzeichnis / relaisverantwortliche Person (Relaisverantwortlicher) | repeater directory / person responsible for the repeater | |
| Relais oder Repeater (Kurzformen von Relaisfunkstelle) | *Relais* or *Repeater* (in German) | English has one word; the sentence is kept as information about German usage: "In German, repeaters (*Relaisfunkstellen*) are also called *Relais* or *Repeater* for short" (relaisfunkstellen) |
| Linkstrecke / HAMNET-Knoten | link / HAMNET node | NE405 |
| Hoheitsgebiet | sovereign territory | extraterritorial stations |
| Forschungsschiff / Polarforschungsstation | research vessel / polar research station | Polarstern, Neumayer III |
| Umlaufbahn (niedrige / mittlere / hohe / hochelliptische / polare) | orbit (Low Earth Orbit, LEO / Medium Earth Orbit, MEO / Geostationary Orbit, GEO / Highly Elliptical Orbit, HEO / polar orbit) | satelliten |
| Nutzlast (Satellit) | payload | |
| Bodenstationen (Steuersignale an Amateurfunksatelliten) | earth command stations | RR 25.2A wording, as VA303; *verschlüsseln* there → encoded, the cryptographic *Verschlüsselungsverfahren* → encryption methods |
| Reinheitsgebot / Amateurfunkzentrum | German Beer Purity Law (Reinheitsgebot) / Amateur Radio Centre (Amateurfunkzentrum) | special event call signs table; the German name stays in brackets because the call signs abbreviate it (DB50AFZ) |
| Fragenkatalog | question catalogue | the catalogue of examination questions, as §15; "im Fragenkatalog vorkommen" → "appear in the question catalogue" (internationale_landeskenner) |
| Eselsbrücken für Landeskenner (Keiner Will Nach Amerika, Viele Elche …) | the German words kept, English meaning in brackets: "Keiner Will Nach Amerika (nobody wants to go to America)" | they work through the letters of the German words; a mnemonic that is only the country's name takes the English name where it spells the same letters (*Frankreich* → France, *Großbritannien* → Great Britain, *mEXiko* → mEXico); German glosses inside are translated (*CosTa (Küste)* → "CosTa (coast)") (DECISIONS.md) |
| Vereintes Königreich / Vatikan / Liechtenstein / Norwegen / Bulgarien / Griechenland / Belarus / Chile / Mexiko | United Kingdom / Vatican / Liechtenstein / Norway / Bulgaria / Greece / Belarus / Chile / Mexico | country-prefix tables; in table cells without the article (Netherlands, Czech Republic, Philippines) |
| ITU-Regionen / Naher Osten / Ozeanien / Antarktis / Grönland / Mongolei | ITU regions / Middle East / Oceania / Antarctica / Greenland / Mongolia | itu_regionen |
| gezielter CQ-Ruf | directed CQ call | as §2 *gezielter Anruf* (dx slides) |
| Diplomprogramme | award programmes | as §2 *Diplom* |
| (DARC-)Auslandsreferat / CEPT-Länderliste | DARC foreign affairs department (DARC-Auslandsreferat) / CEPT country list | the German name in brackets at first mention in a file (funken_im_ausland) |
| Reports (Berichte) und Recommendations (Empfehlungen) | Reports and Recommendations | the German glosses only translate the CEPT's English document types back and are dropped (bracket rule) |
| Entry Level License / Novice License (CEPT) | Entry Level Licence / Novice Licence | the CEPT labels in British spelling, as §14 *Klasse N (Entry Level License)* |
| Lehrplan | syllabus | ECC Report 89, ERC Report 32, T/R 61-02 |
| Umzug ins Ausland / Wohnsitz verlegen | moving abroad / move one's residence | funken_im_ausland |
| behördliche Zulassung (für Sender und Sendeanlagen) | official approval | the approval radio amateurs are exempt from (recht_zum_selbstbau); not *licence*, which is the amateur's *Zulassung* (§1.3) |
| EU-Konformitätserklärung / Importeure und Händler | EU declaration of conformity / importers and distributors | EU legal wording, as *Inverkehrbringen* (§1.2) |
| Selbstbau | home construction; building your own equipment | as *Selbstbaugerät* → home-built equipment (§1.2) |
| Hochspannungsleitungen im Stromnetz / Höchstspannungsleitung | high-voltage lines of the electricity grid / extra-high-voltage line | *grid* here, not *mains* (§12): the transmission network, not the household supply (spannung) |
| Blitzableiter | lightning conductor | British |
| elektrische Stromstärke (Kurstext) | electric current | English has one word for *Strom* and *Stromstärke* (§3); "Wir sprechen von der elektrischen Stromstärke" → "We speak of the electric current" (strom), as NA202 |
| Stromquelle (wie eine Batterie, Kurstext) | power source | where the course means any source of electricity (stromkreis); *current source* (§3) stays for the circuit element |
| physikalische Stromrichtung | electron flow (the physical direction of current) | as AB601; plain "physical direction of current" where the text speaks of ions carrying the charge, where *electron flow* would be wrong (physikalische_stromrichtung) |
| Wasserkreislauf / Pumpe / Ventil / Wasserrad | water circuit / pump / valve / water wheel | the circuit analogy (stromkreis) |
| Kippschalter / Schiebeschalter | toggle switch / slide switch | |
| Herzstillstand / Elektrokardiogramm (EKG) | cardiac arrest / electrocardiogram (ECG) | the English abbreviation (gefahren) |
| Sekundärunfälle / Schreck | secondary accidents / fright | NK302 (gefahren) |
| 5 Sicherheitsregeln: Freischalten / Gegen Wiedereinschalten sichern / Spannungsfreiheit feststellen / Erden und Kurzschließen / Benachbarte, unter Spannung stehende Teile abdecken oder abschranken | Isolate / Secure against reconnection / Verify that no voltage is present / Earth and short-circuit / Cover or fence off adjacent live parts | the five rules of DIN VDE 0105-100 (EN 50110), British *isolate* and *earth* (gefahren) |
| Messleitung / Anschluss (Multimeter) | test lead / socket | spannungsmessung, strommessung |
| Zeigerinstrument / Zeiger / Zeigeranzeige | analogue meter / needle / needle display | §11 *Zeigerinstrument*; *needle* as §2 *Zeigerausschlag* (zeigerinstrumente_ablesen) |
| kleinste Auflösung / Auflösungsvermögen | finest resolution / resolving power | AI104 "finest resolution" |
| Messgenauigkeit (auch Toleranz oder Fehler) | accuracy (also tolerance or error) | strom_spannung_messung_3 |
| Kenngröße (beim Messen) / Faustregel | parameter / rule of thumb | |
| Stromteilung | current division ("the current divides") | |
| reales Spannungsmessgerät / reales Strommessgerät | real voltmeter / real ammeter | drawing labels of 1004, 1007, which stay German until the drawings are done |
| Spitzen- oder Scheitelwert | peak (or crest) value | where the German gives both names (spitze_effektiv_wert); either alone stays *peak value* (§3) |
| Spitzenspannung / Effektivspannung / Spitzen-Spitzen-Spannung | peak voltage / RMS voltage / peak-to-peak voltage | captions and solutions (spitze_effektiv_wert, AI305, AI306) |
| bedrahtet (Bauteil) | leaded | as opposed to SMD (spitze_effektiv_wert) |
| Kästchen (Oszilloskop) | square | the grid square; *Skalenteil / Division* → division (§11) (oszilloskop_1) |
| Gitter (Oszilloskopbildschirm) | grid | |
| AUTO-Taste / SINGLE-Taste / X-Position | AUTO button / SINGLE button / X position | front-panel labels (oszilloskop_1, oszilloskop_2) |
| Triggerspannung / Triggereinrichtung | trigger voltage / trigger circuit | AI302; the German gloss *engl. trigger = „auslösen"* is dropped (bracket rule) |
| Prüfspitze / Krokodilklemme | probe tip / crocodile clip | British *crocodile clip* |
| Masseverbindung / Bezugsmasse (Tastkopf) | earth connection / earth reference | the probe's clip goes to the scope's earthed screen; *earth*, never *ground* (oszilloskop_2) |
| Teilverhältnis (Tastkopf) | division ratio | 10:1, 1:1 probes |
| Typschild | rating plate | leistung |
| Wickelwiderstand / Wickelkörper | wound resistor / former | wirewound resistors (widerstand_materialien) |
| Überlastbarkeit | overload capacity | |
| Manganin / Konstantan | manganin / constantan | resistance alloys, lower case |
| aufgedampft / Träger (Schichtwiderstand) | vapour-deposited / substrate | |
| Kaltleiter / Heißleiter (Werkstoffeigenschaft) | PTC conductor / NTC conductor | where the German means a material, not the component ("Die meisten Metalle sind Kaltleiter", leiterwiderstand): *PTC thermistor* (§4) would call a metal a component |
| NTC / PTC (englisch Negative / Positive Temperature Coefficient) | NTC / PTC (negative / positive temperature coefficient) | the German *(englisch …)* gloss gives the expansion, which in English is stated plainly: "*NTC* stands for negative temperature coefficient" (widerstand_ntc_ptc) |
| Einschaltstrombegrenzung | inrush current limiting | |
| Thermoelement | thermocouple | cf. *Thermoumformer* → thermocouple converter (§11) |
| Platine | circuit board; printed circuit board (PCB) | as *Leiterplatte* (§4) |
| Bauform (Diode, LED, SMD) | package style; package | |
| Merkhilfe | memory aid | |
| *Vertiefung:* (label opening an indepth box) | *In depth:* | |
| Kurze Wiederholung (Folie) | quick recap | |
| Leistungsfaktor / Verhältnisfaktor (Dezibel) | power ratio / ratio | the ratio of two powers that a dB value expresses (dezibel_1, dezibel_2), as the questions' "(as a power ratio)"; trap: English *power factor* is cos φ. *Gesamtverstärkungsfaktor* → overall gain factor |
| Logarithmieren / Potenzieren | taking the logarithm / raising to a power | |
| Zehnerlogarithmus | base-ten logarithm | the German's other name for the common logarithm (§3 *Logarithmus*) |
| Eulersche Zahl | Euler's number | |
| Bel (Tabellenspalte, Folien) | bels | "Wir zählen die Nullen (und nennen das Ergebnis "Bel")" → "… call the result "bels"" (dezibel_1 slides) |
| Hilfsmaßeinheit / Pseudoeinheit | auxiliary unit / pseudo-unit | the dB (dezibel_2, AA112) |
| (Dezibel) bezogen auf / Bezugswert | (decibels) relative to / reference value | "dBm = Dezibel bezogen auf mW" → "decibels relative to mW"; *Bezugsgröße* → reference quantity (§3) |
| Signalkette | signal chain | |
| Zusatz (an dB: dBm, dBi …) | suffix | "Diese Zusätze geben an, auf welche Bezugsgröße …" (dezibel_1, dezibel_2); not *addition* |
| Referenzstrahler | reference radiator | dBi, dBd |
| vorzeichenrichtige Subtraktion | subtracting with the correct signs | dBm values (dezibel_2) |
| Hilfsmittel (Prüfung) | examination aids | the permitted aids, i.e. the formula sheet (AA108–AA110) |
| Gegeben / Lösungsweg / Abkürzung (Überschriften in Lösungen) | Given / Solution / Shortcut | *Abkürzung* as a heading is a quicker way to the answer; trap: elsewhere *Abkürzung* is *abbreviation* (§2) |
| (Formelsammlung:) Pegel, Verstärkung, Leistung / Leistungs- und Spannungspegel | (formula sheet:) levels, gain, power / power and voltage levels | the formula sheet's section names, cited in brackets in solutions; lower case, as descriptions |
| Energiegehalt | energy content | battery |
| Stromrechnung / Stromverbrauch | electricity bill / electricity consumption | AA103 |
| Zimmerlautstärke | normal room volume | dezibel_1 slides |
| Handfunke | handheld | as *Handfunkgerät* (§6) |
| effektive Leistung (EME-Station) | effective radiated power | the 100 kW of an EME station in the dB slides (dezibel_1); not *RMS power*, which is the measuring sense (§11, AI105, and EB513's *effektive Leistung*) |
| frequenzerzeugende Stufe | frequency-generating stage | |
| Gehörlosenlehrer | teacher of the deaf | A. G. Bell |
| Bauformen (Fotos von Kondensatoren, Spulen, Transistoren) | types | "Schaltzeichen und Bauformen von Kondensatoren" → "Circuit symbol and types of capacitors" (bauelemente); *package style* (*Bauform* above) stays for semiconductor and SMD packages |
| Strom über Zeit / Leistung über Zeit (Folien) | current times time / power times time | ladung_energie slides; English "over time" would read as a division beside $Q = I\cdot t$ |
| in den Äther lauschen (umgangssprachlich) | listen in to the ether | the colloquial survival of the *Äther* (physics: *aether*, above), spelt *ether* as English writes the idiom; "has survived in everyday language as "the ether"" bridges the two spellings (e_feld) |
| zeitlich veränderlich / zeitlich variabel / zeitlich konstant / zeitlich unveränderlich | (that) varies with time; time-varying / constant with time; does not vary with time | EB301 "a current that varies with time" / "constant with time" (e_feld, em_feld) |
| senkrecht aufeinander stehen / senkrecht auf | (be) at right angles to each other / at right angles to | EB304; *perpendicular* only for a line on a plane (em_feld) |
| Durchschlagsfeldstärke / Grenzfeldstärke | breakdown field strength / limiting field strength | the field strength a dielectric withstands; *Durchschlagsfestigkeit* stays *dielectric strength* (§4, EB104) (e_feld) |
| stromdurchflossener Leiter | current-carrying conductor | |
| (Feldlinien) in sich geschlossen | (field lines) closed loops | "sind stets in sich geschlossen" → "are always closed loops" (h_feld) |
| mittlerer Durchmesser / mittlerer Umfang / mittlere Länge (Ringkern) | mean diameter / mean circumference / mean length | EB203 |
| Wicklungsanzahl | number of turns | as *Windungszahl* (§4) |
| gleichgerichtetes Feld | a field pointing in one direction | the uniform field's lines all run one way (e_feld slides); not *rectified*, which is *gleichgerichtet* for a voltage |
| Naturforscher (historisch) | natural philosopher | the period term for a scientist before about 1850 (Ørsted, 1820, h_feld); a modern *Naturforscher* is a *scientist*. The German's *Oerstedt* is written *Ørsted* |
| elektrische Feldkonstante / magnetische Feldkonstante | electric constant / magnetic constant | $\varepsilon_0$, $\mu_0$ (kondensator_1, spule_1) |
| relative Dielektrizitätszahl / relative Permeabilität | relative permittivity / relative permeability | as §4 *Dielektrizitätszahl* |
| magnetische Flussdichte | magnetic flux density | |
| Selbstinduktion / Selbstinduktionsspannung / Induktionsgesetz | self-induction / self-induced voltage / law of induction | |
| Lenzsche Regel | Lenz's law | |
| Wirbelströme | eddy currents | |
| Kupferlackdraht / versilberter Kupferdraht | enamelled copper wire / silver-plated copper wire | |
| Festkondensator / gepolter Kondensator / Tantalkondensator | fixed capacitor / polarised capacitor / tantalum capacitor | |
| Trimmkondensator / Lufttrimmer / Luftdrehkondensator | trimmer capacitor / air trimmer / air-spaced variable capacitor | |
| Drehkondensator (neben *veränderliche Kondensatoren*) | rotary variable capacitor | where the German names it as one kind of *veränderlicher Kondensator*, so that the list does not read "variable capacitors in the form of variable capacitors"; alone it stays *variable capacitor* (§4, EC206) (kondensator_1) |
| Folien-Wickelkondensator / Folienwickelkondensator | wound film capacitor | |
| ESR / ESL | equivalent series resistance (ESR) / equivalent series inductance (ESL) | the symbols $R_\text{ESR}$, $R_\text{Isolator}$, $L_\text{ESL}$ stay |
| Antennenanalyzer / vektorieller Network Analyzer | antenna analyser / vector network analyser (VNA) | British *analyser*, as §11 |
| Zweikanal-Oszilloskop | dual-channel oscilloscope | |
| Zeigerdiagramm / rotierender Zeiger / Einheitskreis | phasor diagram / rotating phasor / unit circle | also the coloured lines B, C, D in the drawing: "the green phasor B" (phase, AB302); *Zeiger* of a meter stays *needle* |
| Bogenmaß / Winkelmaß (Grad) | radians / degrees | "im Bogenmaß angeben" → "give in radians" |
| Satz des Pythagoras / geometrische Addition | Pythagoras' theorem / geometric addition (geometric sum) | |
| Scheinwiderstand (neben *Impedanz*) | impedance | English has one word for both; where the German equates $|Z|$ with the *Scheinwiderstand*, the German word is named once: "is what German calls the *Scheinwiderstand*" (kondensator_2, spule_2); otherwise *Scheinwiderstand* → impedance (§5) |
| Übertrager oder Transformator, kurz Trafo (als Synonyme) | transformer | the German names in brackets where the text introduces them: "the *transformer* (in German *Übertrager* or *Transformator*, *Trafo* for short)" (uebertrager_1); *signal / power transformer* only where the German contrasts them (§4) |
| Leerlauffall | open-circuit case | as §3 *Leerlauf* |
| Stromdichte / Belastbarkeit von Wicklungen | current density / current rating of windings | the formula-sheet entry for $I = S \cdot A_\mathrm{Dr}$ (AC307) |
| frei verlegte Leiter | conductors installed in free air | VDE current ratings |
| Pulvereisenringkern / Ferritringkern | iron-powder toroidal core / ferrite toroidal core | |
| Weißblech | tinplate | screening |
| Unun-Übertrager / bifilar (verdrillt) gewickelt | unun transformer / wound bifilar (twisted) | |
| Stichwort (Formelsammlung) | keyword | "(siehe Formelsammlung – Stichwort: Induktiver Blindwiderstand)" → "(see the formula sheet – keyword: inductive reactance (*Induktiver Blindwiderstand*))" (DECISIONS.md) |
| Merkhilfe (Reim): Beim Kondensatoooor eilt der Strom vooor / Bei der Induktivitäääät kommt der Strom zu spääät | the German rhyme kept, English meaning in brackets: "(in the capacitor, the current leads)", "(in the inductance, the current comes too late)" | as the country-prefix mnemonics (DECISIONS.md) |
| Energiebandlücke / Bandlückenenergie | energy band gap / band-gap energy | halbleiter_2, diode_1 |
| Valenzband(energie) / Leitungsband / Valenzbandkante | valence band (energy) / conduction band / valence band edge | halbleiter_2 |
| Elementhalbleiter / Verbindungshalbleiter | elemental semiconductor / compound semiconductor | |
| dotierbar / n-Dotierung / p-Dotierung | can be doped / n-type doping / p-type doping | |
| Elektronenfehlstelle / Defektelektron | electron vacancy | what is called a *hole*; not the Germanism "defect electron" (halbleiter_2, transistor_1, transistor_2) |
| Diffusionsstrom / Feldstrom | diffusion current / drift current | *Feldstrom* is the current driven by the junction field, English *drift current* (halbleiter_2) |
| Raumladungszone | space-charge region | beside *Verarmungszone* → depletion region and *Sperrschicht* → depletion layer (§4), each as the German writes it (diode_2) |
| Sperrsättigungsstrom / Sättigungs-Sperrstrom / Sättigungsstrom | reverse saturation current / saturation current | $I_S$ (diode_1, transistor_1, transistor_2) |
| Temperaturspannung | thermal voltage | $U_T = kT/q$ |
| Sperrdurchbruch / Zener-Spannung / Kathodenstrich | reverse breakdown / Zener voltage / cathode bar | Zener diode (diode_1); *Z-Diode* → Zener diode (§4), also where the slides say the name stuck |
| Metall-Halbleiter-Übergang / Halbleiterübergang | metal-semiconductor junction / semiconductor junction | Schottky diode |
| pn-Diode / npn- / pnp-Transistor / n-Kanal / p-Kanal | pn diode / npn / pnp transistor / n-channel / p-channel | the case of the letters follows the German in each place (as *n-dotiert* in §4); the question bank writes NPN, PNP, N-channel because its German does |
| antiparallele Dioden | diodes in inverse parallel | as §14 *antiparallel geschaltete Dioden* (diode_2, AC405, AC406) |
| geklippt / Clipping | clipped / clipping | |
| Fotowiderstand | light-dependent resistor | as AC407 and §4 *LDR* |
| nicht-sperrender Kontakt | non-rectifying contact | the contacts of an LDR (diode_2) |
| galvanisch getrennt / galvanisch trennen | galvanically isolated / isolate galvanically | AC408 "galvanic isolation" |
| Masseschleife / Netzbrummen | earth loop / mains hum | British *earth loop*, not *ground loop* (diode_2) |
| gegen Masse / auf Masse liegen / Massepotential | to chassis / be connected to chassis / chassis potential | as §4 *Masse* and EC612 "chassis potential" (transistor_2, integrierte_schaltkreise, AC519, AC522) |
| Ausgleichsströme | equalising currents | AC408 |
| spannungsgesteuerte Stromquelle | voltage-controlled current source | transistor_1 |
| Stromverstärkung $B$ / Stromverstärkungsfaktor | current gain / current gain factor | *B*; the bank's *Gleichstromverstärkung* stays *DC current gain* (§3) |
| Leckstrom | leakage current | |
| Schalttransistor / Ansteuerung / Steuerspannung | switching transistor / drive / control voltage | transistor_1 slides |
| Serien-Gegenkopplung | series negative feedback | emitter resistor (transistor_2) |
| Regelbetrieb | normal operation | |
| (Relais) hat angezogen | (the relay) has pulled in | |
| Kanalwiderstand / Kanalstrom | channel resistance / channel current | AC514 "resistance of the channel" |
| Bulk-Schicht | bulk layer | under the channel of an insulated-gate FET |
| Source / Drain / Gate (with the German glosses *Quelle*, *Abfluss*, *Gatter*) | source / drain / gate | the German explains the English names; in English the gloss is not given back, only what the electrode does (transistor_2), as §14 *NTC / PTC (englisch …)* |
| Wehr / Steuerkanal / Steuerklappe | weir / control channel / control flap | the water analogy of the transistor (transistor_1) |
| "Kleiner Radiomann" des Kosmos-Verlags | the "Kleiner Radiomann" (little radio man) kit published by Kosmos | the kit's name stays German with a gloss; *kit* tells the English reader what it is (transistor_1) |
| Merksatz *Pfeil Nach Platte* | Pfeil Nach Platte (arrow towards the plate) | German mnemonic for the PNP symbol kept, as the other mnemonics (DECISIONS.md) |
| HF-Abblockung / HF-Entkopplung (der Betriebsspannung) / Betriebsspannungsleitung | RF decoupling (of the supply voltage) / supply line | MMIC circuit (integrierte_schaltkreise) |
| Ersatzwiderstand / Widerstandsnetzwerk | equivalent resistance / resistor network | reihe_parallel_widerstand, AD106–AD110, AD114 |
| hintereinander geschaltet | connected one after the other | i.e. in series (reihe_parallel_widerstand) |
| Bruchrechnung (nach den Regeln der) | (using the rules for) working with fractions | |
| Methode des scharfen Hinsehens | solving by inspection | the established English phrase for reading a result off the values without calculating (reihe_parallel_widerstand tip) |
| gemischte Schaltung(en) / gemischte Schaltungstechnik | series-parallel circuit(s) / series-parallel combinations | slide headings *Gemischte Schaltungen*, captions *Gemischte Schaltung - Variante 1* (reihe_parallel_widerstand, reihe_parallel_kondensator) |
| Zwei Parallel und dazu einer in Reihe / Zwei in Reihe und dazu einer Parallel | two in parallel, plus one in series / two in series, plus one in parallel | slide headings, "Variant 1: …" |
| Gesamtbelastbarkeit / Einzelbelastbarkeit | total power rating / individual power rating | as ED107 |
| Teilströme | branch currents | of a parallel connection (AD106) |
| Grenzfall / Schleifer (Potenziometer) | limiting case / wiper | as *Schleifkontakt* (AD109) |
| Maschenregel / Knotenregel / Masche / Knotenpunkt / Kirchhoff'sche Gesetze | loop rule / junction rule / loop / junction / Kirchhoff's laws | reihe_parallel_widerstandsnetz_2 slides |
| Spannungsteilerverhältnis | divider ratio | brueckenschaltung, AD111 |
| abgeglichene Brücke / abgleichen / Brückenspannung | balanced bridge / balance / bridge voltage | $U_\mathrm{AB}$ (brueckenschaltung, AD112) |
| Wheatstone-Messbrücke / Messbrücke nach Wheatstone / Widerstandsmessbrücke | Wheatstone bridge / Wheatstone bridge / resistance measuring bridge | the Pontavi instrument: "Wheatstone resistance measuring bridge (Pontavi)" |
| Messwerk | meter movement | the moving-coil movement in the bridge diagonal |
| Multiplikator / Messbereichsmultiplikator (Messbrücke) / Großer Drehknopf | multiplier / range multiplier / large knob | brueckenschaltung indepth |
| Messpunkt (A, B) | measuring point | brueckenschaltung, AD111–AD113; *gegen Masse gemessen* → "measured with respect to chassis" (§14 *gegen Masse*) |
| Durchschlag (Kondensator) | breakdown | as *Durchschlagsfeldstärke* (§14) |
| Vorsilbe (nano, Kapazitätswerte) | prefix | as *Einheitenvorsatz* (§3) |
| Endstufennetzteil | power supply of a power amplifier | photo caption (reihe_parallel_kondensator) |
| Teilabschnitte (zwischen Anzapfungen) | sections (between the taps) | reihenschaltung_spule |
| komplexe Größe / Realteil / Imaginärteil / komplexe Ebene | complex quantity / real part / imaginary part / complex plane | $Z = R + jX$ (reihe_parallel_gemischt) |
| Wirkwiderstand $R$ (neben Blind- und Scheinwiderstand) | resistive part, or simply the resistance $R$ | introduced once as "the resistive part, or simply the resistance $R$", afterwards *resistance*; *Scheinwiderstand* $|Z|$ → "the magnitude of the impedance, $|Z|$, which German calls the *Scheinwiderstand*", as §14 *Scheinwiderstand* and AD104/AD105 (reihe_parallel_gemischt) |
| Labornetzgerät / Strombegrenzung | laboratory power supply / current limiting | innenwiderstand |
| Quellenspannung $U_q$ / Spannungsfall | source voltage / voltage drop | innenwiderstand, spannungsquelle |
| Spannungsanpassung / Stromanpassung (Konstantspannungsquelle / Konstantstromquelle) | voltage matching / current matching (constant-voltage source / constant-current source) | as AB203, AB204 |
| Sinusgenerator / Ausgangsbuchse | sine-wave generator / output socket | |
| 3-adrige Leitung / Aderfarben / Aderkennzeichnung | 3-core cable / core colours / core identification | EK205 "core identification colours" (*Adernkennfarben*, §12) |
| Haussicherung | fuse in the house wiring | spannungsquelle slides; not "household fuse", which a British reader takes for the plug fuse |
| Kontroll-Leuchtdiode / beleuchtetes Anzeigeinstrument | indicator LED / illuminated meter | netzgeraet_1 |
| äußerer Schleifkontakt (Schukostecker) | outer sliding contact | the earthing contact of the Schuko plug (netzgeraet_1) |
| durchgebrannte Sicherung / Schmelzsicherung (mit Draht) | blown fuse / fuse (in which a thin wire melts) | *Schmelzsicherung* stays *fuse* (§12), not "wire fuse"; *thermische Abschaltung* → thermal shutdown, as ND108 |
| Auslösezeit / Abschaltzeit / Einschaltstrom / Nennstrom / Kennzeichen (Sicherung) | tripping time / breaking time / inrush current / rated current / marking | table of fuse characteristics: flink F / mittelträge MT / träge T → fast-acting / medium time-lag / time-lag, markings unchanged (§12) |
| Akkumulator (Akku) neben Batterie | rechargeable battery beside (non-rechargeable) battery | where the German contrasts the two, as ND110, NK306; where only rechargeable batteries are meant (akku), plain *battery* (DECISIONS.md) |
| Tiefentladung / Stromentnahme / Mindestspannung | deep discharge / drawing current / minimum voltage | |
| Bleiakku / Bleibatterie / NiCd / NiMH / Lithium-Ionen / LiFePO4 | lead-acid battery / nickel-cadmium (NiCd) / nickel-metal hydride (NiMH) / lithium-ion / lithium iron phosphate (LiFePO4) | |
| Kfz-Sicherung / Anschlussbox / verpolungsgeschützt | automotive fuse / connection box / reverse-polarity-protected | batterien_und_akkus photo caption |
| durchgestrichenes Mülltonnensymbol / Hausmüll | crossed-out wheelie bin symbol / household waste | |
| Batteriefach / Fieldday (Kurstext) | battery compartment / Field Day | as *Fieldday-Contest* → Field Day contest (§2) |
| Nennspannung / Zellnennspannung / Verschaltung (4S1P) | nominal voltage / nominal cell voltage / configuration (4S1P) | the 4S1P / 4S2P codes unchanged |
| Balancer / Balanceranschluss / Batteriemonitor / Balance-Stecker | balancer / balancer connector / battery monitor / balance connector | akku |
| Entladestrom / Entladezeit / entnehmbare Ladungsmenge | discharge current / discharge time / usable quantity of charge | akku, AB211 |
| Photoelement / Strang (Solarmodul) / Solarzellenverbund | photovoltaic cell / string / interconnected solar cells | as AD301 "strings" (photovoltaik) |
| photoelektrischer Effekt / photovoltaischer Effekt | photoelectric effect / photovoltaic effect | photovoltaik, AB212 |
| Spannungswandler / Hochsetzsteller / Tiefsetzsteller / Buck-Boost-Converter | voltage converter / step-up (boost) converter / step-down (buck) converter / buck-boost converter | *Step-UP-Wandler (Hochsetzsteller)* → "step-up converter (boost converter)"; *DC/DC-Wandler* → DC–DC converter (§5, AB213) |
| Einweggleichrichtung / Lastspannung | half-wave rectification / load voltage | gleichrichter_1; *Halbwelle* → half cycle (§3) |
| Leerlaufspitzenspannung / Sicherheitsaufschlag | open-circuit peak voltage / safety margin | gleichrichter_2, AD303, AD304 |
| LC-Siebglied | LC smoothing filter | as *Siebglied* (§5) |
| Diodenringmischer | diode ring mixer | brueckengleichrichter tip |
| Bauformen (Brückengleichrichter) / Anschlussfolge | package styles / order of the terminals | as *Bauform* (§14) |
| Brummton / AC-Kopplung / galvanische Kopplung (Oszilloskop) | hum / AC coupling / DC coupling | restwelligkeit |
| Schaltnetzteil (engl. switched-mode power supply) | switch-mode power supply | the German gloss only gives the English term and is dropped (bracket rule) (schaltnetzteil_1) |
| Ferritkernübertrager | ferrite-cored transformer | |
| Regelbarkeit / Ausfallwahrscheinlichkeit / Unterhaltungselektronik | regulation ("gute Regelbarkeit" → good regulation) / probability of failure / consumer electronics | schaltnetzteil_1 |
| Wo Licht ist, ist auch Schatten | there is no light without shadow | |
| Schaltzeit / Energietransport / Rückführung / Steuerblock (Schaltnetzteil) | switching time / transfer of energy / feedback / control block | schaltnetzteil_2; *der leitende Zustand des Schalters wird verändert* → "the time for which the switch conducts is varied" |
| Netzspannungspotentiale / Netztrennung | mains potentials / mains isolation | as *galvanische Trennung* → galvanic isolation (§5) |
| Störspektrum / (ungenügend) entstört | interference spectrum / (not adequately) suppressed | as §12 *Bürstenmotor (schlecht entstört)* (schaltnetzteil_2, AD312, AD313) |
| EMV-Filter / Funkentstörfilter / leitungsgebundene Störungen | EMC filter / radio interference suppression filter / conducted interference | |
| *Merke:* | *Remember:* | as in the earlier units (stromkreis, kondensator_2) |
| Referenzspannung / Spannungsreferenzquelle / Regelverhalten | reference voltage / voltage reference / regulation | spannungsstabilisierung; *unerwünschte Schwingungen im Regelverhalten* → the regulation "can break into unwanted oscillation" |
| diskret aufgebaute Spannungsstabilisierung / linear geregelt | voltage stabiliser built from discrete components / linear regulated | *Spannungsstabilisierung* as a circuit → voltage stabiliser, as AD321; as a technique → voltage stabilisation (§5) |
| systembedingt | by its (their) very nature | "The efficiency of linear voltage regulators is, by their very nature, often very low" (spannungsstabilisierung) |
| Fernspeiseweiche oder englisch BIAS-T / BIAS-T (Kurstext) | bias tee (remote DC feed) | the German's "oder englisch" gloss only gives the English term and is dropped; "(remote DC feed)" as AD322, at first mention and in the figure caption; the slide bullet *Englisch: BIAS-T* → "Also called a remote DC feed"; afterwards plain *bias tee* (fernspeiseweiche); §5 *Fernspeiseweiche / Bias-T* |
| abgesetzter Vorverstärker / Empfangskonverter | remotely mounted preamplifier / receive converter | fernspeiseweiche |
| Gleichspannungsversorgung(sleitung) / Versorgungsgleichspannung / DC-Anschluss / DC-Seite | DC supply (line) / DC supply voltage / DC connection / DC side | fernspeiseweiche |
| HF-Nutzfrequenz | wanted RF frequency | as §13 *Nutzfrequenz* → wanted frequency |
| Feinsicherung / TR5 / Diazed / Neozed / Hochspannungssicherung | miniature fuse / TR5 / Diazed / Neozed / high-voltage fuse | type names unchanged; *KFZ-Sicherung Flachstecksicherungen* → automotive blade fuses (sicherungen) |
| kommerzielle Funkgeräte | commercially made radios | factory-built, as opposed to home-built (sicherungen) |
| RC-Glied / RL-Glied / LC-Glied | RC network / RL network / LC network | simple filter sections (schwingkreis_1, schwingkreis_2) |
| Flanken (Filter) / steilflankiger | slopes / steeper | "ihre Flanken im Grenzbereich eher flach" → "their slopes are rather shallow around the cut-off"; *steile Flanken* of a crystal filter → steep skirts, as §5 *Flankensteilheit* |
| Frequenzweiche / Antennenweiche | frequency splitter / antenna splitter | high-pass and low-pass filters combined; the 2 m / 70 cm one is called a *diplexer* in both languages (schwingkreis_1) |
| Duoband-Antenne / UKW-Duoband-Gerät | dual-band antenna / VHF/UHF dual-band radio | 2 m and 70 cm; German *UKW* loosely covers both bands here, English names them both (schwingkreis_1) |
| Direktfunk / Relaisfunk | direct contacts / repeater operation | as §2 *Direktverbindung* |
| Bauvorschlag / Berechnungsprogramm | construction design / calculation program | computer *program* |
| Stimmgabel / Rechteckimpuls | tuning fork / square pulse | |
| Serienschwingkreis bzw. Reihenschwingkreis | series tuned circuit | English has one term for the two German synonyms; the slide bullet *Oder Serienschwingkreis* → "Called *Reihenschwingkreis* or *Serienschwingkreis* in German" |
| "Aus diesem Grund spricht man von einem Schwingkreis" | "This is why it is called a tuned circuit (in German *Schwingkreis*, literally "oscillating circuit")" | the German argues from its own word (*schwingen*, oscillate); *tuned circuit* does not carry the point, so the German word is named once with a literal gloss, as *Scheinwiderstand* (schwingkreis_1) |
| Betragsfrequenzgang | magnitude response | the magnitude of $Z$ or of $U_A/U_E$ against frequency (schwingkreis_1, schwingkreis_2) |
| Thomsonsche Schwingungsformel / Thomsonsche Schwingkreisformel | Thomson's formula | $f_0 = 1/(2\pi\sqrt{LC})$, after William Thomson (Lord Kelvin); formula-sheet topic "tuned circuits" (*Schwingkreise*) |
| Güte (im Englischen Q-Faktor) / Gütefaktor | Q factor | the bracket only gives the English term and is dropped; slide bullet *Auch Q-Faktor* → "Also called the quality factor" |
| unterkritische Kopplung / Durchlassbereich / Delle | under-critical coupling / passband / dip | coupled tuned circuits, with §5 *Kopplung (lose / kritisch / überkritisch)* and §6 *Durchlasskurve* → passband curve |
| Schwingquarz / Quarz (Werkstoff, SiO$_2$) | crystal / quartz | as §4 *Quarz*; the slide note *Im Englischen mit t: Quartz* → "In German spelt without the t: Quarz" (oszillatoren) |
| Wirkkette | chain of cause and effect | $U\uparrow \rightarrow C\downarrow \rightarrow f\uparrow$ (oszillator_vco) |
| Frequenzabweichung / Sollfrequenz | frequency error / nominal frequency | not *deviation*, which is the FM *Hub* (§7) (oszillator_tcxo_ocxo, oszillator_gpsdo) |
| geregelte Heizung / thermisch isoliertes Gehäuse | controlled heater / thermally insulated case | OCXO |
| Rubidium-Frequenznormal | rubidium frequency standard | |
| Satellitennavigationssysteme, englisch Global Navigation Satellite Systems (GNSS) | global navigation satellite systems (GNSS) | the German's English gloss is the English term itself (bracket rule) |
| GPS-synchronisierter Oszillator oder englisch GPS-Disciplined Oscillator (GPSDO) | GPS-disciplined oscillator (GPSDO) | bracket rule; as AD606 |
| Kurzzeitstabilität / Alterung (Bauelemente) | short-term stability / ageing | §5 *Langzeitstabilität* → long-term stability; British *ageing* |
| ein Impuls pro Sekunde | one pulse per second | GPS receiver output |
| Mit eingesetzten Werten: | Substituting the values: | solutions, also inside `\text{}` (AD225), as in earlier units |
| Chirp (*das englische Wort „Chirp" bedeutet wörtlich „Zwitschern"*) | chirp ("the English word "chirp" means the short, high call of a small bird") | the gloss explains the English word and stays, as *Ducting* above; it does not translate it back (oszillator_spannungsstabilitaet, AD609) |
| Verstärkerelement / Selbsterregung | amplifying element / self-excitation | oscillator condition, with §5 *Schleifenverstärkung* (oszillator_schaltungen, AD613) |
| kapazitiv rückgekoppelt (Dreipunktoszillator) / kapazitiver Spannungsteiler | capacitive-feedback (three-point oscillator) / capacitive potential divider | AD614, AD616, AD617 |
| Oszillator / Verstärker in Kollektorschaltung (Emitterschaltung) | common-collector (common-emitter) oscillator / amplifier; "in common-collector configuration" | AD401, AD409, AD617; captions *Bipolartransistor in Emitterschaltung* → "Bipolar transistor in common-emitter configuration" |
| wechselspannungsmäßig / signalmäßig (für Wechselspannung) | as far as AC is concerned / as far as the signal is concerned (for AC) | "der Kollektor liegt wechselspannungsmäßig auf Masse" → "the collector is connected to chassis as far as AC is concerned" (oszillator_schaltungen, kollektorschaltung) |
| Oberschwingungen / Obertöne (Quarz) | overtones | a crystal operated *auf einer Oberschwingung* → "on an overtone", as AD617 "on its third overtone"; for signals *Oberschwingung / Oberwelle* stays *harmonic* (§3) (oszillator_schaltungen) |
| auskoppeln / Auskopplung (Signal) / Ein- und Auskopplung | couple out / coupling out / coupling in and out | AD615 "coupled out" |
| Phaseninkrement / Adresszähler / Wertetabelle / Sinustabelle | phase increment / address counter / table of values / sine table | DDS, with §14 *Tuning Word / Lookup-Tabelle* (oszillator_dds) |
| D/A-Wandler | D/A converter | as §8 *D/A-Umsetzer (DAC)* (oszillator_dds) |
| Phasendetektor | phase detector | as §5 *Phasenvergleicher*, AD701 (AD703) |
| eingerastet (locked) | locked | the bracket only gives the English word and is dropped; *stabiler Zustand* → stable state, as AD702 (oszillator_pll) |
| Teilverhältnis / Teilerfaktor / Teilfaktor (PLL) | division ratio | all three German variants, as §5 *Teilerverhältnis* (oszillator_pll, AD703) |
| Vergleichsfrequenz (PLL) | comparison frequency | the frequency at the phase detector (oszillator_pll) |
| Verzerrerstufe / nichtlineare Verzerrerstufe | distorting stage / non-linear distorting stage | AF311 |
| Verdoppelung / Verdreifachung / Verneunfachung | doubling / tripling / multiplying by nine | multiplier stages; *ver-3-facht* (slides) → "multiplied by 3", keeping the digit |
| Zwischenstufe (Vervielfacher) / Frequenzen zwischen den Stufen | intermediate stage / frequencies between the stages | AF314; the slide's *Es werden Zwischenfrequenzen erzeugt* → "Frequencies are produced at the intermediate stages", not "intermediate frequencies", which is the IF (§6) (frequenzvervielfacher_2) |
| Gegenprobe | check | heading in worked solutions (frequenzvervielfacher_2 slides) |
| Lösung (Aufzählungspunkt unter der Überschrift *Lösungsweg*) | Working: | so that it does not repeat the heading "Solution" (mischer slides) |
| Hoch- / Heruntermischung / hochmischen / heruntermischen | up-conversion / down-conversion / mix up / mix down | mischer, transverter_1 |
| Betragsstriche / Fallunterscheidung | vertical bars (magnitude) / distinguishing two cases | the bars around $x$ that give its magnitude (mischer) |
| balancierter Ringmischer (Balance-Mixer) | balanced ring mixer | the bracket only gives the hybrid German-English name and is dropped; §5 *Balancemischer / Ringmischer* (mischer) |
| Mischprodukte höherer Ordnung | higher-order mixing products | mischer |
| Sende-/Empfangsumschaltung | transmit/receive switching | converter vs transverter (transverter_1) |
| quarzstabilisierter Oszillator | crystal-controlled oscillator | as AF314 "crystal-controlled radio" (transverter_1) |
| Up-Konverter | up-converter | QO-100 (transverter_2) |
| Linearitätsabweichungen / Bandpasscharakteristik | departures from linearity / band-pass response | verstaerker |
| Strom-Verstärker / Spannungs-Verstärker (linearer) | (linear) current amplifier / voltage amplifier | kollektorschaltung, emitterschaltung |
| Arbeitspunkt (engl. bias, Vorspannung) / Arbeitspunkt (BIAS) / BIAS-Spannungsteiler | operating point (bias) / bias potential divider | the gloss *engl. … Vorspannung* is dropped (bracket rule), "bias" kept as the English term; *BIAS* written in lower case |
| Eingangskennlinie | input characteristic | kollektorschaltung |
| Kollektor-Emitter-Strecke / Basis-Emitter-Strecke | collector-emitter path / base-emitter path | kollektorschaltung, emitterschaltung |
| Abblockkondensator in der Betriebsspannung (+) | decoupling capacitor on the supply voltage (+) | §5 *Abblockkondensator* |
| ausregeln (thermisch bedingte Änderungen) | compensate | kollektorschaltung, emitterschaltung |
| Emitterkondensator / den Emitterwiderstand überbrücken | emitter capacitor / bypass the emitter resistor | AD413–AD415 |
| ohne Arbeitspunktvoreinstellung | without a preset operating point; without its operating point being preset | AD406 (emitterschaltung) |
| gesperrter Transistor / sperren | transistor cut off / cut off | AD406 |
| Zur Erinnerung: | As a reminder: | solutions AD402, AD403, AD405 |
| A/B-Betrieb / Verstärkerklasse A/B (Kurstext) | class AB operation / amplifier class AB | the course text writes *A/B*, the question bank and the course's own list "A, B, AB und C" write *AB*; English writes *class AB* throughout, as AD416, AD422, AD423; the subscript $I_\mathrm{A/B}$ stays (verstaerker_klasse) |
| Verstärkerklassen / Klasse-D-, Klasse-E-, Klasse-F-Verstärker / Klasse J, Klasse S | amplifier classes / class D, class E, class F amplifiers / class J, class S | lower-case *class* in running text, as §5 *A-Betrieb* → class A operation; capitalised only at the start of a sentence, bullet or table cell |
| Ruhearbeitspunkt / Arbeitsgerade / zwischen Sperrung und Sättigung / Sperrpunkt | quiescent operating point / load line / between cut-off and saturation / cut-off point | verstaerker_klasse; *Arbeitspunkt* → operating point (§5) |
| Stromflusswinkel ($\Theta$) | conduction angle | verstaerker_klasse |
| Steuergröße / Ausgangsgröße (Kennlinie) | control quantity / output quantity | the transistor characteristic (verstaerker_klasse) |
| Einsetzen des Kollektorstroms | onset of collector current | "Geringe Vorspannung bis zum Einsetzen des Kollektorstroms" → "Small bias, up to the onset of collector current" (verstaerker_klasse) |
| Stromimpulse / konstante Hüllkurve | current pulses / constant envelope | class B and class C operation (verstaerker_klasse) |
| Gegentaktschaltung, im Englischen *push-pull amplifier* | *push-pull* circuit | the gloss only gives the English term and is dropped (bracket rule); §5 *Gegentaktschaltung* (verstaerker_klasse) |
| zugeführte / aufgenommene Gleichstromleistung / Gleichstrom-Versorgungsleistung / Gleichspannungsleistung | DC input power supplied / DC power drawn / DC supply power / DC power | AF401 "the DC input power supplied"; $P_\mathrm{DC}$, $P_\text{zu}$, $P_\text{ab}$ stay (verstaerker_wirkungsgrad, verstaerker_klasse, AD429, AD430) |
| Oszillation/Pfeifen (Rückkopplung Mikrofon–Lautsprecher) | oscillation/howling | acoustic feedback in a PA system (verstaerker_eigenschwingung tip); *howling* (howl-round) is the English word for this, *whistle* is a receiver's beat note (*Pfeifstellen*) |
| Hilfsmittel (das, was moduliert wird: Rauch, elektrische Schwingung) | medium | what telegraphy influences to carry a message, before the text names it the *carrier* (rauch_und_morsezeichen); not *aid*, which is *Hilfsmittel* in the examination sense (above) |
| Morsezeichen geben | send Morse characters | "Man spricht davon, Morsezeichen zu *geben*" → "This is called *sending* Morse characters" (rauch_und_morsezeichen) |
| Modulationsarten (AM, FM … als Begriff) | types of modulation | as NE102 "types of modulation"; on a radio's *Mode* switch and in its table, *mode* (§7) (modulationsarten, trxmodulation) |
| Sprachsignal / Sprachspektrum / Audiospektrum | speech signal / speech spectrum / audio spectrum | sprachsignale |
| Phasenlage | phase | unmodulierter_traeger |
| Additionstheoreme für Winkelfunktionen | trigonometric addition formulas | am slides |
| ausschlagen (Anzeige eines Spektrums) | show a peak | am indepth |
| unteres / oberes Seitenband, englisch lower / upper sideband | lower sideband (LSB) / upper sideband (USB) | the German gloss is the English term and is dropped; the warning that *USB* does not stand for *unteres Seitenband* is kept as information about German usage (DECISIONS.md) (ssb) |
| Einseitenbandmodulation, gebräuchlicher englisch single-sideband modulation | single-sideband modulation (SSB) | bracket rule (ssb, ssb_2) |
| Trägerfrequenzauslenkung (Frequenzhub) / Frequenzauslenkung / Trägerauslenkung | deviation of the carrier frequency (frequency deviation) / frequency excursion / carrier deviation | EE306 "the deviation of the carrier frequency" (fm_2, fm_3); *Frequenzabweichung (Frequenzhub)* of an FM carrier is likewise "frequency excursion (frequency deviation)", not the oscillator's *frequency error* (fm_2) |
| Lautstärkeinformation | volume information | EE306 |
| Hub-Regler | deviation control | EE305 "deviation setting" (fm_2) |
| Schmalband-FM (englisch Narrow-FM, kurz NFM) | narrowband FM (NFM) | bracket rule, as §2 *Schmalband-FM* (fm) |
| Spitzen-Hüllkurvenleistung (PEP) / Tastkopfverhältnis | peak envelope power (PEP) / the probe's division ratio | as *Teilverhältnis (Tastkopf)* above (ssb_3, AI305, AI306) |
| Zweiton-Nutzsignal / Eintonsignal | two-tone wanted signal / single-tone signal | ssb_3 |
| Winkelmodulationstechniken / Phasensprung / Flanke (Rechteck) | angle modulation techniques / phase jump / edge | pm |
| Nutzsignal (das zu übertragende Signal $m(t)$ bei PM/FM) | information signal | as NE202/NE301 *Informationssignal*; *wanted signal* (§6) is the receiver's sense, against interference (pm) |
| vollständig ausgesteuert (AM-Träger bei $m = 1$) | fully modulated | the English phrase for 100 % modulation; *Aussteuerung* of a transmitter or amplifier stays *drive* (§14) (am_2) |
| Kanalleistungsmessung / Nachbarkanalleistungsmessung | channel power measurement / adjacent-channel power measurement | spectrum analyser functions (bandreite_3) |
| zus. Nutzungsbedingungen (Tabellenkopf, Anlage 1 AFuV) / Auszug | add. conditions of use / extract | bandbreite; as §14 *Nutzungsbestimmungen* |
| Dynamic Compressor / NF-Dynamikkompressor / Sprachkompressor | dynamic compressor / AF compressor / speech compressor | AE210 "AF compressor"; *NF-Sprachprozessor* stays *audio speech processor* (dynamik_kompressor_1, dynamik_compressor_2) |
| prägnant und durchdringend (Signal) | punchy and penetrating | dynamik_kompressor_1 |
| Geradeausempfänger ("Der Name kommt daher, dass …") | tuned radio frequency (TRF) receiver (in German *Geradeausempfänger*, literally "straight-through receiver") | where the German explains its own name (the frequency is not changed before the demodulator), the German word is named once with a literal gloss, as *Schwingkreis* above; otherwise plain *TRF receiver*, as EF102 (aufbau_empfaenger) |
| Selektivität (Trennschärfe) / Selektivität, also Trennschärfe / Nahselektion oder auch Trennschärfe | selectivity / close-in selectivity, or simply selectivity | German has two words for one English term; the bracket or *also* is dropped (bracket rule). *Nahselektion* → close-in selectivity, as AF111, AF115; where a slide lists *Selektivität* and *Trennschärfe* as two bullets, "better selectivity" / "sharper selectivity" (ueberlagerungsempfaenger_einfachsuper_1, _2) |
| hochohmiger Kopfhörer / träge (Kopfhörer) / Stromstöße | high-impedance headphones / sluggish / current pulses | crystal set (detektorempfänger) |
| Rundfunksender im Lokalbereich / Fernempfang von Sendern im Fernbereich | local broadcast stations / long-distance reception of distant stations | detektorempfänger |
| Eingangsfilterblock / Eingangsfilter | input filter block / input filter | superhet, filter ahead of the first mixer |
| Wortneubildung | coinage | *superheterodyne* (ueberlagerungsempfaenger_einfachsuper_1) |
| Lokal-Oszillator (LO) / Schaubild | local oscillator (LO) / diagram | ring mixer (mischer_2) |
| Ringschaltung / Ringmodulator / Dioden-Gleichrichter | ring circuit / ring modulator / diode rectifier | mischer_2; *Balancemischer, Ringmischer oder Ringmodulator* → "balanced mixer, ring mixer or ring modulator" |
| konzeptbedingt / prinzipbedingt | by its very nature / inherently | spiegelfrequenzen |
| Spiegelfrequenzstörungen | image-frequency interference | AF107, AF203 |
| Vorselektion (Empfänger) | preselection | as AF204 "The preselection"; *Preselektor* stays *preselector* (§6) (spiegelfrequenzen, doppelueberlagerungsempfaenger_doppelsuper) |
| CO (Quarzoszillator) / Funktionsblöcke | CO (crystal oscillator) / functional blocks | double-conversion superhet, as AF117 |
| Regelspannung … für die Steuerung der Eingangsempfindlichkeit (AGC) | a control voltage for controlling the input sensitivity (AGC) | where the German itself names the AGC after it; elsewhere *Regelspannung* → AGC voltage (§6) (doppelueberlagerungsempfaenger_doppelsuper) |
| Störunterdrückungsverfahren | interference-suppression methods | doppelsuper tip |
| Lösungsmöglichkeiten / 1. Lösung, 2. Lösung (Folien) | possible solutions / Solution 1, Solution 2 | two oscillator frequencies that are both correct; *Lösungsweg 1/2* for two methods to one answer stays "Method 1/2" (doppelueberlagerungsempfaenger_doppelsuper slides) |
| Überlagerungsmischung | heterodyne mixing | BFO (bfo_1 slides) |
| Hörfrequenz / Tonfrequenz (CW) | listening frequency / audio frequency | the pitch of the CW tone (bfo_2) |
| nichtlinearer Grenzbereich | (operation) at the edge of its range, in the non-linear region | "non-linear limit region" is not an English term (intermodulation_kreuzmodulation) |
| Grundsignale / Steigung / Schnittpunkt (IP3) | fundamental signals / slope / point of intersection | two-tone test and IP3 (intermodulation_kreuzmodulation) |
| Intercept Point dritter Ordnung / Intercept Point 3. Ordnung | third-order intercept point / 3rd-order intercept point | the digit kept where the German writes one; as §6 *Intercept-Punkt (IP3)* |
| Abschwächer (auch Attenuator genannt) / Dämpfungsglied (Attenuator) | attenuator | the bracket only gives the English word and is dropped (bracket rule); the slide heading *Attenuator* stays (vorverstaerker_daempfungsglied, intermodulation_kreuzmodulation) |
| Leistungsdämpfungsglied / ohmsches Dämpfungsglied / T- und π-Dämpfungsglied / PI-Konfiguration | power attenuator / resistive attenuator / T and $\pi$ attenuator / pi configuration | daempfungsglieder |
| Systemimpedanz / impedanzrichtiger Abschluss | system impedance / termination with the correct impedance | daempfungsglieder |
| Störimpulse | interference pulses | FM limiter (begrenzerverstaerker) |
| Antennenzuleitung / PTT-gesteuert | antenna feeder / PTT-controlled | preamplifier (vorverstaerker_daempfungsglied) |
| Low Noise Block Converter (LNB) | low-noise block converter (LNB) | as the German writes it, lower case as a term; §6 gives the longer *low-noise block downconverter* (low_noise_block) |
| Polarisationsrichtungen | polarisations | horizontal and vertical (low_noise_block) |
| S-Wert | S reading | "ein S-Wert von S9" → "an S reading of S9"; *S-Stufe* stays *S unit* (§2) (s_meter, AA114) |
| Grundrauschen oder Eigenrauschen | noise floor or internal noise | as §14 *Rauschflur* and §6 *Eigenrauschen* (s_meter tip) |
| Ansprechverhalten / Ansprechzeit / Abfallzeit (AGC) / Empfängerausstattung | response / attack time / decay time / the receiver's features | AGC Slow, AGC Normal, AGC Fast, AGC Off are menu labels and stay (agc_1) |
| Keramikresonatoren | ceramic resonators | AF208 |
| Regelkreis / Regelwirkung (AGC) | control loop / control action | "geschlossener Regelkreis" → "closed control loop"; *AGC-Regelspannung* (caption) → "AGC voltage", not "AGC AGC voltage" (agc_2) |
| Regelspannung (VCO einer PLL) | control voltage | the VCO's tuning voltage in a PLL demodulator; *AGC voltage* (§6) only where it controls the gain (demodulator) |
| Phasenregelschleife (inside a description of a PLL) | phase control loop | "In einer PLL wird ein VCO über eine Phasenregelschleife … gekoppelt" → "is locked … by a phase control loop", so the sentence does not read "In a PLL … via a phase-locked loop"; elsewhere §5 *phase-locked loop (PLL)* (demodulator) |
| aufmodulierte NF | the AF modulated onto the carrier | envelope detector, PLL (demodulator) |
| Rauschzahl … mittels Logarithmierung in Dezibel dargestellt / Rauschmaß (laut DIN) | noise factor … expressed in decibels as the *noise figure* / *Rauschmaß* named as the German term | §6 trap: the ratio is the noise factor, its dB value the noise figure; the DIN remark that the dB value is called *Rauschmaß* and that "diese Bezeichnung nicht sehr verbreitet ist" is about the German word and is kept as such ("this German term"), as DECISIONS.md *USB* (snr_rauschzahl). On slides *Rauschmaß* → noise figure |
| Pegeländerung der Rauschleistung / Bezugsbandbreite | change in level of the noise power / reference bandwidth | rauschen, AB409 |
| über das Band wandern | wander across the band | both stations chasing each other's frequency (rit) |
| Sprachfrequenzen gespiegelt (LSB) | speech frequencies inverted | rit tip |
| "Clarifier" / "CLAR RX" (Herstellerbezeichnung der RIT) | "Clarifier" / "CLAR RX" | manufacturers' control labels, quoted as printed; the function itself is §6 *clarifier* (rit) |
| Rauschsperre … Meist wird … der englische Begriff Squelch (Abkürzung: SQL) verwendet | squelch (abbreviation: SQL) | one English word for both; the sentence that only gives the English term is dropped (bracket rule) and the abbreviation moves to the first mention (squelch) |
| Sendepausen (Squelch einstellen) | pauses between transmissions | "so dass es gerade nicht mehr rauscht" → "so that the noise just disappears" (squelch) |
| Kerbe / "Daher auch der Name Notch-Filter" | notch / "hence the name notch filter" | *Notch-Filter (Kerbfilter)* → notch filter (bracket rule); the explanation of the name works in English as it stands (notchfilter) |
| feste Trägerkomponenten | steady carrier components | automatic notch filter (notchfilter) |
| impulsförmige Störungen | pulse-type interference | as EF214 (noise_reduction) |
| Kurzwellenfunkgerät | HF radio | photo caption (noise_reduction) |
| neu abgleichen / Abgleich / Abgleichanleitung | realign / alignment / alignment instructions | as §1.3 *Abgleicharbeiten* (frequenzmessung_1) |
| abgesetzte Drei (Anzeige) / vor dem Komma / Nachkommastellen | the separate three / before the decimal point / decimal places | frequency counter display; English writes a decimal point (frequenzmessung_1) |
| Frequenzmessbereich / Bedienungsanleitung | frequency measurement range / operating manual | frequenzmessung_1 |
| Perioden beziehungsweise Flanken oder Nulldurchgänge / direkt zählender Frequenzzähler | periods, or rather edges or zero crossings / direct-counting frequency counter | gate time (frequenzmessung_2) |
| Aktualisierung (Anzeige) / Notbehelf | updating / makeshift | frequenzmessung_2 |
| GPS-synchronisierter Oszillator (ohne Abkürzung) / … (GPSDO) | GPS-synchronised oscillator / GPS-disciplined oscillator (GPSDO) | as AI511 "synchronised to GPS"; where the German adds *GPSDO*, the abbreviation decides (frequenzmessung_2, frequenzgenauigkeit) |
| Frequenzgenauigkeit / relative Abweichung | frequency accuracy / relative deviation | *maximal zu erwartende Frequenzabweichung* → "maximum frequency error to be expected", as §14 *Frequenzabweichung* (frequenzgenauigkeit) |
| Abw. (Größe in Lösungsfolien, $\textrm{Abw.} = \qty{10}{\ppm}$) | Dev. | an abbreviated word naming a quantity, translated like `\text{Ordnung}` → `\text{order}`; the subscript in $f_{B,\mathrm{max},\text{Abw}}$ stays (frequenzgenauigkeit slides) |
| Lösungsweg Teil 1 / Teil 2 (Folien) | Solution, part 1 / Solution, part 2 | frequenzgenauigkeit slides |
| Hinweis bzgl. Umrechnung/Darstellung von 10er Potenzen | Note on converting and writing powers of 10 | the digit kept for the number check (frequenzgenauigkeit) |
| Gemessene Frequenz / Anzeigefrequenz / Messwert (Gegeben) | measured frequency / displayed frequency / reading | AI506, AI507, AI509 solutions |
| »das Komma schieben« | "move the decimal point" | AI506 |
| Vorüberlegung (Überschrift in Lösungen) | Preliminary consideration | AI510 |
| Malkreuz (im Block-Symbol des Mischers) | multiplication sign | aufbau_sender |
| Mischer fügt … zusammen | the mixer combines … | aufbau_sender; *mixing* stays the term for the process (§5) |
| Grundwelle (1. Harmonische) / Ordnungszahl | fundamental (1st harmonic) / ordinal number | nicht_sinus_signale, AJ205, AJ206 |
| Oberwelle (Kurstext, neben *Harmonische*) / Oberwellen allgemein / Oberwellenanteil | overtone / harmonics / harmonic content | where the course text sets *Oberwelle* against *Harmonische* (nicht_sinus_signale: the 1st *Oberwelle* is the 2nd *Harmonische*), *overtone*, with the German words named once: "*overtones* (in German *Oberwellen* or *Oberschwingungen*)"; $f_\mathrm{Oberwelle,N}$ stays. Where *Oberwellen* only means unwanted multiples of a frequency (filters, spectrum analyser, AI614 "harmonics"), *harmonics*, as §3 (DECISIONS.md) |
| Sprungstellen / Über- und Unterschwingen (Gibbs-Phänomen) | discontinuities / overshoot and undershoot | nicht_sinus_signale |
| Doppelseitenband-Signal mit unterdrücktem Träger (DSB) | double-sideband suppressed-carrier signal (DSB) | as AE206 (modulatoren) |
| Diodenring / Ringanordnung / gegenüberliegende Diodenpaare | diode ring / ring arrangement / opposite pairs of diodes | balanced modulator (modulatoren) |
| ausbalanciert / Trägerabgleich / Amplitudensymmetrie / Phasenabgleich | balanced / carrier balancing / amplitude balance / phase adjustment | modulatoren; *symmetrisch, also ausbalanciert* → "symmetrical, that is, *balanced*" |
| Gegentaktanregung | push-pull drive | modulatoren slides |
| Filtermethode (SSB) | filter method | modulatoren |
| Seitenbandfilter | sideband filter | AF305 |
| im Kapitel „Mischer II" | in the second chapter on mixers | chapter titles not yet translated; descriptive, as in earlier units (modulatoren) |
| breitbandiger Koppeltransformator | broadband coupling transformer | leistungsvertaerker |
| Auslegungsfrequenz (Pi-Filter) | design frequency | leistungsvertaerker |
| LDMOS (Laterally Diffused Metal-Oxide-Semiconductor) | LDMOS (*laterally diffused metal-oxide-semiconductor*) | lower case as an expansion (leistungsvertaerker) |
| BIAS-Spannung / Gate-Vorspannung | bias voltage / gate bias | lower case, as §14 *Arbeitspunkt (BIAS)*; $U_\text{BIAS}$ stays (leistungsvertaerker, AF420, AF423, AF424) |
| gleichspannungsmäßig / HF-mäßig (betrachten, entkoppeln) | (considered) as far as DC is concerned / for DC; (decoupled) as far as RF is concerned | as §14 *wechselspannungsmäßig*; *Gleichspannungsbetrachtung* (slides) → DC analysis (leistungsvertaerker) |
| frei schwebendes Gate / unterer Zweig (Spannungsteiler) / Einstellwiderstand | floating gate / lower arm (of the potential divider) / preset resistor | leistungsvertaerker, AF421, AF424 |
| Betriebsspannungszuführungen | supply lines | as §14 *Betriebsspannungsleitung* (leistungsvertaerker) |
| Kurzwellen-Verstärker / Kurzwellen-Endstufe | HF amplifier / HF output stage | KW → HF (leistungsvertaerker, parasitaere_schwingungen); AF420 "LDMOS HF PA" |
| TX-Anzeige / Parallel-Widerstand am Transformator | TX indicator / resistor in parallel with the transformer | parasitaere_schwingungen, AF416 |
| ALC-Anzeige / Sendeleistungs-Anzeige / NF-Aussteuerung | ALC indicator / transmit power indicator / AF drive | alc |
| TUNE-Taste / PWR-Regler / Handbuch (WSJTX) | TUNE button / PWR control / user guide | labels quoted as printed (alc indepth) |
| Spalten der Anlage 1 AFuV: Frequenzbereiche / Maximale Leistung / Zusätzliche Nutzungsbestimmungen gemäß B | "Frequency ranges" (*Frequenzbereiche*) / "Maximum power" (*Maximale Leistung*) / "Additional conditions of use under B" (*Zusätzliche Nutzungsbestimmungen gemäß B*) | the examination aid is the German annex, so the heading to look for follows in brackets, as the formula-sheet keywords (DECISIONS.md) (ausgangsleistung) |
| Hüllkurvenspitzenleistung | (German term for PEP) | kept as information about German usage: "The rarely used German term for PEP is *Hüllkurvenspitzenleistung*" (ausgangsleistung); §7 *Spitzenleistung (PEP) / Hüllkurvenspitzenleistung* → peak envelope power |
| effektive Wirkleistung … während einer Periode … (Definition der PEP) / im Mittel an einen reellen Abschlusswiderstand | average real power … during one cycle … / the average power … into a resistive termination | as EB501 (ausgangsleistung, senderausgangsleistung) |
| HF-Tastkopf / HF-Messkopf | RF probe / RF measuring head | AI605, AI608 (sender_messungen) |
| Forward-Spannung (Diode) | forward voltage | as §4 *Durchlassspannung* (sender_messungen) |
| Senderabschluss | transmitter termination | sender_messungen |
| Spannungsverdoppler / Spitze-Spitze-Detektor / doppelte Spitzenwertgleichrichtung | voltage doubler / peak-to-peak detector / double peak rectification (rectifier) | AI606, AI607 (sender_messungen) |
| berechnet (in Lösungsfolien, neben *gegeben / gesucht*) | calculated | sender_messungen slides |
| auf den Holzweg geraten | go astray | AF414 |
| (Emitter) unbeschaltet | no external circuitry (at the emitter) | as §13 *Beschaltung* (AF414) |
| Störung / störende Beeinflussung (Kurstext, gegenübergestellt) | interference / breakthrough | where the course sets them apart (limits exceeded vs. limits kept but equipment upset by the wanted signal); German words named once: "interference (in German *Störung*) and breakthrough (*störende Beeinflussung*)"; slide heading *Störende Beeinflussung* → Breakthrough. The question bank keeps *interference* for both (EJ103, EJ110, EJ112) (DECISIONS.md) (stoerungen_vermeiden, stoerungen_elektronischer_geraete_1) |
| Beeinflussung / beeinflussen (ohne *störend*) | effect / affect | "verschiedenen Beeinflussungen elektronischer Geräte" → "electronic equipment can be affected in various ways" (stoerungen_elektronischer_geraete_1, _2) |
| Übersteuerung (Empfänger) / Übersteuerung (Sender, Verstärker) | overloading / overdriving | EJ103, EJ106, EJ107 "overloaded"; EJ213, AJ207 "overdriven" |
| Abschlusswiderstand oder künstliche Antenne (Synonyme der Dummy Load) | termination or artificial antenna | dummy_load_1; §11 *Dummy Load* |
| induktionsarme Widerstände / Anzapfung / Masseanschluss (Dummy Load) | resistors with as little inductance as possible / tap / chassis connection | AI603's *erdnahes Ende* stays "earthed end" (§11) (dummy_load_2) |
| Teilspannung / Teilungsverhältnis (Spannungsteiler) | partial voltage / divider ratio | as *Spannungsteilerverhältnis* (dummy_load_2) |
| *Anzeige:* (Werbung im Kurstext) | *Advertisement:* | trap: *Anzeige* is otherwise a reading or display (§11) or a BEMFV notification (§1.4) (dummy_load_2) |
| DARC-Verlag / Bausatz | DARC-Verlag / kit | the publisher's name stays (dummy_load_2) |
| Verfügung 33/2007 (der BNetzA) / Verfügung 33 von 2007 | Order 33/2007 / Order 33 of 2007 | as *Verfügung 13/2005* (§1.2) (unerwuenschte_aussendungen_3) |
| Oberwellendämpfung (Bildunterschrift) | harmonic attenuation | captions 918, 1140 (unerwuenschte_aussendungen_3) |
| maximaler Sendesignalspitzenpegel des Senders (PEP) / maximaler Sendesignalpegel | maximum peak level of the transmitter's transmitted signal (PEP) / maximum transmitted signal level | AJ224, AJ225 "maximum PEP of the transmitter" (unerwuenschte_aussendungen_3) |
| Oberwellen bzw. Harmonische (engl. harmonics) (Spektrumanalysator) | harmonics | the German pairs its two words and glosses them with the English one, which is all English needs (bracket rule); *overtone* only where the text contrasts the two (§14 *Oberwelle*) (unerwuenschte_aussendungen_3) |
| CE-Erklärung / ETSI Norm EN 301783 | CE declaration / ETSI standard EN 301783 | unerwuenschte_aussendungen_3 |
| Einstreuungen von NF-Signalen (Netzversorgungsseite) | AF signals coupled in (on the mains supply side) | AJ223 (unerwuenschte_aussendungen_3) |
| UKW-Rundfunk / UKW-Rundfunkbereich / UKW-Radiosender (Kurstext) | VHF FM broadcasting / FM broadcast band (VHF) / FM broadcast stations (VHF) | as §10 *Ultrakurzwelle (UKW)*; AJ204 "FM broadcast band" (unerwuenschte_aussendungen_2, _3, stoerungen_vermeiden) |
| Bandstoppfilter (Bandsperren) | band-stop filters | the bracket only gives the other German name and is dropped (AJ208) |
| *Ober*schwingungen (Hervorhebung der Vorsilbe) | *harmonics* | the German stresses *Ober-* ("upper"); English *harmonics* has no such prefix, so the whole word is italicised (AJ208) |
| Funkstörungsannahme / Funkstörannahme (Folie) | radio interference reporting service (Funkstörungsannahme) | the slide's variant spelling written as the service's name; §1.2 (stoerungen_vermeiden, empfangsstoerungen) |
| Referenten für elektromagnetische Verträglichkeit (DARC) / Referat für EMV / Distrikte | electromagnetic compatibility officers / department for electromagnetic compatibility / districts | as §1.2 *EMV-Beauftragter des RTA* → EMC officer; *Ortsverband* → local club (stoerungen_vermeiden, empfangsstoerungen) |
| Jetzt Mitglied im DARC werden! | Become a DARC member now! | link text, as in earlier units |
| Konfliktfall / Leib und Leben / Sachen von bedeutendem Wert | case of conflict / life and limb / property of considerable value | BNetzA powers (stoerungen_vermeiden) |
| Garagentorsteuerung / Funk-Autoschlüssel / LED-Leuchten mit kapazitiven Sensoren | garage door control / radio car key / LED lights controlled by capacitive sensors | stoerungen_elektronischer_geraete_1 |
| Mantelwellen-Sperren (Verdrosselung) / Gleichtaktströme / Klappringkerne aus Ferrit, Klappferrite | common-mode chokes / common-mode currents / clip-on ferrite cores, clip-on ferrites | as §12 *Mantelwellendrossel*, *Klappferritkern*; "*Mantelwellen-Sperren (Verdrosselung)* von Zuleitungen" → "*choking leads with common-mode chokes*", not a bracketed "(choking)" (stoerungen_elektronischer_geraete_1) |
| Aussetzer / Artefakte / Verstummen (DAB, DVB-T) | dropouts / artefacts / muting | British *artefacts* (stoerungen_elektronischer_geraete_2) |
| Längsimpedanz / Eigenresonanz / Leistungscharakteristik (HF-Stufe) | series impedance / self-resonance / power response | AJ214 (stoerungen_elektronischer_geraete_2) |
| Powerline Communication / Afu-Bänder | powerline communication / amateur bands | empfangsstoerungen slides |
| Sicherungen ausschalten (Störungssuche im Haushalt) | switch off circuits at the fuse box | empfangsstoerungen slides; cf. §14 *Haussicherung* |
| Standort des Operators / Remote-Standort / Bedienteil des Operators / Block 1–3 | operator's location / remote site / operator's control unit / Block 1–3 | as §6 *Kontrollseite / Remoteseite*, *Bedienteil*; *Block* capitalised as a label, as AF703 (remote_station) |
| Laufzeiten im Netzwerk / Verarbeitungszeiten (Remote-Betrieb) | transit times in the network / processing times | AF709, AF710 (remote_station) |
| Logbuchführung / verpflichtende (angeordnete) Logbuchführung / Aufbewahrung des Logbuchs | keeping a log / mandatory log-keeping / keeping the log available | as §2 *angeordnete Logbuchführung* (BG102, BG103); slide headings (logbuch) |
| Logbuch-Software / Logdatei / Praxis-Tipp | logging software (logging program) / log file / practical tip | as §2 *Logbuchsoftware*; *Praxis-Tipp:* opening a tip box → "*Practical tip:*" (logbuch) |
| Universal Time Coordinated / Sommerzeit / Winterzeit | Universal Time Coordinated / summer time / winter time | the German's expansion of UTC is kept as written (see the unit report of nea_logbuch_und_qsl_karten); British *summer time* (logbuch, qsl_karten) |
| Amateurfunk-Diplom / Kurzzeitdiplom / Urkunde (DXCC) | amateur radio award / short-term award / certificate | as §2 *Diplom* → award (qsl_karten) |
| Vermittlungsbüro / QSL-Vermittlung (international "Bureau") / via-Feld | (QSL) bureau / QSL bureau / via field | the gloss *international "Bureau" genannt* only gives the English word and is dropped (bracket rule, DECISIONS.md) (qsl_karten) |
| Bildmotiv / persönliches Motiv (QSL-Karte) | picture / personal picture | the design on the front of a QSL card (qsl_karten) |
| DARC QSL-Service / DCL / Wavelog / Drittanbieter | DARC QSL-Service / DCL / Wavelog / third-party services | names of DARC services and software unchanged (logbuch, qsl_karten) |
| Datenträger | storage media | callbooks "auf Datenträger und online" (qsl_karten) |
| Digimode / Digimodes (Kurstext) / Digimode-Interface | data mode / data modes / data mode interface | §8 gives *digital mode / data modes*; in the course text, where the German writes *Digimodes* beside *digitale Übertragungsverfahren*, *data mode(s)* throughout, so that the two German words stay apart: *digitale Übertragungsverfahren* → digital transmission methods, or digital modes where operating is meant, as EJ217–EJ219 and alc (computersteuerung, digimode_ssb, 9600_port, automatische_empfangsberichte) |
| Informationsübertragung / Informationsübermittlung | transmitting information; conveying information | analog_vs_digital, morsetelegrafie |
| Zehnersystem oder Dezimalsystem / Dualsystem, Dualzahl (neben Binärsystem, Binärzahl) | base-ten system or decimal system / binary system, binary number | English has one word for *binär* and *dual*; the German pair is named once as German usage: "binary number system (in German also called *Dualsystem*)", slide *Neben Binärzahl wird auch Dualzahl gesagt* → "In German, a binary number is called *Dualzahl* as well as *Binärzahl*" (binaer) |
| Stelle / Stellenzahl / Breite (Dualzahl) / Ziffernvorrat zu Ende | position / number of digits / width / run out of digits | binaer; *Stellenwert* → place value (§3) |
| Fernschreiber / Funkfernschreiber (Gerät) | teleprinter / radio teleprinter | the device; *Funkfernschreiben* (the mode) stays *radioteletype* (§2); *RTTY des englischen Begriffes radio teletype* → "RTTY, for radio teletype" (computersteuerung) |
| Unterbrechung (BK) / Trennung innerhalb eines Durchgangs (BT, =) / Ende des Durchgangs (AR) / Ende der Sendung (SK) / Korrektur | Interruption (BK) / Separator within an over (BT, =) / End of over (AR) / End of transmission (SK) / Correction | Morse special characters (morsetelegrafie); *Unterbrechung der Sendung* → "Interruption of the transmission", as BB109 b; *Durchgang* → over (§2) |
| Abkürzungstabelle (Telegrafie): Bedeutung "Bitte (vom Englischen "Please")" … | the English meaning alone ("Please", "Report", "Thanks", "Very"); an origin that is not the meaning stays in brackets: CQ "General call (from "seek you")", SK "End of contact (from "Silent Key")" | DECISIONS.md; *Abkz. / Bedeutung* → Abbr. / Meaning; DE → "This is" (§14 *hier ist / von*); 73 → "Best regards"; *Trennzeichen* → separator (funkfernschreiben) |
| Startsound / Benachrichtigungstöne | start-up sound / notification sounds | computersteuerung, NF117 |
| Hardware-Modem / TNC (Terminal Node Controller) / Packet-Radio | hardware modem / TNC (Terminal Node Controller) / packet radio | computersteuerung, 9600_port |
| DATA-Port / DATA-Anschluss / 9600-Anschluss / 9600-Baud-Anschluss | DATA port / DATA port / 9600 port / $\qty{9600}{\baud}$ port | as NF115, EF219 "analogue data port … called a 9600 port"; §6 *Datenanschluss* |
| Audiopfad / Audio-Weg / De-Emphasis-Prozess | audio path / audio path / de-emphasis | 9600_port; §7 *Deemphasis* |
| Empfangsbericht (automatischer) / Skimmer-Stationen / Internetplattformen | (automatic) reception report / skimmer stations / internet platforms | EE405; the services' names (WSPRnet, Reverse Beacon Network, PSK Reporter) unchanged (automatische_empfangsberichte) |
| Repeaternetzwerk / Relaisverbund / Richtfunkanbindung | repeater network / repeater network / radio link | NE402 "repeater network" (digital_voice) |
| Raum (DV) / Zeitslot / Zeitschlitz | room / time slot / time slot | digital voice settings, with §8 *Sprechgruppe / Talkgroup*, *Reflektor*, *Color Code* (digital_voice, NE402) |
| TDMA (Time Division Multiple Access) oder Zeitmultiplexverfahren | TDMA (time-division multiple access) | the German name beside the English one is dropped (bracket rule); §8 (digital_voice) |
| Reaktions- und Haltezeit (ALC) | response and hold time(s) | digimod_uebersteuerung; *Ansprechzeit* of an AGC stays *attack time* (§14) |
| Farbtiefe / zeilenweise / Bewegtbilder | colour depth / line by line / moving pictures | SSTV, ATV (digimode_ssb); EE415 |
| Einstiegspunkt / HAMNET-Knoten mit Benutzerzugang / WLAN-Transceiver | access point / HAMNET node with user access / Wi-Fi transceiver | paketvermittelte_netzwerke; *WLAN* → Wi-Fi, as in earlier units |
| Teilnehmer (Netzwerk) / Netzwerkgerät / Heimnetz / Firmennetz | user / network device / home network / company network | paketvermittelte_netzwerke |
| Vorwahl / Ortsnetz / Schrägstrich / Netzmaske | area code / local exchange / slash / netmask | *Subnetzmaske* stays *subnet mask* (§8) (paketvermittelte_netzwerke) |
| Datenübertragungsrate / Datenrate (Kurstext) / binäre Zahlen, die sogenannten Bits | data rate / data rate / binary digits, known as bits | both German words are *data rate*, as EA106, EE401 and §8; *Bit* is the binary digit (datenuebertragungsrate) |
| Symbolfrequenz / Symbolgröße / Symbolgrenze / Symbolintervall / Symbolumschaltung | symbol frequency / symbol size / symbol boundary / symbol interval / switching between symbols | AE405, AE406, AE415 (symbole_symbolrate, psk, iq_verfahren, symbolumschaltung_bandbreite) |
| Bit/Symbol (Einheit: `\bit\per\text{Symbol}`, `\bit\per{Symbol}`, `\text{Symbol}\per\second`) | bit/symbol | the word in the unit is a running word and becomes *symbol*; the subscripts $R_\mathrm{Daten}$, $R_\mathrm{Symbol}$, $R_\mathrm{D}$, $R_\mathrm{S}$ stay (symbole_symbolrate, AA104, AE405, AE406) |
| Zeicheneinheiten (zur Übertragung des Informationsgehaltes) | signalling units | the slide's definition of a symbol (symbolumschaltung_bandbreite) |
| I/Q-Darstellung / I/Q-Ebene / I-Achse / Signalpunkt / Konstellationspunkt / Signalzustand | I/Q representation / I/Q plane / I axis / signal point / constellation point / signal state | iq_verfahren, mapping, psk, qam; §8 *Konstellationsdiagramm*; *I-Q-Diagramm* (caption) → I-Q diagram, as the German writes it |
| Zeigerdarstellung / Zeiger / komplexer Zeiger / Signalzeiger | phasor representation / phasor / complex phasor / signal phasor | as §14 *Zeigerdiagramm*; *Startzustand / Anfangszustand (des Zeigers)* → starting state / initial state (iq_verfahren, qam) |
| In-Phase Component / Quadrature Component (the German's English names of I and Q) | in-phase component / quadrature component | lower case, as §8 *I/Q*; "wird als $I$ für *In-Phase Component* bezeichnet" → "is called $I$, for *in-phase component*" (iq_verfahren) |
| Amplitudenumtastung (Amplitude Shift Keying, ASK) / Frequenzumtastung (Frequency Shift Keying, FSK) / Phasenumtastung (Phase-Shift Keying, PSK) / Quadraturphasenumtastung (QPSK) / Audio Frequency Shift Keying (AFSK) | amplitude-shift keying (ASK) / frequency-shift keying (FSK) / phase-shift keying (PSK) / quadrature phase-shift keying (QPSK) / audio frequency-shift keying (AFSK) | the German's bracketed English name only repeats the term and is dropped (bracket rule), the abbreviation stays; captions such as *ASK (Amplitude-Shift Keying) im zeitlichen Verlauf* keep the expansion, lower case: "ASK (amplitude-shift keying) over time"; *Quaternäre Amplitudenumtastung (Quaternary Amplitude-Shift Keying)* → "Quaternary amplitude-shift keying"; EE408 "audio frequency-shift keying (AFSK)" (ask_fsk_afsk, mapping, psk, afsk) |
| Mapper (Baustein) / Bitstrom / Bitkombination / Bitfolge (3-stellige) | mapper (building block) / bit stream / bit combination / (3-digit) bit sequence | mapping, qam |
| Entscheidungsbereich / Entscheidungsgrenze / Empfangswert (verrauschter) | decision region / decision boundary / (noisy) received value | QPSK applet (psk) |
| I/Q-Modulator / (mit dem I-Signal) gewichtet / Wertepaar $(I,Q)$ / Freiheitsgrade | I/Q modulator / weighted (by the I signal) / pair of values $(I,Q)$ / degrees of freedom | AE404 (qam) |
| Schweizer Taschenmesser (der Modulatoren) | Swiss Army knife (of modulators) | qam |
| DA-Wandler | D/A converter | as *D/A-Wandler* above (qam) |
| Sprechfunkgerät | voice radio | AFSK carried like speech (afsk) |
| Quelle / Senke (Informationsübertragung) / Irrelevanz | source / sink / irrelevance | "Redundanzen … oder Irrelevanzen" → "redundancy … or irrelevance" (quellencodierung) |
| Codec / Codec2 | codec / Codec2 | the codec's name unchanged (quellencodierung) |
| Prüfbit (*Parity Bit*) / *Even Parity* / *Odd Parity* | check bit (*parity bit*) / *even parity* / *odd parity* | the German's English terms in lower case, as §8 *Prüfbit / Paritätsbit* and AE411; *Gerade / ungerade Parität* stays even / odd parity (fehlererkennung, fehlerkorrektur) |
| Mehrbitfehler / Ein-Bit-Fehler / Restwahrscheinlichkeit / Ausweisnummer | multi-bit error / one-bit error / residual probability / identity card number | fehlererkennung |
| erneute Übertragung / Neuübertragung | retransmission | AE413 (kanalcodierung, fehlerkorrektur) |
| Paritätsprüfung schlägt fehl / erweiterter Hamming-Code | parity check fails / extended Hamming code | fehlerkorrektur; §14 *Hamming-Code* |
| "Im Englischen wird dieses Verfahren als *Forward Error Correction* (FEC) bezeichnet" | (dropped) | the sentence only gives the English term; the abbreviation moves to the first mention, "*forward error correction* (FEC)", as §14 *Rauschsperre … Squelch*; the slide bullet saying the same is dropped too (fehlerkorrektur) |
| *Spitzfindigkeit:* (opening an in-depth box) | *Splitting hairs:* | psk |
| Rauschenergie | noise energy | as the German says; the formula uses the noise power $P_\text{N}$ (shannon_hartley_gesetzt) |
| Bedienelemente der Applets ("Erneut übertragen") | English, German label in brackets: 'The button "Transmit again" (*Erneut übertragen*)' | the applets are still German (DECISIONS.md) (psk slides) |
| De-Mapper / I/Q-Demodulator / Sender-Prozess / Empfänger-Prozess | de-mapper / I/Q demodulator / transmitter process / receiver process | counterparts of §14 *Mapper*, *I/Q-Modulator*; *Sendekette* → transmit chain (sende_empfangsketten) |
| Zugriffsverfahren / Störanfälligkeit / Bandbreiteneffizienz / Spreizcode | access methods / susceptibility to interference / bandwidth efficiency / spreading code | §8 *Spreizcodierung*, EE411; *Kanalabstand* → channel spacing (§6) (vielfachzugriff) |
| Mobilfunksystem (GSM, UMTS, AMPS) / schnurloses Telefonsystem (DECT) / satellitengestütztes Navigationssystem | mobile phone system / cordless telephone system / satellite navigation system | vielfachzugriff |
| Zeitmultiplexverfahren / Frequenzmultiplexverfahren / Codemultiplexverfahren mit drei Signalen (captions) | time-division / frequency-division / code-division multiplexing with three signals | no abbreviation in the caption, so *…multiplexing*, as §8; *Time Division Multiple Access – Zeitmultiplexverfahren* on a slide → "Time-division multiple access" (bracket rule, as digital_voice) (vielfachzugriff) |
| Trägerabstand / Frequenzfehler / Dopplerverschiebung / frequenzselektives Fading | carrier spacing / frequency error / Doppler shift / frequency-selective fading | *Frequenzabweichungen zwischen Sender und Empfänger* as the cause of a *Frequenzfehler* → "frequency offsets between transmitter and receiver" (not *deviation*, §14 *Frequenzabweichung*) (ofdm) |
| Intersymbolinterferenz oder Symbolübersprechen | intersymbol interference, or crosstalk between symbols | §8 *Intersymbolinterferenz*, §14 *Übersprechen*; English has no second term, so the German synonym is rendered descriptively (ofdm) |
| Synchronisierung / zeitliche Übereinstimmung | synchronisation / time alignment | as §8 *Synchronisation* and AE407 "Establishing time alignment" (synchronisation) |
| Grundfrequenz (Polarmodulation) / Wellenzug | base frequency / cycle | here the carrier's starting frequency that the phase is shifted from, not the *fundamental* of a harmonic series (§3 *Grundfrequenz*); *der einzelne Wellenzug* is one cycle of the wave (polarmodulation) |
| momentane Amplitude / momentane Phase / Amplitudenpfad / Phasenpfad / aufprägen | instantaneous amplitude / instantaneous phase / amplitude path / phase path / impress (on) | polarmodulation; §14 *Hüllkurvenverstärker* → envelope amplifier, §6 *Schaltendstufe* → switching amplifier |
| Blick über den Tellerrand | a look beyond the syllabus | of a topic outside the examination (polarmodulation) |
| Sampling (in Deutsch … Probenahme) / Samples (Proben) | sampling / samples | the German gloss only translates the English word back into German and is dropped (bracket rule) (digitale_signalverarbeitung_einleitung) |
| Samplingrate oder Abtastrate | sampling rate or sample rate | the German names its two words for one quantity; English has two established names of its own, so the pair stays a pair (sampling_quantisierung); either alone is *sampling rate* (§8) |
| Abtastzeitpunkt / Abtastwert / Samplewert / Momentanzustand | sampling instant / sampled value / sample value / instantaneous state | sampling_quantisierung |
| Zeitachse / Wertachse (diskretisieren) / Zeitdiskretheit / Wertdiskretheit | time axis / value axis (make discrete) / discrete time / discrete values | sampling_quantisierung slides; *zeit-/wertkontinuierlich, -diskret* → continuous-/discrete-time, -value (§14, AF601–AF606) |
| Dimmer / Stufenschalter (mit 5 Stufen) | dimmer / step switch (with 5 steps) | the quantisation analogy (sampling_quantisierung, dac_adc) |
| Quantisierungsfehler / Quantisierungsstufen | quantisation error / quantisation steps | AF607 (dac_adc) |
| Zeitquantisierung / Wertquantisierung (Applet-Regler *Zeit-Sampling*, *Wert-Quantisierung*) | time quantisation (*Zeit-Sampling*) / value quantisation (*Wert-Quantisierung*) | the sliders of the applet `quantisierung_und_sampling`, which is still German; the German label in brackets (DECISIONS.md, applet labels) (sampling_quantisierung) |
| Abtasttaktgenerator / Taktgenerator / Taktrate | sampling clock generator / clock generator / clock rate | as AF620 and §8 *Abtastratengenerator* (dac_adc, anti_alias_rekonstruktionsfilter) |
| Nyquist-Shannon-Abtasttheorem / Nyquist-Bedingung | Nyquist–Shannon sampling theorem / Nyquist condition | en dash between the two names, as *Shannon–Hartley* (§8); *Nyquist criterion* avoided, as it usually names the ISI criterion (abtasttheorem, AF619) |
| Alias-Effekte bzw. Aliasing-Effekte / Aliase | aliasing effects / aliases | the German pair is one English term (bracket rule), as AF618 "aliasing effects" (abtasttheorem, anti_alias_rekonstruktionsfilter) |
| Moiré-Muster / räumliche Auflösung / Bildpunkte (Kamerasensor) | moiré pattern / spatial resolution / pixels | of a camera sensor, the everyday English word (anti_alias_rekonstruktionsfilter indepth) |
| HiFi-Frequenzbereich | hi-fi frequency range | abtasttheorem |
| Zaunpfahlproblem | fencepost problem | 16 levels, 15 intervals (dac_adc slides) |
| Stufen / Zwischenschritte / Abstände (D/A-Umsetzer) | levels / steps / intervals | AF610, AF611 "voltage levels", "step size" (dac_adc) |
| diskrete Fourier-Transformation (DFT) / Fast-Fourier-Transformation (FFT) | discrete Fourier transform (DFT) / fast Fourier transform (FFT) | as AF630; §8 *Fourier-Transformation* (fourier_transformation) |
| Sinussignal / Rechtecksignal / Sägezahnsignal / Dreiecksignal (Sinus, Rechteck, Sägezahn, Dreieck auf Folien) | sine-wave signal / square-wave signal / sawtooth signal / triangular-wave signal (sine wave, square wave, sawtooth, triangular wave) | as §3 *Sinusschwingung / Rechteck- / Dreieck- / Sägezahnschwingung* (fourier_transformation, AB404–AB407) |
| ungeradzahlige / geradzahlige / ganzzahlige Vielfache / Gleichanteil | odd / even / integer multiples / DC component | *ungeradzahlige Oberwellen* → odd harmonics (fourier_transformation) |
| Spektralanteil / Spektralspitze | spectral component / spectral peak | AB404–AB407 solutions |
| Finite / Infinite Impulse Response ("finite" (zu Deutsch endlich)) | finite / infinite impulse response | lower case as an expansion; the German gloss of *finite* is dropped (bracket rule) (digitale_filter) |
| gleitender Mittelwert / Faltungsoperation / Filterkoeffizienten / Abgriffe / Schieberegister / Eingangsspeicher | moving average / convolution / filter coefficients / taps / shift register / input memory | FIR filter (digitale_filter) |
| Mixed Signal Frontends / Dezimationsfilter | mixed-signal front ends / decimation filters | digitale_filter |
| Pufferspeicher (englisch "buffer") / Zwischenspeicherung (Buffer) | buffer / temporary storage (buffering) | the German gloss only gives the English word and is dropped (bracket rule) (latenz) |
| Laufzeit (Latenz) | propagation time | as AF637 "propagation time or delay"; *Verzögerung* → delay (latenz). Here, where the German derives the *Laufzeit* from the *Verzögerung*, not the bare §14 *Laufzeit* → delay, which would say "the delay results in a delay" |
| Filmkamera / Bilder pro Sekunde | film camera / pictures per second | the sampling analogy (digitale_signalverarbeitung_einleitung, abtasttheorem) |
| Aufruf nach Ziffern / Aufruf nach Ländern oder Kontinenten / Kontaktwünsche | calling by digit / calling by country or continent / requests for contacts | pile-up techniques (pileup); "*only number* 5" (nur Ziffer 5) → "(the digit 5 only)", as BE306 "the digit 3" |
| fortlaufende Nummer / Alter (Contest-Austausch) / Rangliste / Punktabzug | serial number / age / ranking list / points deducted | contest |
| Fuchsjagdsender / Zielpunkt / Wimpel / Zeitnehmer | foxhunt transmitters / finish / pennant / timing unit | ardf; *Fuchsjagd* named as the German word "(foxhunt)" where the text says what it is called in German-speaking countries |
| Rapportsystem RSV, V-Werte: Nur Synchronisation zu sehen / Großes Call lesbar / Große (Kleine) Details zu erkennen / Rauschfreies Bild | Only synchronisation visible / Large call sign readable / Large (Small) details recognisable / Noise-free picture | sstv |
| Leitstation (Notfunk) | net control station | notfunk |
| Notfunkreferat des DARC | DARC emergency communications department (Notfunkreferat) | as *Auslandsreferat*; *Notfallkommunikation* → emergency communications (notfunk) |
| Notfunkfrequenzen | emergency communications frequencies | IARU Region 1 band plans; BF109 "centres of activity for emergency communications" (notfunk) |
| "Notfall" oder "Emergency" (Rufworte im Notfall) | "Notfall" (German for "emergency") or "Emergency" | the German word is what is said on a national contact, kept with a gloss (DECISIONS.md, `<qso>` entry) (notfunk) |
| Amateurfunkmedien | amateur radio media | notfunk slides |
| Up- and Outer-Antenne | up-and-outer antenna | a dipole with one leg vertical (radiator) and one horizontal (radial); in quotation marks at first mention, as the German has it (rundstrahler) |
| Dipolschenkel / Schenkel / Teilstück (Dipol) | leg (of a dipole) / leg / section | *Schenkel* of a delta loop → side; *gleichlange Schenkel* of a G5RV → two legs of equal length (rundstrahler, dipol, antennenformen_2, antennenformen_3) |
| gegen Erde (oder eine Fahrzeugkarosserie) erregt | fed against earth (or a vehicle body) | as NG104 "a λ/4 vertical antenna fed against earth" (rundstrahler, antennenformen_2, antennenformen_3) |
| Ortsverbindungen (UKW) | local contacts | rundstrahler slides |
| End-Fed (kurz) / endgespeister Halbwellendipol (englisch: end fed half wave, EFHW) | end-fed / end-fed half-wave dipole (EFHW) | the German's English gloss is the English term itself and is dropped (bracket rule); the abbreviation stays, as the text goes on to use it (endgespeiste_antennen, antennenformen_2) |
| Stummel-Stabantenne | stubby rod antenna | DVB-T example (polarisation slides) |
| Poynting-Vektor | Poynting vector | EB305 (polarisation_2) |
| magnetische Ringantennen (Magnetic-Loops) / Magnetantennen / Magloop | magnetic loop antennas / magnetic antennas / mag loop | the bracket that only gives the English name is dropped (bracket rule) (antennenformen_2, polarisation_2) |
| elektrische Schleifenantenne | electric loop antenna | the full-wave loop as against the *magnetic* loop (verkuerzungsfaktor_2) |
| Keule (Strahlungsdiagramm) / hertzscher Dipol / Richtwirkung | lobe / Hertzian dipole / directional properties | with §9 *Hauptkeule*; *Richtwirkung* as a slide heading (antennenformen_2) |
| Sperrtopf / Kreuz-Yagi-Uda | sleeve / crossed Yagi-Uda | the λ/4 *Topf* of the *Sperrtopfantenne* (sleeve dipole, §9) is its sleeve; where *Sperrtopf* stands for the antenna, *sleeve dipole*, as EG107 (antennenformen_2) |
| Zeppelinantenne (Kurstext) | Zepp antenna, short for Zeppelin antenna | as AG120 and §9 *Zepp antenna*; the German name explains the airship story that follows, so the first mention says what *Zepp* is short for (antennenformen_3) |
| Mantelwellensperre (Abkürzung MWS) | common-mode choke (in German *Mantelwellensperre*, abbreviated MWS) | the drawings and AG123, AG124 use the German abbreviation (antennenformen_3) |
| Un-Un (1 zu 49) / Pigtail / Symbolbild | unun (1 to 49) / pigtail / illustrative photo | captions (antennenformen_3) |
| Erde als Gegenpol / Erdpotential | earth as the other pole / earth potential | antennenformen_2, antennenformen_3 |
| Verkürzungsfaktor (Kurstext) | shortening factor (antennas) / velocity factor (lines, cables) | where the course introduces it for lines including antenna wires: "the *velocity factor* $k_\mathrm{v}$ (for antennas usually called the *shortening factor*; German has one word for both, *Verkürzungsfaktor*)" (DECISIONS.md) (verkuerzungsfaktor_1, _2) |
| Vakuumlichtgeschwindigkeit / Überlichtgeschwindigkeit / Phasengeschwindigkeit / Gruppengeschwindigkeit | speed of light in a vacuum / faster than light / phase velocity / group velocity | verkuerzungsfaktor_1, _2 |
| Polyäthylen (Formelsammlung) | polyethylene (*Polyäthylen*) | the formula sheet's spelling in brackets, as a formula-sheet keyword to look for (DECISIONS.md); the questions write *Polyethylen* → polyethylene (verkuerzungsfaktor_2) |
| Anpassgerät bzw. Tuner | antenna tuning unit or tuner | as §9 *Antennenanpassgerät* (antenne_laenge_resonanz) |
| plattgedrückte Ganzwellenschleife | flattened full-wave loop | the folded dipole (antenne_laenge_resonanz) |
| Anpassung (Folienüberschrift: Dipol auf die Frequenz bringen) | adjustment | where it means bringing a dipole to the wanted frequency by changing its length, not impedance matching (dipol slides) |
| Aufbauhöhe (Antenne) | height (above the ground) | EG207, EG208 "height at which it is installed"; *bei geringerer Aufbauhöhe* → "at lower heights" (fusspunktimpedanz_1, _2) |
| Speiseimpedanz / Speisewiderstand (Kurstext) | feed-point impedance | as §9 *Fußpunktimpedanz*, also where the text derives it from Ohm's law; there the bare *Widerstand* $R = U/I$ stays *resistance*, and *niederohmig / hochohmig* → low-impedance / high-impedance, as EG204, EG205 (strom_spannung_speisung_1, fusspunktimpedanz_1) |
| stromgespeist / spannungsgespeist / Strom- und Spannungsspeisung | current-fed / voltage-fed / current and voltage feeding | EG204–EG206, AG207, AG208 |
| Strombauch / Strombäuche (gezählt) | current antinode(s) | the course pairs *Bauch* with *Knoten* (strom_spannung_speisung_1) and counts the antinodes to find the multiple (strom_spannung_speisung_2, AG203–AG206); §9 |
| Anregung / Anregungsfrequenz (Dipol) | (when the dipole is) fed at / operating frequency | as §9 *Erregung / Erregerfrequenz* and AG203–AG206 "applies when the dipole is fed at 28 MHz" |
| mechanische / elektrische Länge | mechanical / electrical length | elektrische_verlaengerung_verkuerzung |
| Verkürzungskondensator | shortening capacitor | the capacitor that shortens an antenna electrically, counterpart of the *Verlängerungsspule* → loading coil (§9) (elektrische_verlaengerung_verkuerzung) |
| Bauform (Antenne) | design; form | "die Bauform eines Parabolspiegels" → "the parabolic dish design", "eine besondere Bauform der Yagi-Uda-Antenne" → "a special form of the Yagi-Uda antenna"; *Bauform* of a component stays *package style* (parabolspiegel_1, yagi_uda_3) |
| Sperrkreis-Dipol, der auch als Trap-Dipol bezeichnet wird / Trap (englisch für „Falle") / wirkt als Sperrkreis | trap dipole / trap / acts as a rejector | English has one name for the dipole, and the gloss only translates *trap* back into German, so both are dropped (bracket rule); where the text says what a trap *does* at resonance (*wirkt als Sperrkreis*), *rejector*, the RSGB word for a parallel-resonant blocking circuit (§5), so that a trap does not "act as a trap"; the questions keep their "traps for the operating frequency" (AG111–AG113) (traps, AG114, AG116) |
| Raumwelle mit nahezu vertikalem Einfallswinkel (NVIS, "zu Deutsch") | (dropped) | the German rendering of the English expansion only translates it back (bracket rule): "*NVIS*, for near vertical incidence skywave" (nvis) |
| Strahlenoptik / Beugungseffekte / Schüssel | ray optics / diffraction effects / dish | parabolspiegel_1 |
| Strahlungsachse / Polarisationsebene | axis of radiation / plane of polarisation | AG126 (yagi_uda_3) |
| Offsetspiegel (auch Offsetantenne genannt) | offset dish (also called an offset antenna) | AG127; §9 *Offsetspiegel* |
| $\frac{Vor}{Rück}$ (Vor-/Rück-Verhältnis in Lösungsfolien) | $\frac{Front}{Back}$ | the ratio written as words in the worked slides; the symbols $P_V$, $P_R$, $U_V$, $U_R$, $g_D$ stay (DECISIONS.md) (vor_rueck_verhaeltnis) |
| Bodenverluste / Wechselwirkung mit dem Boden | ground losses / interaction with the ground | *Erdboden* → the ground (§13) (fusspunktimpedanz_1) |
| Lichtbogen / Kabelbrand / Fahrzeugbrand | arc / cable fire / vehicle fire | NK307 "Arcing and vehicle fire" (einbau_kfz) |
| Mittelkonsole / PKW / Gegenelement (Fahrzeugdach) | centre console / car / counterpoise | as §9 *Gegengewicht* (einbau_kfz) |
| Stecker / Kupplung / Buchse / Einbaustecker (Koaxialsteckverbinder) | plug / socket / panel socket / panel plug | koaxsteckverbinder defines *Stecker* as the male part, *Kupplung* as the female part, and *Buchse* / *Einbaustecker* as a *Kupplung* / *Stecker* built into equipment; so *Kupplung* takes *socket* and the built-in forms take *panel*: *PL-Einbaubuchse* → PL panel socket, but *N-Buchse* (no contrast) → N socket. Not *jack*, which in British English is also the male audio plug. Elsewhere a bare *Buchse* stays *socket* (§4). Reverse SMA: "the reverse SMA plug is a socket" (DECISIONS.md) |
| Steckverbinder / Koaxialsteckverbinder / Stecker (als Typbezeichnung: N-Stecker, BNC-Stecker) | connector / coaxial connector / connector | where *Stecker* names the connector type rather than the male part (uebertragungsleitungen_2 slides, EG303 "N connector") |
| Mittelstift / Kontaktöffnung / Außengehäuse (Steckverbinder) | centre pin / contact opening / outer body | koaxsteckverbinder, steckverbinder_n; §14 *Kontaktstift* → contact pin |
| Winkeladapter / Reverse-SMA-Steckverbinder / „Geschirmter Bananenstecker" | right-angle adapter / reverse SMA connector / "screened banana plug" | steckverbinder_bnc, steckverbinder_sma, steckverbinder_pl slides (a nickname of the PL connector, kept literally); *umgedreht (reverse)* → "reversed", the bracket only repeats the English word |
| Schutzmantel / Mantel (Kabel) / Kunststoffummantelung / Drahtgeflecht / Folie / Abschirmfolie | protective sheath / sheath / plastic sheath / wire braid / foil / screening foil | uebertragungsleitungen, koaxsteckverbinder, kabeldaempfung_2; British *sheath* rather than *jacket* |
| Induktivitätsbelag / Kapazitätsbelag | inductance per unit length / capacitance per unit length | $L'$, $C'$ (wellenwiderstand) |
| Mittenabstand (der Leiter) | centre-to-centre spacing (of the conductors) | $a$ in the twin-feeder formula, AG305 "spacing between the parallel conductors" (wellenwiderstand) |
| Querschnittsaufbau | cross-sectional structure | uebertragungsleitungen_2, EG301 |
| Gegentaktströme / Gleichtaktströme (Zweidrahtleitung) | differential-mode currents / common-mode currents | as §9 *Gleichtakt / Gegentakt*; *Gleichtaktanteile* → common-mode components (AG312) (uebertragungsleitungen_3) |
| Hochfrequenzeigenschaften / Biegeradius | RF properties / bending radius | AG303 (uebertragungsleitungen_3) |
| Aufschäumung / geschäumt / nicht-geschäumtes Polyethylen | foaming / foamed / solid (non-foamed) polyethylene | *solid* is the established English term, as AG302 "solid PE" and AG317 "solid polyethylene" for *Voll-PE*; the course text adds "(non-foamed)" to keep the German contrast with *geschäumt* (uebertragungsleitungen_3) |
| geometrische ("mechanische") Länge $L_\mathrm{G}$ | geometric ("mechanical") length | symbol unchanged; AG317 "physical length" (uebertragungsleitungen_3) |
| Hin-Richtung / Rück-Richtung / Hinweg / Rückweg (Leitungsdämpfung) | on the way there / on the way back | the forward and return trip of a wave on a lossy line (swr_3, AG402–AG404); *in Hin- und Rückrichtung jeweils* → "in each direction, there and back" |
| Leitungsdämpfung / verlustbehaftete Leitung | line loss / lossy line | swr_3 |
| Stehwellenmessgerät, kurz SWR-Meter | SWR meter | one English term for both German words (§11); the "kurz" doublet and "vom englischen Begriff standing wave ratio abgeleitete Abkürzung" are dropped (bracket rule) (swr) |
| einschleifen (SWR-Meter) | insert (in the line) | NI202, AI401 "inserted in the line"; "Das SWR-Meter wird … eingeschleift" → 'inserting the SWR meter in the line' (swr, swr_meter_1) |
| Koppelleitung / kapazitive / induktive Kopplung (Richtkoppler) | coupling line / capacitive / inductive coupling | swr_meter_2; §14 *Messwerk* → meter movement, §11 *Kreuzzeigerinstrument* → cross-needle meter |
| „Skineffekt" vom englischen Wort „skin" für „Haut" | "skin effect" | the gloss only translates the English word back (bracket rule) and is dropped (skineffekt) |
| Mantelwellen (Definition im Kurstext) / Mantelstrom / Mantelwelle | common-mode currents (in German *Mantelwellen*, literally "sheath waves") / sheath current / sheath wave | where the course defines the effect (mantelwellen_1) the German word is named once, because the text and the questions also say *sheath current(s)* (EG404, AG425, AG426, AG428); *Mantelstrom mit zugehöriger Mantelwelle* → "a sheath current, with its associated sheath wave" (mantelwellen_2); everywhere else *Mantelwellen* → common-mode currents (§9, DECISIONS.md) |
| stromkompensierte Drossel neben Mantelwellensperre (Kurstext) | current-compensated choke / common-mode choke | where the text gives both names ("eine sogenannte *stromkompensierte Drossel* … auch als *Mantelwellensperre* bezeichnet"), two English names are needed; *current-compensated choke* as AG426, embedded in the same text (mantelwellen_1, mantelwellen_2; DECISIONS.md) |
| Symmetrierglied (Kurstext) | balancing device | as AG420 "balancing devices such as … a balun"; "ein sogenanntes *Symmetrierglied*, einen Balun" → "a *balancing device*, a balun" (mantelwellen_1) |
| Gegentaktsignal / Gleichtaktsignal | differential-mode signal / common-mode signal | as §9 *Gleichtakt / Gegentakt* (mantelwellen_2) |
| Spannungsbalun / Spartransformator | voltage balun / autotransformer | AG428, AG429; §4 *Spartransformator* (mantelwellen_2) |
| (HF-)Trenntrafo / Pol (des Trenntrafos) | (RF) isolating transformer / terminal | AJ115; §14 *HF-Trenntrafo* (mantelwellen_2) |
| Dreileitersystem / Außenseite des Innenleiters / Innenseite des Außenleiters / Außenseite des Außenleiters | three-conductor system / outside of the inner conductor / inside of the outer conductor / outside of the outer conductor | mantelwellen_1 |
| kontaktlose Einkopplung (in den Koax-Schirm) | contactless coupling (into the coax screen) | AG427, AG429 "coupling into the coax screen" (mantelwellen_2) |
| Umwegleitung / Umwegeleitung / λ/2-Umwegleitung (Kurstext) | delay line / delay line / $\lambda/2$ delay line | as AG420, AG423, AG424; also in captions, where the German has no λ/2 (umwegleitung; DECISIONS.md) |
| Anschlusspunkte (einer Antenne) | terminals | AG424 "at each of its terminals" (umwegleitung) |
| betragsgleich, 180° phasenverschoben | equal in magnitude, 180° out of phase | umwegleitung |
| Frequenz-Sweep / Wobbeln | frequency sweep / wobbulation | the older German word gets its older English counterpart (*wobbulator*) (vna_2) |
| Startfrequenz / Stoppfrequenz / Frequenzpunkt | start frequency / stop frequency / frequency point | vna_2 |
| imaginäre Einheit / imaginäre Zahl / reelle Zahl / komplexe Zahl | imaginary unit / imaginary number / real number / complex number | as §14 *komplexe Größe* (vna_2) |
| Zustände "offen" / "Kurzschluss" / "angepasst" (VNA) | "open-circuit" / "short-circuit" / "matched" condition | as §11 *Betriebszustände Kurzschluss, Leerlauf und Anpassung* and EI206 "short-circuit, open-circuit and matched conditions" (vna_1) |
| Leitungsabschluss | line termination | vna_1; §11 *Abschlusswiderstand* → terminating resistor |
| Zweidrahtleitung (Lecherleitung) | two-wire line | a Lecher line is not a feeder, so §9's *twin feeder* (AG311) is not used; AG320 "two parallel conductors" (lecherleitung slides) |
| gewünschter Speisewiderstand $Z_\mathrm{E}$ (λ/4-Transformation) / geometrisches Mittel | desired input impedance $Z_\mathrm{E}$ / geometric mean | $Z_\mathrm{E}$ is the impedance wanted at the input end of the transformer section, not the antenna's feed point, which is $Z_\mathrm{A}$ (AG417, AG418); *Speise- und Lastwiderstand* → "the input impedance and the load resistance" (impedanztransformation) |
| Kreiszahl | the number $\pi$; the mathematical constant | "hat nichts mit der Kreiszahl $\pi$ zu tun" → "has nothing to do with the number $\pi$" (impedanztransformation) |
| Gewinnfaktor (Kurstext, Klasse N) | gain factor | the course states the gain as a factor and sets it against the "gain in decibels" (effektive_strahlungsleistung_erp_1, aequivalente_isotrope_strahlungsleistung_eirp_1, sendeleistung_klasse_n); the questions keep §9's "a gain of 2.5 (as a power ratio)" (VD725, VD726) (DECISIONS.md) |
| Kugelstrahler, fachsprachlich isotroper Strahler | spherical radiator, known technically as an isotropic radiator | where the course gives both words at first mention (aequivalente_isotrope_strahlungsleistung_eirp_1, slide heading "Spherical radiator or isotropic radiator"); everywhere else *Kugelstrahler* → isotropic radiator, as §9 (DECISIONS.md) |
| "equivalent isotropic radiated power" / "effective radiated power" (the German's *vom englischen …* gloss) | equivalent isotropically radiated power (EIRP) / effective radiated power (ERP) | the gloss only gives the English term and is dropped (bracket rule): "… usually abbreviated to ERP"; the German's *isotropic* written as the established *isotropically* (RR 1.161, §9); the slide line *Effective radiated power* under the heading "Effective radiated power (ERP)" is dropped, *Equivalent isotropic radiated power* under the bare heading "EIRP" stays as the expansion |
| Feldwellenwiderstand $Z_\mathrm{F}(d)$ (Kurstext) / Feldwellenwiderstand des freien Raums $Z_0$ | wave impedance / impedance of free space | the distance-dependent ratio $\lvert E/H \rvert$ is the *wave impedance*, as AK102 "the wave impedance of the medium"; $Z_0 \approx 377\,\Omega$ stays *impedance of free space* (§3) (nahfeld, AK102) (DECISIONS.md) |
| Fresnel-Bereich / Strahlungswiderstand / Feldanteile (quasistatisch, induktiv, Strahlung) | Fresnel region / radiation resistance / field components (quasi-static, inductive, radiation) | the `\text{}` labels under the braces are running words and are translated (nahfeld, AK101) |
| Momentaner Spitzenwert / 6-Minuten-Intervalle / Gepulste Felder (26. BImSchV) | instantaneous peak value / 6-minute intervals / pulsed fields | as EK102 "instantaneous peak value", "RMS value averaged over 6 minutes"; *quadratischer Mittelwert* → RMS value (personenschutzabstand_grenzwerte) |
| Bundesamt für Strahlenschutz | Federal Office for Radiation Protection (Bundesamt für Strahlenschutz) | the office's own English name; German name in brackets at first mention (personenschutzabstand_grenzwerte) |
| Eindringtiefe / Thermoregulation / Kraftwirkungen / Wärmewirkung / Energieabsorption | penetration depth / thermoregulation / force effects / heating effect / energy absorption | biological effects of RF fields (personenschutzabstand_grenzwerte) |
| nachvollziehbar (Dokumentation, zeichnerische Darstellung) | comprehensible | as VE512, VE513, and the tip that names it as the key word (anzeige_ortsfester_amateurfunkanlagen) |
| kontrollierter Bereich (neben kontrollierbarer Bereich) | controlled area | written as the German writes it (personenschutzabstand_2); *kontrollierbarer Bereich* stays *controllable area* (§1.4) |
| Anleitung zur Durchführung der Anzeige ortsfester Amateurfunkanlagen nach §9 der BEMFV / Erläuterung(en) der Bewertungsverfahren nach BEMFV | Instructions for notifying fixed amateur radio installations under Section 9 BEMFV / Explanation(s) of the assessment procedures under the BEMFV | BNetzA documents, in German only; as link text the English title alone, where a solution cites one as its source without a link the German title follows in brackets so that it can be found (AK103) (personenschutzabstand_2, nahfeld) |
| Mobilfunknetz-Betreiber / Sendeanlage für das Mobilfunknetz | mobile network operator / transmitter for the mobile phone network | personenschutzabstand, standortbescheinigung |
| Näherungsformel / Fernfeld-Näherungsformel / Fernfeldformel / Abstandsformel (Sicherheitsabstand) | approximation formula / far-field approximation formula / far-field formula / distance formula | as §1.4 *Näherungsformel für die Fernfeldberechnung* and EK105, EK106 (naeherungsformel_1, naeherungsformel_2, personenschutzabstand_3) |
| Fernfeld (bzw. strahlendes Nahfeld) / Freiraum (Folien) | far field (or radiating near field) / free space | §14 *Nahfeld (reaktives / strahlendes)*; *Gilt nur im Freiraum* → "Only valid in free space" (naeherungsformel_1 slides) |
| Erläuterungen zur BEMFV (Linktext) | Explanations of the BEMFV | link text, translated as written; the document's full title is the row *Erläuterung(en) der Bewertungsverfahren nach BEMFV* above (naeherungsformel_1) |
| Umrechnungsfaktor $\textrm{Faktor}_\textrm{FmodPers}$ | conversion factor $\textrm{Faktor}_\textrm{FmodPers}$ | the symbol is the field name in the BEMFV notification, which the reader has to fill in, so it stays German like the formula subscripts (personenschutzabstand_3, naeherungsformel_2 slides) |
| Strahlungskeule / Hauptstrahlungskeule / Winkeldämpfung | radiation lobe / main lobe / off-axis attenuation | with §9 *Hauptkeule* and §14 *Winkeldämpfung* (personenschutzabstand_richtantennen) |
| Hilfsmittel der Bundesnetzagentur / Kapitel „Pegel" / „Strahlungsleistung und Gewinn" (Formelsammlung) | the Federal Network Agency's examination aids / the section "Levels" (*Pegel*) / "Radiated power and gain" (*Strahlungsleistung und Gewinn*) | formula-sheet section names as keywords, English with the German in brackets (DECISIONS.md) (AK105) |
| Benötigte Formeln / Angaben aus der Aufgabenstellung / Lösungs(s)chritte / Interpretation / Umstellung der Formel (Lösungen) | Formulas needed / Data from the question / Solution steps / Interpretation / Rearranging the formula | headings of the worked solutions AK106–AK115 |
| Teil 1 / Teil 2 des Lösungsansatzes / Einsetzen / Interpretation der Formel (Lösungen) | Approach, part 1 / Approach, part 2 / Substituting / Interpreting the formula | AK105 |
| Leistungszusammenhang EIRP und ERP | relationship between EIRP and ERP | AK106–AK113 |
| Bonusfrage (Folien) | Bonus question | naeherungsformel_1 slides |
| Portabelbetrieb | portable operation | naeherungsformel_2 |
| Feldwellenwiderstand im Vakuum / Wellenwiderstand des Mediums | wave impedance in a vacuum / wave impedance of the medium | AK102 (personenschutzabstand_3 slides) |
| Dachständer (Kurstext, Bildunterschrift) / Freileitung / elektrische Freileitung / Energieversorgungsleitung | roof-mounted support (for an overhead mains line) / overhead line / overhead power line / power line | §9 *Dachständer* described as needed; NK311 "power lines" (antennen_energieleitungen) |
| Bauamt von Stadt oder Gemeinde / Nachbargrundstücke / Mitgliedsbeitrag / Versicherungsleistung | building authority of the town or municipality / neighbouring properties / membership fee / insurance cover | antennen_baurecht_haftung; VE602, VE707 |
| Ehrensache / vor lauter Tatendrang | a point of honour / in all the eagerness to get on with the job | repairing your own equipment (elektrische_geaete_oeffnen_2) |
| Netzseite (230 V) / Nennspannung des Netzes / Kondensatoranschlüsse | (230 V) mains side / nominal mains voltage / capacitor terminals | elektrische_geaete_oeffnen_1, _2 |
| Entladewiderstand / hochohmiger, isolierter Widerstand / Lichtbogenbildung / Leiterbahnen / Pulsbetrieb | discharge resistor / high-value, insulated resistor / arcing / PCB tracks / pulse operation | AK201 "high-value resistor with an adequate power rating" (elektrische_geaete_oeffnen_2, AK201) |
| Isolierhandschuhe in einer ausreichenden Schutzklasse / isoliertes Werkzeug | insulating gloves of an adequate protection class / insulated tools | as §14 *Isolierhandschuhe* (elektrische_geaete_oeffnen_2) |
| Blitzschutz-Zwischenstecker (für Koaxkabel) | in-line lightning protection adapter (for coaxial cable) | with a gas discharge tube (§4) (blitzerdung) |
| Erdungsleitung (massiver Draht, keine Litze) / Gebäudeerdung | earthing conductor (solid wire, not stranded) / building earth | EK209, EK210 "single solid wire", "building earth"; §12 *Erdungsanlage* → earthing system (blitzerdung) |
| Schraubanschluss Ground (GND) (Bildunterschrift) | Ground (GND) screw terminal | *Ground (GND)* is the label printed on the equipment and is kept; in running text *Erdung* stays *earthing* (§12) (blitzschutz) |
| Potentialausgleichsschiene / Potentialausgleichsleiter / Ausgleichsstrom | equipotential bonding busbar / equipotential bonding conductor / equalising current | §12 *Potentialausgleich*, §14 *Ausgleichsströme* (schutzerdung_2, AK202, AK203) |
| Elektroinstallation / Erdleitungen / Heizungsrohre | electrical installation / earth leads / heating pipes | schutzerdung_2 |
| Spannungsbauch (Erdungsleitung, Antenne) / HF-Spannungsbauch | voltage antinode / RF voltage antinode | as in strom_spannung_speisung; §9 *Spannungsbauch* (schutzerdung_2, antennen_beruehrung_2, AK203) |
| „heiß" (Sendergehäuse) / Herdplatte | "hot" / hotplate | AK203 "the transmitter case is "hot"" (schutzerdung_2) |
| Prasselstörungen / Antennenzuführung | crackling interference / antenna feeder | static charges (statische_aufladung); EK207 |
| der Rothammel | the Rothammel antenna book | the standard German antenna handbook, named so that the English reader knows what it is (statische_aufladung slides) |
| erschrecken oder verkrampfen / Erschrecken und Verkrampfen / Sekundärunfall | give you a fright or make your muscles cramp / fright and muscle cramp / secondary accident | as gefahren "fright … muscle cramp" (antennen_beruehrung_1) |
| Abschnitt "Gefahren durch elektrischen Strom" | the section "Dangers of electric current" | section titles are not yet translated; quoted in English (antennen_beruehrung_1) |
| direkter Strahlengang (einer Sendeantenne) | direct beam | EK201 "direct beam of transmitting antennas"; §14 *Strahlengang* → radiation path stays for the optics of a dish (strahlengang_aufenthalt) |
| Gewebe / Wärmeabfuhr / Hoden | tissue / heat dissipation / testes | strahlengang_aufenthalt |
| HF-Funkenüberschläge / Körperstrom | RF flashovers / current through the body | as §13 *Spannungsüberschlag* → flashover (AK204, AK202) |
| aus Sicht der Niederfrequenz | at low frequencies | here DC and the mains frequency, not audio: not *AF* (AK203) |
| Backsteinaktion / Mauersteine | brick campaign / bricks | the radio amateurs' protest of January 1949 before the first AFuG (gesetze_vorschriften) |
| Grundgesetz (der Bundesrepublik Deutschland) / Wirtschaftsrat (1949) / Deutscher Bundestag | Basic Law (Grundgesetz) / Economic Council / German Bundestag | the established English names (gesetze_vorschriften) |
| internationaler Fernmeldevertrag | international telecommunication treaty | the course's name for the RR (gesetze_vorschriften) |
| Bundesminister für Digitales und Verkehr | Federal Minister for Digital and Transport | the ministry's own English name (gesetze_vorschriften) |
| Rechtsgrundlage / Amateurfunkbetriebsrechte / unmittelbar geltendes Recht | legal basis / right to operate amateur radio / directly applicable law | gesetze_vorschriften |
| Funkdienste (Services) / Seefunk (Maritime Service) / Rundfunk (Broadcasting Service) | radiocommunication services / maritime mobile service / broadcasting service | the brackets only give the English and are dropped; *Seefunk* as §1.1 *Seefunkdienst* (amateurfunkdienst) |
| Funkanwendungen mit Allgemeinzuteilung | radio applications under a general assignment | as §14 *Allgemeinzuteilung*; *WLAN* → Wi-Fi (amateurfunkdienst) |
| Gesetzgeber / öffentlich gesprochenes Wort | legislator / public speech | "Alle Äußerungen sind öffentlich gesprochene Worte" → "Everything said counts as public speech"; *das nicht öffentlich gesprochene Wort* → private (non-public) conversations, as §1.2 (amateurfunkstelle) |
| Handwerksbetrieb | tradesman's business | funkamateur |
| Zulassungsbescheid (zur Teilnahme am Amateurfunkdienst) | notice of authorisation (to participate in the amateur service) | beside *Prüfungsbescheid* → examination result notice (§1.3); *Zulassungsurkunde* stays *licence document* (zulassung) |
| Gebührenbescheid / Zahlungsaufforderung | fee notice / demand for payment | gebuehren_beitraege |
| Verwaltungs-Vollstreckungsgesetz (VwVG) / Vollstreckungsmöglichkeiten | Administrative Enforcement Act (Verwaltungs-Vollstreckungsgesetz, VwVG) / means of enforcement | course text, where the German gives the abbreviation; VE704 keeps "Administrative Enforcement Act" (§1.2) (gebuehren_beitraege) |
| Geheimhaltungspflicht / Verwertung und Weitergabe (von Nachrichten) | duty of confidentiality / using and passing on (messages) | as VE202 (fernmeldegeheimnis_abhoerverbot) |
| Rechtsgüterabwägung | balancing of legal interests | fernmeldegeheimnis_abhoerverbot |
| Wanzen | bugs | eavesdropping devices (VE204) |
| Strafvorschriften / Freiheitsstrafe / Geldstrafe / Täter / fahrlässig | penal provisions / imprisonment / fine / offender / negligently | *Geldstrafe* (criminal) and *Geldbuße* (administrative, §1.2) are both *fine* in English; "Mit Freiheitsstrafe bis zu zwei Jahren oder mit Geldstrafe wird bestraft, wer" → "Imprisonment for up to two years or a fine shall be imposed on anyone who", as § 323c StGB in notfunk (§ 27 TDDDG) |
| eine Mitteilung machen (§ 5 Abs. 2 TDDDG) | make a disclosure | the TDDDG's prohibition on telling others the content or the fact of reception |
| Bußgeldvorschriften / Aberkennung (des Amateurfunkzeugnisses) | provisions on fines / withdrawal (of the amateur radio certificate) | as §1.2 *Entzug*, so the prose matches the wrong answers of VC125 b and VE704 b (verstoesse_und_folgen) |
| Merkhilfen der Q-Gruppen (*v*orbereitet, ein *z*weites Mal, gr*o*ße Leistung, *b*ergauf und *b*ergab, "*K*ommen") | English where a faithful rendering of the cue word keeps the letter: *M*an-made, *N*atural, *t*erminate, *l*ogged (ge*l*oggt), *o*n top (*o*bendrauf), at time *X*, *H*ome, *P*iano, Change Frequenc*y*; otherwise the German cue kept with its English meaning: "ich bin *v*orbereitet" ("I am prepared"), "*b*ergauf und *b*ergab" (German for "uphill and downhill"), "*K*ommen" (German for "over") | DECISIONS.md; a German gloss of the English cue (*H*eimat beside *H*ome, *Beenden* beside *terminate*) is dropped (betriebliche_abkuerzungen, q_schluessel) |
| Atmosphärische Störungen (QRN) / menschengemachte Störungen (QRM) / schwankende Zeichen (QSB) / Frequenzwechsel (QSY) | atmospheric interference / man-made interference / fluctuating signals / change of frequency | descriptive meanings in the course text; where a Q code's wording is given, the ITU wording (§2) (q_schluessel) |
| QRP-Betrieb / QRP-Geräte / QRP-Verbindungen | QRP operation / QRP equipment / QRP contacts | q_schluessel |
| Locator-System / QTH-Locator / Kästchen (Locator) | locator system / QTH locator / box | BE111 "QTH locator or grid locator" (§2 *Standortkenner*) (locator) |
| Feld / Quadrat / Unter-Quadrat (Maidenhead-Locator); Größtfeld / Großfeld / Kleinfeld | field / square / subsquare; the German names kept as German | the glosses *(englisch fields)*, *(Quadrate)* only repeat the English and are dropped; the table's German columns are headed "German" and "Alternative German name" (locator) |
| DARC-Geschäftsstelle | DARC head office | in Baunatal (locator) |
| Kartendaten © OpenStreetMap-Mitwirkende / Kartendarstellung © OpenTopoMap | Map data © OpenStreetMap contributors / Map style © OpenTopoMap | the services' own English attribution wording (locator captions) |
| Distriktsortskenner (DOK) / Distrikt | district local club identifier (Distriktsortskenner, DOK) / district | DOK kept, as *OV* for *Ortsverband* (→ local club); "DARC local club (Ortsverband, OV)" at first mention (N_Ende) |
| Lern-App / Prüfungstrainer / Trainingsapp | learning app / exam trainer / training app | N_Ende |
| Nachwuchsförderung / Nachwuchs | encouraging young people / young people | N_Ende |
| Nach der Prüfung ist vor der Prüfung | after the exam is before the exam | motto rendered literally; the German's following *denn* clause explains it (N_Ende) |
| DARC-Chat / DARC-Treff / Dienstags-Treff / AFUBarcamp / HAM RADIO / Funk.Tag / HAM-Challenge | unchanged | names of DARC services and events; *Dienstags-Treff* glossed "(Tuesday meeting)" once in the section (N_Ende) |
| Kurzwellenhörer / Höramateur (deutsche Bezeichnung des SWL) | short-wave listener; the German names kept where the text remarks on them | "Trotz der deutschen Bezeichnung *Kurzwellenhörer* …" → "Despite the German name *Kurzwellenhörer* (short-wave listener), the hobby is not limited to short wave"; slide *deutsche Bezeichnung: Kurzwellenhörer oder Höramateur* → "German names: *Kurzwellenhörer* (short-wave listener) or *Höramateur* (listening amateur)"; the expansion *Short Wave Listener* stays as the German writes it; index term "Short-wave listener" (swl_vorwort, swl_was_ist_swl; DECISIONS.md) |
| DE-Prüfung / SWL-Prüfung | DE examination / SWL examination | the DARC's listener examination; each as the German writes it; "die DE-Prüfung des DARC" → "the DARC's DE examination" (swl_vorwort, swl_steckverbinder, swl_rufzeichen; DECISIONS.md) |
| DE-Kennzeichen / Hörerkennzeichen / SWL-Nummer / Mitgliedsnummer | DE identifier / short-wave listener identifier / SWL number / membership number | not *DE call sign*: the text insists it is no call sign; *Hörerkennzeichen* as §2; VD102's *Hörerrufzeichen* stays "listener call sign ("DE series")" (swl_was_ist_swl, swl_rufzeichen; DECISIONS.md) |
| Hörbericht / Empfangsbericht / Empfangsrapport (SWL) | listener report / reception report / reception report | *Hörbericht* is the SWL's report of a contact heard; *Empfangsrapport* the signal report in it, as BE207 (swl_vorwort, swl_was_ist_swl) |
| Sendegenehmigung | transmitting licence | the DE identifier "ist keine Sendegenehmigung" (swl_was_ist_swl) |
| Weltempfänger / SDR-Stick / SDR-USB-Stick / aktive Mini-Whip-Antenne | world-band receiver / SDR stick / SDR USB stick / active Mini-Whip antenna | *Mini-Whip* capitalised as the design's name (swl_vorwort, swl_erste_empfangsstation) |
| Außenantenne / Zimmerantenne / Empfangsantenne / (reine) Empfangsanlage / Empfangsstation | outdoor antenna / indoor antenna / receiving antenna / receive-only installation / receiving station | swl_erste_empfangsstation, swl_antennensicherheit, swl_steckverbinder |
| Typischer Einstieg / Einstiegsbereiche (Tabelle der Empfänger) | typical way in / ways in | swl_erste_empfangsstation slides |
| Signalstärkeanzeige | signal strength indicator | swl_erste_empfangsstation; the S meter (§2) |
| Steckdosenleiste / Zuleitungen / netzspannungsführende Geräte | multi-socket extension lead / supply leads / equipment that carries mains voltage | NK305 "supply leads"; *gehören in fachkundige Hände* → "should be left to qualified people" (swl_elektrische_sicherheit) |
| Ladegerät / aufgeblähte Akkus | charger / swollen batteries | first mention "rechargeable batteries", then *battery*, as DECISIONS.md *Akku* (swl_elektrische_sicherheit) |
| Miet-, Bau- und Denkmalschutzrecht | tenancy law, building law and heritage protection law | swl_antennensicherheit |
| Hauptverwaltung für das Post- und Fernmeldewesen des Vereinigten Wirtschaftsgebietes | Main Administration for Posts and Telecommunications of the United Economic Area | the post-war authority of the Bizone; German name in brackets (swl_rufzeichen) |
| Deutsche Empfangsstation (DE, seit 1925) | *Deutsche Empfangsstation* (German receiving station) | the German expansion of DE kept, because it is what the letters stand for (swl_rufzeichen) |
| Merkhilfen der SWL-Landeskennertabelle: Anfangsbuchstabe / LuXemburg / Franz. PAys-Bas | Initial letter / LuXembourg / French: PAys-Bas | as DECISIONS.md *German mnemonics*: the English name spells the same letters (LuXembourg), the French one stays; *OEsterreich (Austria)*, *Schönes Polen (beautiful Poland)*, *EspaniA* as internationale_landeskenner (swl_landeskenner) |
| Daumenregel / Faustregel / Faustformeln | rule of thumb / rule of thumb / rule-of-thumb formulas | swl_modulationsarten, swl_ionosphaere, swl_frequenzbereiche |
| VFDB | VFDB | the German telecommunications employees' radio club; unchanged, not expanded, as the German (swl_was_ist_swl) |
| Deutschland-Diplom-SWL (DLD-SWL) / Deutschland-Diplom / DLD-SWL 100 … 1000 / Sonder-DOK / Diplomregeln | *Deutschland-Diplom-SWL* (Germany Award for SWLs, DLD-SWL) / *Deutschland-Diplom* (Germany Award) / DLD-SWL 100 … 1000 / special DOK / award rules | the DARC award's German name kept, because the abbreviation spells it, with the English gloss at first mention in a file; afterwards *DLD-SWL* / *DLD*, as the German (swl_dld; DECISIONS.md) |
| Deutscher Empfangsmeister (DEM) / Grundstufe / Bronze, Silber, Gold / korporativer Verband / Ausschreibungsbedingungen | *Deutscher Empfangsmeister* (German Reception Master, DEM) / basic level / Bronze, Silver, Gold / affiliated association / award conditions | title kept in German in its base form (also for the German's inflected *der Deutsche Empfangsmeister*), glossed at first mention in a file; *Empfangsmeister erhalten …* → "Holders of the title receive …" (swl_dem, swl_de_kennzeichen, swl_abschluss; DECISIONS.md) |
| Distrikts-Ortsverbands-Kennziffer (DOK) | district local club identifier (*Distrikts-Ortsverbands-Kennziffer*) | the SWL course's own expansion of DOK; same English as *Distriktsortskenner* (N_Ende) (swl_dld) |
| Ortsverbandsvorsitzende(r) / Distriktsvorsitzende(r) / AJW-Distriktsreferent / DL-AJW-Referat, DL-AJW-Referent / Vorstand (DARC) / DARC-Regularien | local club chair / district chair / district AJW officer / DL-AJW department, DL-AJW officer / (DARC) board / DARC rules | AJW not expanded, as VFDB; *Referat* → department and *Referent* → officer, as *Referat für EMV* (swl_de_pruefung, swl_antrag) |
| Wunschkennzeichen / Wunschsuffix / Suffixkombination / Vergabeschlüssel / Vergabestelle / Urkunde (DE-Kennzeichen) / Kennzeichenbereich | preferred identifier / preferred suffix / suffix combination / allocation scheme / issuing office / certificate / identifier range | as *Wunschrufzeichen* → preferred call sign (swl_de_kennzeichen, swl_antrag) |
| geprüfte Empfangsstation / geprüfter SWL / Ausbildungsempfangsstation / Höramateur, Empfangsamateur | qualified receiving station / qualified SWL / training receiving station / short-wave listener, listening amateur | *Höramateur* is *listening amateur* where it is set against *Funkamateur* (swl_rechtsgrundlagen), otherwise *short-wave listener*; *Empfangsamateur* → listening amateur (swl_de_kennzeichen, swl_dld, swl_dem) |
| Prüfungskommission / Fragebogen, Prüfungsbogen / Probeprüfung | examining board / question paper, examination paper / practice examination | the DE examination (swl_de_pruefung, swl_antrag, swl_abschluss) |
| Hörpause / Hörübung / wertbare Verbindungen / Tabellenkalkulation | pause for listening / listening exercise / valid contacts / spreadsheet | swl_betriebsbeobachtung, swl_relais, swl_logbuch; *Split-Verkehr* → split operation (§2, BE308) |
| Gesamtkurs N / E / A / Aufbaukurs N -> E, E -> A, N -> A / SWL-Kurs | Full course N / E / A / Upgrade course N -> E, E -> A, N -> A / SWL course | titles of the tables of contents (toc/*.json); *Aufbaukurs* as *Aufstockungskurs*; the arrow kept as written |
| Kurs Klasse N / Kurs Klasse E (mit N) / Kurs Klasse A (mit N und E) / Aufstockungskurs N nach E / Auszug Digitaltechnik (E und A) | Class N course / Class E course (with N) / Class A course (with N and E) / Upgrade course N to E / Extract: digital technology (E and A) | site buttons (contents/snippets) |
| Vorwort / Kursabschluss (Abschnittstitel) | Foreword / End of the course | toc |
| Foliensatz / Sektion (Folien) / Buchreihe / Ausbildungsplattform / Prüfling / Mobilfunk, Rundfunk, Flugfunk (als Funkdienste) | slide set / section / book series / training platform / candidate / mobile telephony, broadcasting, aeronautical radio | vorwort |
| Präsenzkurs / Kurse vor Ort und Online / Selbst-Studium / Patenkarte / Lehrgangskarte / Lehrgang für die Karte melden | face-to-face course / local and online courses / self-study / mentor map / course map / report a course for the map | static pages and snippets; *Ausbildungspate* → mentor (§14) |
| Erstprüfung / Zusatzprüfung / Anmeldeformular / Prüfungstermin / Lösungsbogen / Entwurfspapier / Single-Choice-Fragebögen / Prüfungszeugnis der Klasse N | first examination / additional examination / registration form / examination date / answer sheet / scrap paper / single-choice question papers / Class N examination certificate | static page pruefung |
| mündliche Nachprüfung | oral re-examination | pruefung; as DECISIONS.md *Nachprüfung* → re-examination |
| Nachteilsausgleich / (fach-)ärztliches Attest / Erleichterungen / Einzelprüfung | compensation for disadvantages / (specialist) medical certificate / concessions / individual examination | pruefung, examinations for people with disabilities |
| Prüfungsteile Betriebliche Kenntnisse / Vorschriften / Technik; Technikteil N | parts of the examination Operating knowledge / Regulations / Technical knowledge; technical part N | pruefung, infos; as §15 |
| Jedermann-Funk (CB-Funk, Freenet, PMR) / freie Funkanwendungen | licence-free personal radio services (CB radio, Freenet, PMR) / licence-free radio applications | infos |
| Rücksichtsvoll / Loyal / Fortschrittlich / Freundlich / Hilfsbereit / Ausgeglichen / Bereit (Ham Spirit) | Considerate / Loyal / Progressive / Friendly / Helpful / Balanced / Ready | hamspirit: the DARC's own wording of the Radio Amateur's Code, translated faithfully, not replaced by Segal's English text |
| Störende Beeinflussung elektronischer Geräte I / II (Abschnittstitel) | Breakthrough into electronic equipment I / II | toc; DECISIONS.md *störende Beeinflussung* → breakthrough |
| Verkürzungsfaktor I / II (Abschnittstitel) | Velocity and shortening factor I / Shortening factor II | toc; part I introduces both names (DECISIONS.md *Verkürzungsfaktor in the course text*), part II is about antennas only |
| Aufbau eines Empfängers / eines Senders / Antennenformen (Abschnittstitel) | Structure of a receiver / of a transmitter / Antenna types | toc |
| Zeiger drehen lassen / Anfangszustand (anzeigen) / Keine Aktion / Fall 1, Fall 2 / Schaltzustände (Applets) | Rotate the phasor / (Show) initial state / No action / Case 1, Case 2 / switching states | applet_iq_zeiger, applet_gleichrichter_1/_2, applet_ringmodulator |
| Überlagerung / Summiertes Signal / Summiertes I/Q-Signal / I-Anteil, Q-Anteil (Applets) | superimposed signal / summed signal / summed I/Q signal / I component, Q component | applet_interferenz, fading_applet, applet_iq, applet_iq_169; as §8 *I/Q (Inphase- / Quadraturkomponente)* |
| Zeit-Sampling / Wert-Quantisierung (Applet) | Time sampling / Value quantisation | quantisierung_und_sampling; the course text names the controls (sampling_quantisierung) |
| Übertragung starten / Erneut übertragen / Neuer Bitstrom / Übertragung läuft (Applet) | Start transmission / Transmit again / New bit stream / Transmission in progress | applet_qpsk; "Transmit again" as the psk slides already quote it |
| Keine Anregung / Anregungsfrequenz (Traps-Applet) | Not fed / operating frequency | applet_traps; as §9 *Erregung / Erregerfrequenz* and §14 *Anregung* |
| Normwerte / Schaltungsform (Dämpfungsglied-Applet) | preferred values / configuration | applet_daempfungsglied; as §4 *Normreihe (E-Reihe)* |
| Kurzbeschreibung / Ausführliche, Detaillierte Beschreibung, Detailbeschreibung / Zusammenfassung / Kurze Zusammenfassung, Kurzzusammenfassung / Kurzfassung / Details (Alt-Text-Abschnitte) | Short description / Detailed description / Summary / Short summary / Brief summary / Details | section labels of the picture descriptions, numbering (1), 2), 1., 2.) kept as in the German (slike_01) |
| Teilbild / Abbildung „a.“ / Allgemein (Alt-Text) | panel / Figure "a." / General | slike_01 |
| offener Anschlusskreis / Anschlussklemme / Knoten, Knotenpunkt (Schaltbild) | open terminal circle / terminal / node (filled dot) | picture descriptions; *Leitung* in a drawn circuit → *line* (slike_01) |
| Wellenlinie / Doppelpfeil / Hilfslinie / Pfeilspitze | wavy line / double-headed arrow / guide line / arrowhead | picture descriptions (slike_01) |
| „1. OW“ … „4. OW“ (Zeichnung 1008) | "1. OW" … "4. OW" (1st to 4th overtone) | numbered *Oberwelle* stays *overtone*, so the numbering stays right (§5 *Oberwelle* trap); the unnumbered label *Oberwellen (OW)* → "Harmonics (OW)", as the course caption (slike_01) |
| Schaltplan in rechteckiger Leitungsführung / Anschlusspunkt / an Masse (liegen), mit Masse verbunden | circuit diagram drawn with right-angled wiring / terminal / connected to chassis | picture descriptions; *Leiter* stays *conductor* (§3) (slike_02) |
| Ableitung (zum unteren Leiter) / Abzweigung / Anzapfung (Schaltbild) | shunt path / branch / tap | slike_02 |
| Halbbögen (Spulensymbol) / Strich / Querstrich / durchgestrichene Linie | semicircles / stroke / crossbar / a line through it | inductor drawn as *Spule* → *inductor*, the two windings of a transformer → *coils* (slike_02) |
| Baustein „IC1“ / polarisierter Kondensator / verstellbarer, variabler Kondensator / Addierer | component "IC1" / polarised capacitor / adjustable, variable capacitor / adder | slike_02 |
| Nullpunkt (Diagramm) / Grundlinie / Auslenkung (Feldlinien) / Bodenfläche | origin / baseline / displacement / ground surface | §14 *Nulllinie* → zero line (slike_02) |
| Grunddämpfung α0 je 100 m Leitungslänge (Kabeldämpfungsdiagramm) | basic attenuation α0 per 100 m cable length | drawing 202; *Voll-PE / PE-Schaum / Massivschirm* as §9 (slike_02) |
| „ZF“, „NF“, „ZF-Amp.“, „NF/Basisband“, „zum Oszillator“ (Zeichnungsbeschriftungen) | "IF" ("ZF"), "AF" ("NF"), "IF amp." ("ZF-Amp."), "AF/baseband" ("NF/Basisband"), "to oscillator" ("zum Oszillator") | a label already in brackets keeps the German in a second bracket: ("AF" ("NF")); the terminal letters „E“ / „A“ stay, like *U_E* / *U_A* (slike_02) |

## 15. Catalogue structure

The 115 section titles of the question catalogue are translated in
`review/prijevod/naslovi.json` and applied to
`contents/questions/fragenkatalog3b.json`; they follow this glossary. The
three parts:

| German | English | Note |
|---|---|---|
| Prüfungsfragen im Prüfungsteil: Technische Kenntnisse | Examination questions in the examination part: Technical knowledge | |
| Prüfungsfragen im Prüfungsteil: Betriebliche Kenntnisse | Examination questions in the examination part: Operating knowledge | |
| Prüfungsfragen im Prüfungsteil: Kenntnisse von Vorschriften | Examination questions in the examination part: Knowledge of regulations | |
| Regelungen / Weitere Regelungen | provisions / other provisions | |
| Bestimmungen | provisions; regulations | |
| Allgemeines / Sonstiges | General / Miscellaneous | |
| Störfall / Störfälle | interference case / interference cases | EMVG heading |
| Rufzeichenanwendung | use of call signs | "Rufzeichen und Rufzeichenanwendung" → "Call signs and their use" |
