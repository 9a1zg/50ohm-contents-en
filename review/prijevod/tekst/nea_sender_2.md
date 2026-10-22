# nea_sender_2 — translation report

Chapter "Sender (2/2)" (Transmitters, part 2): 11 sections, each with its
slides, and 6 solutions. 28 files:

- `contents/sections/` and `contents/slides/`: `dummy_load_1.md`,
  `dummy_load_2.md`, `unerwuenschte_aussendungen_1.md`,
  `unerwuenschte_aussendungen_2.md`, `unerwuenschte_aussendungen_3.md`,
  `elektromagnetische_vertraeglichkeit.md`, `stoerungen_vermeiden.md`,
  `stoerungen_elektronischer_geraete_1.md`,
  `stoerungen_elektronischer_geraete_2.md`, `empfangsstoerungen.md`,
  `remote_station.md`.
- `contents/solutions/`: `AI601.md`, `AJ106.md`, `AJ113.md`, `AJ118.md`,
  `AJ208.md`, `AJ211.md`.

`revizija-guard.py --brojevi`: 28 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comments (unerwuenschte_aussendungen_1
`% TODO: Editionsspezifisch machen`, stoerungen_vermeiden `% TODO
Editionsspezifisch anpassen:`, unerwuenschte_aussendungen_3 `%TODO BILD VON
DL1COM EINBAUEN`, stoerungen_elektronischer_geraete_1 `%- Reduzierung der
Sendeleistung …`, slides/unerwuenschte_aussendungen_2 `%Die Fragen habe ich …
(DL9MJ)`, all unchanged), idents, the formula subscripts ($R_\mathrm{ges}$,
$R_\mathrm{Zweig}$, $R_{ges}$), German names given on purpose (the EMVG's
German title, *Funkstörungsannahme*, *Funkanlagengesetz*, *Störung* /
*störende Beeinflussung*) and the publisher's name *DARC-Verlag*. Line counts,
leading and trailing whitespace (the markdown line breaks in the slides of
unerwuenschte_aussendungen_3, stoerungen_elektronischer_geraete_2 and
remote_station, the whitespace-only lines in unerwuenschte_aussendungen_2,
unerwuenschte_aussendungen_3 and elektromagnetische_vertraeglichkeit, the
indented picture lines in slides/unerwuenschte_aussendungen_2), the line
wrapping of the solutions AJ106, AJ113, AJ118, AJ208 and AJ211, and the
final-newline state are the same as in the German in every file.

Embedded questions looked up in English and the prose aligned with them:
VD110–VD112, NJ101, NJ102, NJ201, NJ202, NF107, NF404, NK101, NK102,
VC118–VC120, VE301–VE309, EF404, EJ101–EJ109, EJ111–EJ124, EJ201–EJ209,
EJ212–EJ214, EJ216, AI601–AI603, AJ101–AJ114, AJ116–AJ119, AJ203, AJ204,
AJ207–AJ211, AJ214, AJ219, AJ222–AJ225, AF701–AF710 (e.g. NF107 "output
stage", VD112 "unmodulated … carrier", NJ201 "does not cause any unwanted
emissions", VD110 "lowest possible level", EJ209 "at the transmitter output,
including any SWR meter", EJ202 "harmonic filter", AJ210 "rejector circuit",
EF404 "operating point of the output stage has been readjusted", EJ213 /
AJ219 "spurious emissions" / "spurious products", EJ212 "AF level or the
frequency deviation", AJ224 / AJ225 "maximum PEP of the transmitter",
AJ203 "third overtone (Oberwelle)" against AJ204 "third harmonic", EJ101 /
EJ102 / AJ105 "conducted pick-up" / "radiated pick-up" / "direct pick-up",
EJ104 / AJ101 "minimum necessary for satisfactory communication", EJ124
"competent regional office … examine the situation", VE301 "keep good
relations with the neighbours", VE303 / VE304 "in cooperation with those
involved", VE307 "radio interference reporting service", EJ119
"common-mode choke", AJ114 "insertion loss", AJ214 "spurious resonances",
"self-resonance", AJ106 "at a base-emitter junction" quoted verbatim in the
solution, AF707 "IP-controlled mains socket", AF708 "watchdog", AF710
"latency", AF701–AF705 "Block 1/2/3", "control unit", "remote interface").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

