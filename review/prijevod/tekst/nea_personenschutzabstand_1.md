# nea_personenschutzabstand_1 — translation report

Chapter "Personenschutzabstand (1/2)" (Safety distance for the protection of
persons, part 1): 11 sections, each with its slides, and 5 solutions. 27
files:

- `contents/sections/` and `contents/slides/`: `personenschutzabstand.md`,
  `effektive_strahlungsleistung_erp_1.md`,
  `aequivalente_isotrope_strahlungsleistung_eirp_1.md`,
  `aequivalente_isotrope_strahlungsleistung_eirp_2.md`,
  `effektive_strahlungsleistung_erp_2.md`, `sendeleistung_klasse_n.md`,
  `anzeige_ortsfester_amateurfunkanlagen.md`, `standortbescheinigung.md`,
  `personenschutzabstand_2.md`, `personenschutzabstand_grenzwerte.md`,
  `nahfeld.md`.
- `contents/solutions/`: `AG503.md`, `AK101.md`, `AK102.md`, `AK103.md`,
  `AK104.md`.

`revizija-guard.py --brojevi`: 27 files checked, *struktura netaknuta*.
German-word grep: the only German left is the `%` comments
(anzeige_ortsfester_amateurfunkanlagen, personenschutzabstand_grenzwerte,
slides/personenschutzabstand_2, the `% TODO` in effektive_strahlungsleistung_erp_1),
the idents, the formula subscripts (`P_\mathrm{Sender}`, `G_\mathrm{Antenne}`,
`P_\mathrm{Verluste}`), and the German names in brackets: *elektromagnetische
Verträglichkeit in der Umwelt* (EMVU), *Bundesamt für Strahlenschutz*, and
the title *Erläuterung der Bewertungsverfahren nach BEMFV* in AK103. Line
counts, trailing spaces and final newlines are as in the German, except
slides/effektive_strahlungsleistung_erp_1, where one line and a blank line
are dropped (see below).

Embedded questions looked up in English and the prose aligned with them:
NK201, VE501–VE519, VD107, VC121, VD724–VD726, VD743, NG401, NG402,
EG501–EG511, AG501–AG503, AK101–AK104, EK101–EK104, EK107 (VE504 "ensure and
document independently that there is no danger to persons"; VE502
"electromagnetic compatibility with the environment"; VE505 the names of the
26. BImSchV and BEMFV; VE509 "competent regional office … before the amateur
radio installation is put into operation"; VE512/VE513 "comprehensible",
"antenna patterns, a site plan, a construction drawing or sketch with
dimensions"; VE515 "simplified assessment procedure, field-strength
measurement, far-field calculation and near-field calculation", "Watt
Wächter"; VE516 "site-specific safety distance"; VE517 "considered together";
EG501/AG501 "the product of the power supplied directly to the antenna and its
gain … in a given direction"; EG511 "notification of a fixed amateur radio
installation under Section 9 BEMFV"; AK102 "wave impedance of the medium";
AK104 "power at the antenna input", "attenuation factor $D$"; EK102 "RMS value
averaged over 6 minutes", "instantaneous peak value", "Annex 1a/1b/3"; EK103
"maximum instantaneous value"; EK107 "from every point of the antenna").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

12 rows: *Gewinnfaktor (Kurstext, Klasse N)*; *Kugelstrahler, fachsprachlich
isotroper Strahler*; the German's English glosses of EIRP / ERP;
*Feldwellenwiderstand $Z_\mathrm{F}(d)$ / des freien Raums*; *Fresnel-Bereich
/ Strahlungswiderstand / Feldanteile*; *Momentaner Spitzenwert /
6-Minuten-Intervalle / Gepulste Felder*; *Bundesamt für Strahlenschutz*;
*Eindringtiefe / Thermoregulation / Kraftwirkungen / Wärmewirkung /
Energieabsorption*; *nachvollziehbar*; *kontrollierter Bereich*; the two BNetzA
document titles (*Anleitung zur Durchführung der Anzeige …*, *Erläuterung(en)
der Bewertungsverfahren nach BEMFV*); *Mobilfunknetz-Betreiber*.

## Added to `DECISIONS.md`

