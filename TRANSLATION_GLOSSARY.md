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
| Fuchskreis | Fuchs matching circuit | |
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
| 5 W-Fragen | the five Ws (who, what, where, when, why) | emergency-message checklist |
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
| Oszillation/Pfeifen (Rückkopplung Mikrofon–Lautsprecher) | oscillation/whistling | acoustic feedback in a PA system (verstaerker_eigenschwingung tip) |

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