29 rows: *Störung / störende Beeinflussung* (set apart); *Beeinflussung /
beeinflussen* without *störend*; *Übersteuerung* (receiver / transmitter);
*Abschlusswiderstand oder künstliche Antenne*; *induktionsarme Widerstände /
Anzapfung / Masseanschluss*; *Teilspannung / Teilungsverhältnis*; *Anzeige:*
(advertisement); *DARC-Verlag / Bausatz*; *Verfügung 33/2007*;
*Oberwellendämpfung*; *maximaler Sendesignalspitzenpegel (PEP)*; *Oberwellen
bzw. Harmonische (engl. harmonics)*; *CE-Erklärung / ETSI Norm*;
*Einstreuungen von NF-Signalen*; *UKW-Rundfunk / -Rundfunkbereich /
-Radiosender*; *Bandstoppfilter (Bandsperren)*; *Ober*schwingungen
(emphasis); *Funkstörungsannahme / Funkstörannahme*; *Referenten / Referat
für EMV, Distrikte*; *Jetzt Mitglied im DARC werden!*; *Konfliktfall / Leib
und Leben / Sachen von bedeutendem Wert*; *Garagentorsteuerung /
Funk-Autoschlüssel / LED-Leuchten mit kapazitiven Sensoren*;
*Mantelwellen-Sperren (Verdrosselung) / Gleichtaktströme / Klappringkerne*;
*Aussetzer / Artefakte / Verstummen*; *Längsimpedanz / Eigenresonanz /
Leistungscharakteristik*; *Powerline Communication / Afu-Bänder*;
*Sicherungen ausschalten*; *Standort des Operators / Remote-Standort /
Bedienteil / Block 1–3*; *Laufzeiten im Netzwerk / Verarbeitungszeiten*.

## Added to `DECISIONS.md`

One entry (Course text):

- *Störung* against *störende Beeinflussung*: where the course text sets them
  apart (limits exceeded vs. limits kept but equipment upset by the wanted
  signal), *interference* / *breakthrough*, the RSGB's established term for
  the second; the German words named once; plain *Beeinflussung* → effect;
  the question bank's *interference* for both (EJ103, EJ110, EJ112, AJ108,
  AJ111) left as it is.

## Judgement calls