1 entry (Course text): *Gewinnfaktor* → gain factor (the questions keep "a gain
of … (as a power ratio)"), *Kugelstrahler, fachsprachlich isotroper Strahler* →
"a *spherical radiator*, known technically as an *isotropic radiator*" and
otherwise *isotropic radiator*, *Feldwellenwiderstand* $Z_\mathrm{F}(d)$ →
wave impedance (AK102) beside $Z_0$ → impedance of free space, and the German's
English glosses of ERP / EIRP dropped, "isotropic" written "isotropically".
Part 2 of the chapter (nea_personenschutzabstand_2) follows it.

## Judgement calls

- personenschutzabstand: *Radio waves … gehören zu den elektromagnetischen Wellen* → "are electromagnetic waves", as the checker of nea_elektrische_schwingungen_funkwellen had it; the EMVU at first mention as law and institution names are: 'what is called "electromagnetic compatibility with the environment" (*elektromagnetische Verträglichkeit in der Umwelt*, EMVU)', since EMVU is a German abbreviation the reader keeps meeting (VE501).
- personenschutzabstand: the 26. BImSchV at first mention in the glossary's form, "26th Ordinance implementing the Federal Immission Control Act" (Ordinance on Electromagnetic Fields, 26. BImSchV); the BEMFV as "Ordinance on the Verification Procedure for Limiting Electromagnetic Fields" (BEMFV), the long title with the abbreviation only (DECISIONS.md, statutes); on the slides the titles without the short name, as the German.
- *Sendeanlage* → "transmitting equipment" throughout (glossary §1.3, EG511), *Funkanlage* → "radio installation", *Amateurfunkanlage* → "amateur radio installation"; *Mobilfunknetz-Betreiber* → "mobile network operators".
- personenschutzabstand indepth and standortbescheinigung: the Federal Network Agency at first mention in each section as "Federal Network Agency (Bundesnetzagentur, BNetzA)"; in anzeige_ortsfester_amateurfunkanlagen, where the German first writes "BNetzA", the full form is given there; citations stay short: "Section 9 BEMFV" (EG511).
- effektive_strahlungsleistung_erp_1: *Gewinnfaktor* → "gain factor" throughout the Class N sections (DECISIONS.md); *Hauptstrahlrichtung* → "direction of maximum radiation" (glossary §9); *wie bei einer Taschenlampe … gebündelt* → "concentrated into a forward beam, as with a torch" (British *torch*).
- effektive_strahlungsleistung_erp_1 and aequivalente_isotrope_strahlungsleistung_eirp_1: *(vom englischen "effective radiated power")* and *nach dem englischen Begriff "equivalent isotropic radiated power"* dropped (bracket rule): "usually abbreviated to ERP", "It is abbreviated to EIRP"; the term written as the established "equivalent isotropically radiated power" (glossary §9, RR 1.161).
- slides/effektive_strahlungsleistung_erp_1: the line *Effective radiated power* under the heading "Effective radiated power (ERP)" only repeated the heading in English, so it and its blank line are dropped (bracket rule, as earlier slide bullets that only gave the English term); slides/aequivalente_isotrope_strahlungsleistung_eirp_1 keeps "*Equivalent isotropically radiated power*" under the bare heading "EIRP", where it is the expansion.
- aequivalente_isotrope_strahlungsleistung_eirp_1: *einen sogenannten Kugelstrahler, der fachsprachlich auch als isotroper Strahler bezeichnet wird* → "what is called a *spherical radiator*, known technically as an *isotropic radiator*"; slide heading → "Spherical radiator or isotropic radiator"; every later *Kugelstrahler* (eirp_1 indepth, eirp_2, sendeleistung slides "isotropen Kugelstrahler") → "isotropic radiator" (DECISIONS.md). Slide note on the Greek origin: 'isotropic: from Ancient Greek ἴσος isos "equal" and τρόπος tropos "turn, direction"'.
- aequivalente_isotrope_strahlungsleistung_eirp_2: *Leistungsfaktor* → "power ratio" (glossary §14), bare *Faktor* → "factor"; table header "≈ Power ratio" and caption "Important power ratios in dB", as in dezibel_1 and kabeldaempfung_1 (without adding `\unit`, which the German caption here does not have); *Anpassgeräte* → "antenna tuning units"; *Verstärkungs- und Dämpfungsglieder* → "several stages that amplify or attenuate".
- aequivalente_isotrope_strahlungsleistung_eirp_2 (EG511): the sentence split around the displayed formula ("… can be split up into" / formula / "and Table [ref:…] gives the factor …") keeps the German's line structure; *nicht-QRP-Gerät* → "equipment that is not a QRP rig".
- slides: *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", *Lösungsweg gleich wie vorher* → "Same method as before", as in earlier units.
- effektive_strahlungsleistung_erp_2 and solution AG503: link text *Anlage 1 der AFUV* → "Annex 1 to the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)", as earlier units; slide *Der Frequenzplan für das 630 m-Band* → "The frequency plan for the 630 m band", lower case, as written (see errors); slide table header "Power ratio / Voltage ratio", caption "Power and voltage ratios for important values of loss and gain".
- sendeleistung_klasse_n slides: *Ein Funkgerät mit 5 W Sendeleistung und einem Gewinnfaktor von 1,8 … darf damit betrieben werden* → "A radio with 5 W transmit power may be operated with an antenna whose gain factor relative to the isotropic radiator is 1.8" — the German gives the radio a gain factor; the English attaches it to the antenna the example is about (see errors).
- anzeige_ortsfester_amateurfunkanlagen: *Personenschutz-Sicherheitsabstand* → "safety distance for the protection of persons", *standortbezogener Sicherheitsabstand* → "site-specific safety distance", *kontrollierbarer Bereich* → "controllable area" (glossary §1.4); *nachvollziehbar* → "comprehensible" (VE512, VE513), also in the tip that names it as the key word; *Spitzfindig betrachtet* → "*Splitting hairs*" (glossary §14).
- personenschutzabstand_2: *Selbsterklärung* → "self-declaration" (glossary §14), *Umgangssprachlich … bezeichnet* → "Radio amateurs informally call this"; *kontrollierten Bereichs* → "controlled area", as the German writes it, though the defined term is *kontrollierbar* (see errors); *Äquivalente Isotrope Strahlungsleistung*, capitalised in the German, in lower case.
- personenschutzabstand_2 and nahfeld: the BNetzA documents as link text in English: "Instructions for notifying fixed amateur radio installations under Section 9 BEMFV", "Explanations of the assessment procedures under the BEMFV"; in AK103, which cites the document as its source without a link, the German title follows in brackets so that the reader can find it, as the formula-sheet keywords (DECISIONS.md). The passages AK103 quotes from it are translated faithfully (no official English text).
- personenschutzabstand_grenzwerte: *Bundesamt für Strahlenschutz* → "Federal Office for Radiation Protection (Bundesamt für Strahlenschutz)", the office's own English name; *Verordnung über elektromagnetische Felder (26. BImSchV)* → "Ordinance on Electromagnetic Fields (26. BImSchV)"; *Anhang 1 (Tabellen 1a und 1b) sowie … Anhang 3* → "Annex 1 (Tables 1a and 1b) and … Annex 3" (glossary §1.2, EK102); *in kV/m über Hz* (the axes of the graphs) → "in kV/m against Hz"; *quadratischer Mittelwert … gemittelt über 6 Minuten* → "RMS value …, averaged over a period of 6 minutes" (EK102); *Kraftwirkungen und eine Wärmewirkung* → "force effects and a heating effect".
- slides/personenschutzabstand_grenzwerte: `$\textrm{Körpergröße} \approx \frac{\lambda}{2}$` → `$\textrm{body height} \approx …$`, a word written as a quantity (DECISIONS.md, *Vor/Rück*); heading *Körperhilfen* → "Implants", the bullets "Active implants" (glossary §1.4).
- nahfeld: *Feldwellenwiderstand* $Z_\mathrm{F}(d)$ → "wave impedance", *Feldwellenwiderstand des freien Raums* → "impedance of free space" (DECISIONS.md, AK102); the `\text{}` labels under the braces translated ("quasi-static", "inductive", "radiation"), as running words; *Lerninhalte der Klasse A* → "the syllabus of Class A"; *nebenstehende Vertiefung* → "the in-depth box alongside"; *Blindanteil / Wirkanteil (Strahlungswiderstand)* → "reactive part / resistive part (radiation resistance)" (glossary §5).
- AK101, AK103: *ist nicht zulässig* → "is not permissible" (not "may not", which a British reader can take as "might not"); *Fresnel-Bereich* → "Fresnel region"; headings *Erklärung* / *Erläuterung* → "Explanation", *Merksatz* → "Remember" (glossary §14 *Merke:*).
- AK102: *Wellenwiderstand Z* → "wave impedance $Z$" (AK102, glossary §3), *Wellenwiderstand des freien Raums* → "impedance of free space".

## Suspected errors in the German original

- sections/aequivalente_isotrope_strahlungsleistung_eirp_2.md (EG510) — "$\qty{1}{\dB}$ entspricht, laut unserer Tabelle [ref:e_dezibel_leistungsfaktoren], einem Faktor von $\num{1,26}$": the table referred to (in the margin of the same section) has no entry for 1 dB; the factor 1.26 is in the formula sheet's other table (shown as `Pegel_Verhältnis` in slides/effektive_strahlungsleistung_erp_2). Translated as written.
- slides/sendeleistung_klasse_n.md — "Ein Funkgerät mit 5 W Sendeleistung und einem Gewinnfaktor von 1,8 … darf damit betrieben werden": the gain factor belongs to the antenna (VD726), and "damit" has nothing to refer to. Rendered with the antenna as the bearer of the gain factor.
- slides/effektive_strahlungsleistung_erp_2.md — "Der Frequenzplan für das 630 m-Band gibt eine maximale ERP von 1 W vor": the section and solution AG503 take the limit from Annex 1 to the AFuV, not from a frequency plan. Translated as written ("frequency plan").
- solutions/AG503.md — "Einen Hinweis auf die richtige Lösung der nächsten Frage gibt schon die Anlage 1": copied from the section, where it introduces AG503; in the solution of AG503 itself, "the next question" points at the wrong question. Translated as written.
- sections/anzeige_ortsfester_amateurfunkanlagen.md — "für eine Amateurfunkstelle mit mehr als 10 W EIRP": two paragraphs earlier, and in VE507–VE509, the threshold is 10 W EIRP *or more*, and the indepth box makes the point that exactly 10 W already needs the procedure. Translated as written ("more than").
- sections/personenschutzabstand_2.md — "dass sie innerhalb des kontrollierten Bereichs liegen": the term defined in anzeige_ortsfester_amateurfunkanlagen and used in VE512 is the *kontrollierbarer* (controllable) area. Translated as written ("controlled area").
- solutions/AK103.md — `$r = \sqrt(\frac{Z_0}{4 \cdot \pi}) \cdot …$`: `\sqrt(` takes only the opening bracket as its argument, so the root sign does not cover the fraction; it should be `\sqrt{\frac{Z_0}{4 \cdot \pi}}`. Also `\qty{120\pi}{\Ohm}` (three times) uses `\Ohm`, where the rest of the course writes `\ohm`. Formulas left unchanged.
- sections/aequivalente_isotrope_strahlungsleistung_eirp_1.md — the English expansion given as "equivalent isotropic radiated power"; the RR (1.161) term is "equivalent isotropically radiated power". Written in the RR form (DECISIONS.md).
- Typos with no effect on the English: sections/personenschutzabstand.md "Felder“ (BEMFV)" (closing quote without matching opening quote); sections/ and slides/aequivalente_isotrope_strahlungsleistung_eirp_1.md "Hat eine Antennen" (*Antenne*); sections/aequivalente_isotrope_strahlungsleistung_eirp_2.md "Stahlungsleistung" (*Strahlungsleistung*), "Bei vielen Transeiver" (*Transceivern*), "mindesten" (*mindestens*), "in dem man" (*indem*), "Beiden gleichen sich" (*Beide*), "wenden … an um" (comma missing), "EIRP also ist" (word order); sections/effektive_strahlungsleistung_erp_2.md and solutions/AG503.md "AFUV" (*AFuV*), AG503 "Zu Lösung der Frage kann auf … zurückgreifen" (*Zur*, subject missing); sections/sendeleistung_klasse_n.md "dürfen die Antennen verwenden" (*Antenne*); slides/sendeleistung_klasse_n.md "vorangig" (*vorrangig*); slides/standortbescheinigung.md "befinden sich bereits eine ortsfeste Funkanlage" (*befindet*); sections/personenschutzabstand_2.md "Äquivalenten Isotropen" (lower case); sections/personenschutzabstand_grenzwerte.md "die biologische Wirkungen von hochfrequenten Felder" (*biologischen*, *Feldern*), comment "des Personenschutzabstand" (*-abstands*); slides/personenschutzabstand_grenzwerte.md "deren Stärke die Grenzwerte … überschreiten" (*überschreitet*); slides/personenschutzabstand_2.md "in einem Abstand von etwa bei 4λ" (*etwa* or *bei*); sections/nahfeld.md "rasch abfallenden … Feldanteile, hohe" (stray comma).
