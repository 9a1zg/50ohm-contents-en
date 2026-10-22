# nea_gesetze_und_vorschriften — translation report

Chapter "Gesetze und Vorschriften" (Laws and regulations): 9 sections, each
with its slides, no solutions. 18 files:

- `contents/sections/` and `contents/slides/`: `gesetze_vorschriften.md`,
  `amateurfunkdienst.md`, `amateurfunkstelle.md`, `funkamateur.md`,
  `zulassung.md`, `anschrift.md`, `gebuehren_beitraege.md`,
  `fernmeldegeheimnis_abhoerverbot.md`, `verstoesse_und_folgen.md`.

`revizija-guard.py --brojevi`: 18 files checked, *struktura netaknuta*.
German-word grep: the only German left is the `%` comment in
amateurfunkdienst, the German titles in brackets (*Grundgesetz*, *Gesetz über
den Amateurfunk*), the quoted letter of the brick campaign (see below) and the
URLs. Line counts, trailing spaces and the empty lines at the end of
gebuehren_beitraege are as in the German.

Embedded questions looked up in English and the prose aligned with them:
VA101–VA104, VA201, VA202, VA301, VA302, VC101–VC106, VC108, VC113,
VC122–VC125, VD113, VD114, VE101, VE103, VE201–VE204, VE701–VE704 (VA102
"self-training … intercommunication … technical investigations"; VA104 "duly
authorised persons … without pecuniary interest"; VA201 "accessory equipment
necessary at one location for operation"; VA202 "a station in the amateur
service"; VA301 "general provisions"; VA302 "communications incidental to the
purpose of the amateur service as defined and … remarks of a personal
character"; VC102, VC103 for the quoted AFuG definitions; VC108 "does not
provide for a minimum age"; VC113 "out of personal interest and not … out of
commercial interest"; VD113 "without delay after the change"; VD114 "unless
the holder has objected"; VE201, VE204 "eavesdropping on private (non-public)
conversations"; VE202 "receiving, using or passing on messages"; VC125 "can
punish the offence with a fine").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

18 rows: *Backsteinaktion / Mauersteine*; *Grundgesetz / Wirtschaftsrat /
Deutscher Bundestag*; *internationaler Fernmeldevertrag*; *Bundesminister für
Digitales und Verkehr*; *Rechtsgrundlage / Amateurfunkbetriebsrechte /
unmittelbar geltendes Recht*; *Funkdienste (Services) / Seefunk (Maritime
Service) / Rundfunk (Broadcasting Service)*; *Funkanwendungen mit
Allgemeinzuteilung*; *Gesetzgeber / öffentlich gesprochenes Wort*;
*Handwerksbetrieb*; *Zulassungsbescheid*; *Gebührenbescheid /
Zahlungsaufforderung*; *Verwaltungs-Vollstreckungsgesetz (VwVG) /
Vollstreckungsmöglichkeiten*; *Geheimhaltungspflicht / Verwertung und
Weitergabe*; *Rechtsgüterabwägung*; *Wanzen*; *Strafvorschriften /
Freiheitsstrafe / Geldstrafe / Täter / fahrlässig*; *eine Mitteilung machen
(§ 5 Abs. 2 TDDDG)*; *Bußgeldvorschriften / Aberkennung*.

## Added to `DECISIONS.md`

None. The unit follows the existing entries: German statutes under the
glossary's English names, RR provisions in the RR's English wording, the
bracket rule, and the generic *er* recast without a pronoun.

## Judgement calls

- All files: German law and bodies written out at first mention in each file, slides included — "Amateur Radio Act (Amateurfunkgesetz, AFuG)", "Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)", "Federal Network Agency (Bundesnetzagentur, BNetzA)", "Telecommunications Act (Telekommunikationsgesetz, TKG)" — also where the German has only the abbreviation; afterwards the abbreviation, or "the Amateur Radio Act" where the German writes the name out. *§ 2 Absatz 2 des Amateurfunkgesetzes* → "Section 2(2) of the Amateur Radio Act"; *§ 5 Absatz 2 Satz 1* → "Section 5(2) sentence 1" (glossary §1.2).
- gesetze_vorschriften: *der internationale Fernmeldevertrag, die sogenannten Radio Regulations (RR)* → "the international telecommunication treaty, the Radio Regulations (RR)", read as an apposition, as the later "des wichtigsten internationalen Fernmeldevertrages, den Radio Regulations (RR)" confirms; *(International Telecommunication Union, ITU)* and *(European Conference of Postal and Telecommunications Administrations, CEPT)* → "(ITU)" / "(CEPT)" after the English name (bracket rule); *allgemeine Regeln* of the RR → "general provisions", as VA301.
- gesetze_vorschriften (indepth): the protest letter's wording *"dass man sich damit über die schleppende Behandlung der Angelegenheit beschwere"* is a pun — *sich beschweren* is both "to complain" and "to weigh oneself down", which is the point of sending bricks. The quotation is kept in German, as the DECISIONS.md entry on quoted German usage does, with the English meaning and the double sense in brackets; an English pun would be an invention. *Dr. Plünder* → "Dr Plünder" (British style); *Wirtschaftsrat* → "Economic Council"; *Grundgesetz* → "Basic Law (Grundgesetz)"; *Backsteinaktion* → "brick campaign".
- gesetze_vorschriften: *Bundesminister für Digitales und Verkehr* → "Federal Minister for Digital and Transport" (the ministry's own English name); *Das Amateurfunkgesetz, das eigentlich Gesetz über den Amateurfunk heißt* → "whose actual title is *Act on Amateur Radio* (*Gesetz über den Amateurfunk*)", VC101's answer with the German title, which is what the sentence is about; *frisch gebackener Funkamateur* → "newly licensed radio amateur".
- amateurfunkdienst: *Funkdienste (Services) … Seefunk (Maritime Service), Rundfunk (Broadcasting Service), Amateurfunk (Amateur Service)* → the English names alone (bracket rule); *Seefunk* → "maritime mobile service", the RR's name (glossary §1.1), rather than the bracket's "Maritime Service"; *WLAN* → "Wi-Fi", as earlier units.
- amateurfunkdienst: the purposes in VA102's RR wording ("self-training", "technical investigations", "intercommunication between radio amateurs"); the quoted § 2(2) AFuG in VC102's wording, with "(the)" for *(der)*; *Weltraumfunkstellen* → "space stations", *Sicherheitsfunkdienste* → "safety services" (glossary §1.1).
- amateurfunkstelle: the quoted § 2(3) AFuG in VC103's wording, except *Frequenznutzungsplan*, which stays "Frequency Usage Plan" as the German quote has it (glossary §1.2; see errors); *Sende- und Empfangsfunkanlagen* → "transmitters and receivers", as VC103.
- amateurfunkstelle: *Alle Äußerungen sind öffentlich gesprochene Worte* → "Everything said counts as public speech", and *das nicht öffentlich gesprochene Wort* → "private (non-public) conversations" (glossary §1.2, VE201, VE204), so the contrast and the link to the later section stay visible; *Funkpartner in anderen Staaten* → "the stations we work in other countries" (glossary §2 *Funkpartner*); slide bullet on RR content in VA302's wording.
- funkamateur: *Finanzielle Interessen* → "pecuniary interests" (glossary §1.1, VA104); *aus persönlicher Neigung und nicht aus gewerblich-wirtschaftlichem Interesse* → "out of personal interest and not out of commercial interest" (VC113); *Amateurfunkrelais* → "amateur repeater"; *Handwerksbetrieb* → "tradesman's business".
- zulassung: *Zulassungsbescheid* → "authorisation notice" in the text and "notice of authorisation" in the section's caption, beside the glossary's *Prüfungsbescheid* → "examination result notice"; the slide caption *Die Zulassungsurkunde* → "The licence document" (glossary §1.3), each as the German has it. Slide heading *Zulassung* → "Licence".
- zulassung: in the quoted news item *bei der Bundesnetzagentur Dortmund* → "at the Federal Network Agency (Bundesnetzagentur) in Dortmund" — German name given at first mention, but no abbreviation inside a quotation; § 4 AFuG translated faithfully, *fachliche Prüfung* → "examination of competence" (glossary §1.3).
- anschrift: link texts → "Online call sign search", "Call sign list as a PDF document"; slide note *Einbettung der Webseite zur Rufzeichensuche* → "Embedded web page for the call sign search"; URLs and the iframe attribute unchanged.
- gebuehren_beitraege: *EMVG* at first mention → "Electromagnetic Compatibility Act (EMVG)", the glossary's short form, rather than the long title with the German long title in brackets (DECISIONS.md: a German title of a dozen words in brackets helps no one); *Verwaltungs-Vollstreckungsgesetz (VwVG)* → "Administrative Enforcement Act (Verwaltungs-Vollstreckungsgesetz, VwVG)", since the course text gives the abbreviation (VE704 keeps the bare English name); *laufenden Gebühren* (section) → "regular fees", *laufenden Beiträgen* (slide) → "regular contributions", each as written (see errors).
- fernmeldegeheimnis_abhoerverbot: TDDDG at first mention with its German name; *ehemals TTDSG* → in the section "formerly the Telecommunications and Telemedia Data Protection Act (TTDSG)", so that the reader links it to VE204, which still names the TTDSG; on the slide, "formerly the TTDSG"; *sperrigen Namen* → "unwieldy name" (the English name is unwieldy too).
- fernmeldegeheimnis_abhoerverbot: § 27 TDDDG translated faithfully, the German's line structure kept — "Imprisonment for up to two years or a fine shall be imposed on anyone who" followed by the three numbered items, as § 323c StGB is quoted in notfunk; *eine Mitteilung macht* → "makes a disclosure" (the § 5(2) prohibition on telling others); *Rechtsgüterabwägung* → "balancing of legal interests"; *Wanzen* → "bugs".
- verstoesse_und_folgen: the generic *er* recast ("The person concerned can still call themselves a radio amateur, but is excluded …"; "A radio amateur who transmits … is using that frequency without an assignment"), as DECISIONS.md; *Zulassung für den Amateurfunkdienst* → "authorisation for the amateur service" (glossary §1.3), bare *Zulassung* → "licence"; *Aberkennung des Amateurfunkzeugnisses* → "taking away the amateur radio certificate"; § 9 AFuG list in VC124's wording, lower case in the section as the German, capitalised on the slide as the German.

## Suspected errors in the German original

- sections/amateurfunkstelle.md — the quoted § 2 Absatz 3 AFuG reads "im Frequenznutzungsplan für den Amateurfunkdienst ausgewiesenen Frequenzen"; the current AFuG, and VC103 embedded right after it, say *Frequenzplan* (the plan was renamed). Translated as written ("Frequency Usage Plan").
- sections/gebuehren_beitraege.md — "Neben den laufenden Gebühren fallen weitere Gebühren an": the annual payments just described are contributions (*Beiträge*), as the slide says ("Neben den laufenden Beiträgen"). Translated as written.
- sections/zulassung.md vs slides/zulassung.md — the same photo 91 is captioned "Der Zulassungsbescheid zur Teilnahme am Amateurfunkdienst" in the section and "Die Zulassungsurkunde" in the slides. Both translated as written.
- sections/fernmeldegeheimnis_abhoerverbot.md — "Dazu gehört bereits der Empfang selbst, aber auch die Verwertung und Weitergabe von Nachrichten, die …, verstoßen gegen das TDDDG" mixes two constructions; rendered with its evident meaning.
- Typos with no effect on the English: sections/ and slides/funkamateur.md "dürfen Ihre Arbeit" (*ihre*); sections/ and slides/anschrift.md "Änderung beim Namen oder bei der Anschrift sind" (*Änderungen*); sections/gesetze_vorschriften.md "dass die Regeln … kein unmittelbar geltendes Recht … ist" (*sind*), "Bestandteil des wichtigsten internationalen Fernmeldevertrages, den Radio Regulations" (*der*), "Amateurfunkverordnung  (AFuV)" (double space); slides/fernmeldegeheimnis_abhoerverbot.md "nicht-öffentlich" beside the section's "nicht öffentlich".