- dummy_load_1: *Abschlusswiderstand oder künstliche Antenne* → "a *termination* or an artificial antenna" (both established English names, so not a gloss to drop); *(vgl. Kapitel Bauteile und Schaltkreise)* → "(see the chapter on components and circuits)", chapter titles described as in earlier units; *Störungen bei anderen Funkverbindungen* → "interference to other contacts" (glossary §2 *Funkverbindung*); *nur auf freien Frequenzen* / slide *Auf freier Frequenz* → "on frequencies that are not in use" (as BE105); *Träger ohne Modulation* kept as "a carrier without modulation"; slide *Anpassgeräte* → tuning units; photo caption *Dummy Load* → "Dummy load".
- dummy_load_2: *Dummyload für den HF-Bereich* → "for radio frequencies" / slide heading "Dummy load for RF" (HF = Hochfrequenz); *möglichst einem rein ohmschen Widerstand von 50 Ω entspricht* → "behaves as closely as possible like a purely resistive 50 Ω"; *Masseanschluss* → chassis connection (§4 *Masse*; AI603's "earthed end" is the bank's *erdnahes Ende*); *Anzeige:* in the margin is an advertisement, not a display → "*Advertisement:*"; *im DARC-Verlag als Bausatz bestellen* → "order it as a kit from [DARC-Verlag]", the publisher's name kept; `<warning>` kept as written (not in the guard's tag list, unchanged); worked slide *Lösungsweg / gegeben / gesucht* → "Solution / given / required", *Reihen mit je 4 Widerständen* → "Chains of 4 resistors each", caption *Widerstandsketten* → "chains of resistors"; the trailing blank line of the slide file kept.
- unerwuenschte_aussendungen_1: *beim Sender gelernt* → "in the chapter on the transmitter"; *Flugfunk* → aeronautical radio (§14); *Amateurfunkgesetz* in the in-depth box translated as written, "Amateur Radio Act (Amateurfunkgesetz, AFuG)" (see errors); slide *Amateurfunkverordnung (AFuV)* → full form at first mention on the slides.
- unerwuenschte_aussendungen_2 (Class E): *Oberwellen* / *Oberschwingung* → harmonics throughout — this lesson does not set them against *Harmonische* (DECISIONS.md *Oberwelle*); *Oberwellenfilter* → harmonic filter (EJ202); *Nebenaussendungen* → spurious emissions, *Nebenprodukte* → spurious products, „Splatter" → "splatter" (glossary §6, EJ213, AJ219, as ssb_3); *im UKW-Rundfunkbereich* → "in the FM broadcast band (VHF)" (glossary §10; see errors); caption 1008 keeps the drawing's abbreviations "(OW)", "(NA)", which stay German until the drawings are done; caption 745 rendered identically here and in stoerungen_vermeiden (*Oberwelle* / *Oberschwingung*); *Kurzwellenbereich* → HF range; *Aufbereitung des Sendesignals* → processing of the transmitted signal; *NF-Aussteuerung* → AF drive (§14); *benachbarte Stationen* → "stations on adjacent frequencies" (EJ214), so that it is not read as the neighbours; slide note *UKW-Radiosender* → "FM broadcast stations (VHF)".
- unerwuenschte_aussendungen_3 (Class A): here the text sets *Oberwelle* against *Harmonische* (the table, the slides) → *overtone* / *harmonic* as nicht_sinus_signale, with the table and its caption worded identically to the shared table `a_harmonische` there; where *Oberwellen* only means unwanted multiples (AJ207 "generating harmonics", the legal limits, the spectrum analyser, the mixer filters) → harmonics; *Oberwellen bzw. Harmonische (engl. harmonics)* → "the harmonics" (glossary row); picture 868 caption "Overtones (OW), harmonics (Harm.) and spurious emissions (NA)", the leading space inside the caption kept; *Verfügung 33/2007 der Bundesnetzagentur* → "Order 33/2007 of the Federal Network Agency (Bundesnetzagentur, BNetzA)" (§1.2 *Verfügung*), the link unchanged; *Sperrkreise* → rejector circuits (AJ210); tip *Der UKW-Rundfunk ist der klassische Rundfunk auf Ultrakurzwelle (UKW)* → "VHF FM broadcasting is the "classic" radio broadcasting on very high frequencies (VHF)"; *ETSI Norm EN 301783* → "ETSI standard EN 301783"; *2-m- oder 70-cm-Band* → "2 m or 70 cm band"; *mit Brummspannung behaftet* → "with a ripple voltage on its output" (§5 *Brummspannung*); *verbrummter Träger/Ton* → "buzzing" carrier or tone (§10); worked slides *Radiobereich* → "broadcast band", *3. Oberwelle* → "3rd overtone" (AJ203).
- elektromagnetische_vertraeglichkeit: EMVG at first mention in the section and on the slides in the glossary's course-text form "Act on the Electromagnetic Compatibility of Equipment (Gesetz über die elektromagnetische Verträglichkeit von Betriebsmitteln, EMVG)" (VC118); *Schutzanforderungen zur Gewährleistung der EMV* → "protection requirements for ensuring electromagnetic compatibility" (VC118); *WLAN* → Wi-Fi; spaced hyphens used as dashes → en dashes; the double space after "mains." kept.
- stoerungen_vermeiden: *Störung* / *störende Beeinflussung* → interference / breakthrough (DECISIONS.md), the German words named once in the in-depth box; *Einstrahlung über eine Empfangsantenne / Direkteinstrahlung / Einströmungen* → radiated pick-up / direct pick-up / conducted pick-up (§12, EJ101, EJ102, AJ105); *ob er der Verursacher ist* → "whether they are the cause" (DECISIONS.md generic *er*); *Funkstörungsannahme der Bundesnetzagentur* → "radio interference reporting service (Funkstörungsannahme) of the Federal Network Agency (Bundesnetzagentur, BNetzA)" (§1.2), afterwards "BNetzA" where the German repeats the full name; *Referenten für elektromagnetische Verträglichkeit* → "electromagnetic compatibility officers", *Referat* (slide note) → department; *nachbarschaftlicher Frieden* → "good relations with the neighbours" (VE301); *Konfliktfall* → "a case of conflict"; slide headings *1./2./3. Fall* → "Case 1/2/3"; *Ursachenforschung / Ermittlung / Überprüfung* → "Looking for the cause / Finding the cause / Check".
- stoerungen_elektronischer_geraete_1: *störende Beeinflussung* → breakthrough, plain *Beeinflussung(en)* → effects / "affected" (DECISIONS.md); *Hierbei spricht man von Übersteuerung oder störender Beeinflussung* → "This is called *overloading* of equipment, or *breakthrough*" (EJ103's correct answer says "overloading or interference", see the decision); *Übersteuerung* of a receiver → overloading (EJ106, EJ107); *Mantelwellensperre* → common-mode choke (§12, EJ119), *Gleichtaktströme auf dem Mantel und dem Innenleiter des beeinflussten Gerätes* → "on the braid and the inner conductor to the affected equipment"; *Klappringkerne aus Ferrit* → clip-on ferrite cores; *zuständige Außenstelle der BNetzA* → "competent regional office" (EJ124); *geschlossenes Metallgehäuse* → "a metal case that is as fully enclosed as possible" (EJ108); *die Kurzwelle* → "the HF range"; the double blank line before "Not all breakthrough" kept.
- stoerungen_elektronischer_geraete_2: *Empfangsstörungen* → "interference to reception"; *VDE-Vorschriften* → VDE regulations; *Modulationsarten CW sowie SSB* → "the types of modulation CW and SSB" (§14 *Modulationsarten*); *Basis-Emitter-Strecken* → base-emitter paths (§14); *UKW-Empfänger* → VHF FM receivers (AJ112); *Abblockkondensatoren* → decoupling capacitors, *gegen Masse ableiten* → divert to chassis; *Eigeninduktivität* → self-inductance; *HF-Frequenzen* → radio frequencies; *Längsimpedanz* → series impedance; *Einbrüchen in der Leistungscharakteristik* → "dips in the power response"; slide heading *Störpotential unterschiedlicher Betriebsarten* → "Interference potential of different modes".
- empfangsstoerungen: *Verursacher* → culprits; tip reworded to keep who supports whom ("members can get support, with expertise and measuring equipment, from the DARC's electromagnetic compatibility officers"); slide note *FuAG: Funkanlagengesetzes* → "Radio Equipment Act (Funkanlagengesetz, FuAG)" (glossary), *Funkstörannahme* → the service's name *Funkstörungsannahme*; *Sicherungen ausschalten* → "Switch off circuits at the fuse box"; *Hier DARC-Werbung machen* → "Promote the DARC here".
- remote_station: *Remote-Standort* → remote site, *Bedienteil* → control unit (§6, AF701); *Block 1/2/3* capitalised as a label, as AF703's answers; the Block 3 sentence (*angesteuert/rückgemeldet durch Signale …*) → "are controlled by the remote interface or a computer at the remote site, and report back to it, by means of signals …"; *Laufzeiten im Netzwerk* → "transit times in the network" (glossary §14 *Laufzeit*), slide *Latenzen* → latency (AF710); *sog. Watchdog* → "what is called a watchdog"; *IP-Steckdose* → IP-controlled mains socket (AF707); *Remote-Clubstationen* → remote club stations; *SWL-Betrieb* kept as SWL operation.
- Solutions: AI601 *Dauerleistung* → continuous power (AI601); AJ106 the answer quoted as the English answer "at a base-emitter junction"; AJ113 *normkonforme Oberwellenunterdrückung* → "harmonic suppression that complies with the standards", *Flankensteilheit* → skirt steepness (§5), " - " → en dash; AJ118 *kapazitiver / induktiver Widerstand* → capacitive / inductive reactance, *Adern* → cores, *Querstrom* → "the current flowing through the capacitors" (not the divider current of §14), *Ausschlussverfahren* → "a process of elimination"; AJ208 *Bandstoppfilter (Bandsperren)* → "band-stop filters" (bracket rule), the German's emphasis on *Ober*-schwingungen carried by italicising *harmonics* (glossary row); AJ211 *lineare Klasse-A-Treiberstufe* → "linear class A driver stage" (AJ211).

## Suspected errors in the German original

- sections/unerwuenschte_aussendungen_1.md (in-depth box) — "Auch wenn das Amateurfunkgesetz nur allgemein verlangt, dass unerwünschte Aussendungen auf das geringstmögliche Maß zu beschränken sind": the slide of the same section, unerwuenschte_aussendungen_3 and VD110 attribute this requirement to the *Amateurfunkverordnung* (AFuV), not the AFuG. Kept ("Amateur Radio Act").
- sections/unerwuenschte_aussendungen_2.md — "die Aussendung einer Oberschwingung eines Transceivers im UKW-Rundfunkbereich … ($\qty{145,9}{\mega\hertz}\cdot 4 = \qty{583,6}{\mega\hertz}$)": 583.6 MHz is in the UHF television band (DVB-T2, as picture 745 shows), not the VHF FM broadcast band. Kept.
- sections/stoerungen_vermeiden.md (in-depth box) — the example "Oberschwingung von einem Kurzwellentransceiver im UKW-Rundfunkbereich" is illustrated by picture 745, which shows DVB-T2 television interference from a 2 m harmonic (the same picture as in unerwuenschte_aussendungen_2). Kept.
- slides/unerwuenschte_aussendungen_3.md (AJ204 working) — "Radiobereich: $\qtyrange{88,5}{108,0}{\mega\hertz}$": the tip in the section gives the FM broadcast band as 87.6–107.9 MHz; the slide's lower edge is the computed 88.5 MHz itself. Kept.
- slides/dummy_load_2.md (AI601 working) — $R_S = 4\cdot\qty{150}{\ohm}$ is listed under "gegeben" although it is derived, and $n_S$ there counts the parallel chains, while the section uses $N_\mathrm{S}$ for the number of resistors in series in each branch and $N_\mathrm{P}$ for the parallel branches. Kept.
- sections/stoerungen_elektronischer_geraete_1.md — TV reception "z. B. $\qtyrange{470}{690}{\mega\hertz}$", while solution AJ113 gives DVB-T2 in Germany as 470–694 MHz (694 MHz is the band edge). Kept.
- sections/unerwuenschte_aussendungen_2.md, _3.md — *Nebenaussendungen* is used for the splatter right next to the transmitted signal; in the RR's terms (1.144, 1.145) emissions just outside the necessary bandwidth caused by the modulation are out-of-band emissions, not spurious emissions. The glossary (§6) and the bank (EJ213, AJ219) render *Nebenaussendungen* as spurious emissions; kept.
- sections/unerwuenschte_aussendungen_3.md — picture 868 and the table both carry the ident `a_harmonische`, and the text refers to both ("Abbildung [ref:a_harmonische]", "Tabelle [ref:a_harmonische]"); one of the references can only resolve to the wrong object. Idents never change; kept.
- Typos with no effect on the English: sections/unerwuenschte_aussendungen_1.md "sind unerwünschten Aussendungen daher"; sections/unerwuenschte_aussendungen_2.md caption "Störung des DVB-T2-Empfang", caption "Selbgebautes Tiefpassfilter", "welches nur auf einer gewünschten Frequenz aussendet sollte" (missing comma); sections/unerwuenschte_aussendungen_3.md "neben des klassischen Oberwellenfilters", "solche *Nebenaussendung*, oder auch *Nebenprodukte* genannt", "stabilierte"; sections/stoerungen_vermeiden.md and slides "Störung des DVB-T2-Empfang"; sections/stoerungen_elektronischer_geraete_1.md "Nichlinearitäten", "Probeleme", "zu beeinflussungen kommt"; slides/stoerungen_elektronischer_geraete_1.md "Übersteuerrung", "wegen ungenügend geschirmten Gehäuse", "trotz gesetzeskonformen Betrieb"; sections/stoerungen_elektronischer_geraete_2.md "mit Ihrer Induktivität"; slides/empfangsstoerungen.md "FuAG: Funkanlagengesetzes", "Funkstörannahme"; solutions/AJ208.md "ergibt als als"; the ident `a_stoerungen_elektrischer_geraete_tiefpassfilter` (idents never change).

## Provjera

Checker: all 28 files compared paragraph by paragraph with the German
(`git show dc8948e~1:<file>`), embedded questions looked up in English.
Every judgement call, the 29 glossary rows and the DECISIONS.md entry
(*Störung* / *störende Beeinflussung* → interference / breakthrough) were
examined: the decision and 28 rows kept as they are, one row reworked.
The suspected errors in the German are confirmed as listed.
`revizija-guard.py --rev dc8948e~1 --brojevi`: 28 files, *struktura
netaknuta*.

Changes: omission 0, meaning 3, technical 1, style 1, glossary 1.

- meaning — slides/unerwuenschte_aussendungen_1 (note): "Filters are not perfect, so keep them to the lowest possible level" made the filters what is kept low; now "so keep unwanted emissions to the lowest possible level", as the German means.
- meaning — slides/dummy_load_2: *HF-Teilspannung wird über Spannungsteiler-Verhältnis berechnet* "is converted using" → "is calculated using the divider ratio".
- meaning — slides/stoerungen_elektronischer_geraete_2: *komplette Ausfälle* "complete dropouts" → "complete loss of reception" (*Aussetzer* is the dropout; *Ausfall* is total failure).
- technical — solutions/AJ118: *Widerstand* of the series capacitors and series inductors at 50 Hz rendered "resistance" → "impedance"; a capacitor or inductor has no resistance in that sense, and the same solution already says "reactance" for *kapazitiver / induktiver Widerstand*.
- style — sections/stoerungen_elektronischer_geraete_1: "*common-mode chokes (choking)* to leads" → "*choking leads with common-mode chokes*" (the bracketed gerund is not English); "can form rectifying effects" → "can produce rectifying effects".
- glossary — §14 row *Mantelwellen-Sperren (Verdrosselung)*: "common-mode chokes (choking)" → "common-mode chokes", with the rendering of *Verdrosselung von Zuleitungen* noted.
