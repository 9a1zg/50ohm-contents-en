# nea_strom_spannungsversorgung_1 — translation report

Chapter "Strom- und Spannungsversorgung (1/2)" (Power supplies, part 1):
13 sections, each with its slides, and 23 solutions. 49 files:

- `contents/sections/` and `contents/slides/`: `spannungsquelle.md`,
  `innenwiderstand.md`, `netzgeraet_1.md`, `batterien_und_akkus.md`,
  `akku.md`, `photovoltaik.md`, `spannungswandler.md`, `gleichrichter_1.md`,
  `gleichrichter_2.md`, `brueckengleichrichter.md`,
  `vollweggleichrichter.md`, `restwelligkeit.md`, `schaltnetzteil_1.md`.
- `contents/solutions/`: `AB202.md`, `AB205.md`–`AB214.md`, `AB501.md`,
  `AD301.md`–`AD310.md`, `AG401.md`.

`revizija-guard.py --brojevi`: 49 files checked, *struktura netaknuta*.
German-word grep: no hits outside `%` comments (left in German, as markup),
picture and photo idents (`a_Strombegrenzung`, `Solarmodul mit Zellen`,
` Brückengleichrichter Bauformen`, `e_Ferritkerntrafo im Schaltnetzteils`
…), the symbol $ü$ and the VDE's German name, kept in brackets on purpose.
Files without a final newline in the German keep it that way.

Embedded questions looked up in English and the prose aligned with them:
AB201–AB214, AB501, AD301–AD310, AG401, ED301–ED304, EK205, NB201,
NB203, NB204, ND101–ND110, NK305, NK306 (e.g. ED301 "voltage stability",
AD301 "strings", AD303/AD304 "transformation ratio", "safety margin",
"voltage rating", AD309 "ripple", "hum frequency", ND108 "thermal
shutdown", "short-circuit current limiting", NK305 "tripping
characteristic").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

32 rows: *Labornetzgerät / Strombegrenzung*, *Quellenspannung /
Spannungsfall*, *Spannungs- / Stromanpassung*, *Sinusgenerator /
Ausgangsbuchse*, *3-adrige Leitung / Aderfarben / Aderkennzeichnung*,
*Haussicherung*, *Kontroll-Leuchtdiode / beleuchtetes Anzeigeinstrument*,
*äußerer Schleifkontakt*, *durchgebrannte Sicherung / Schmelzsicherung*,
*Auslösezeit / Abschaltzeit / Einschaltstrom / Nennstrom / Kennzeichen*,
*Akkumulator (Akku) neben Batterie*, *Tiefentladung / Stromentnahme /
Mindestspannung*, the battery chemistries, *Kfz-Sicherung / Anschlussbox /
verpolungsgeschützt*, *durchgestrichenes Mülltonnensymbol / Hausmüll*,
*Batteriefach / Fieldday*, *Nennspannung / Zellnennspannung / Verschaltung
(4S1P)*, *Balancer / Balanceranschluss / Batteriemonitor / Balance-Stecker*,
*Entladestrom / Entladezeit / entnehmbare Ladungsmenge*, *Photoelement /
Strang / Solarzellenverbund*, *photoelektrischer / photovoltaischer
Effekt*, *Spannungswandler / Hoch- / Tiefsetzsteller / Buck-Boost-Converter*,
*Einweggleichrichtung / Lastspannung*, *Leerlaufspitzenspannung /
Sicherheitsaufschlag*, *LC-Siebglied*, *Diodenringmischer*, *Bauformen /
Anschlussfolge* (bridge rectifiers), *Brummton / AC-Kopplung / galvanische
Kopplung*, *Schaltnetzteil (engl. …)*, *Ferritkernübertrager*,
*Regelbarkeit / Ausfallwahrscheinlichkeit / Unterhaltungselektronik*, *Wo
Licht ist, ist auch Schatten*.

## Added to `DECISIONS.md`

One entry: *Akku* is a "rechargeable battery" where the German sets it
against *Batterie* (batterien_und_akkus, as ND110 and NK306), and a plain
"battery" where the text is about rechargeable batteries throughout (akku),
once the first mention has said "rechargeable".

## Judgement calls

- All files: *Netzgerät / Netzteil* → power supply unit / power supply (glossary §5); *Halbwelle* → half cycle (glossary §3), *Einweg- / Vollweggleichrichtung* → half-wave / full-wave rectification; *Ladekondensator* → reservoir capacitor, *Siebkondensator* → smoothing capacitor; *Trafo* → transformer; *Übersetzungsverhältnis* → transformation ratio, as AD303/AD304; *Lösungsweg / gegeben / gesucht* → "Solution / given / required", *vgl. Formelsammlung* → "see the formula sheet", as in earlier units.
- spannungsquelle: the VDE at first mention as "Association for Electrical, Electronic and Information Technologies (Verband der Elektrotechnik Elektronik und Informationstechnik e. V., VDE)", following the rule for German bodies; *Außenleiter / Neutralleiter / Schutzleiter* → line / neutral / protective earth conductor (glossary §12, EK205).
- spannungsquelle slides: *die Spannung zur "Erde" abzuleiten und damit die Haussicherung auszulösen* → "to conduct the voltage away to "earth" … and so to trip the household fuse"; *Nicht drauf verlassen, sondern messen!* → "Don't rely on it – measure!".
- innenwiderstand: *Koaxialkabel … können besonders hohe Leistungen übertragen, da der Strom im Kabel geringer verteilt wird* → "because of the way the current is distributed in the cable": the German reason is unclear (see errors), so the English does not invent a sharper one.
- innenwiderstand: the closing pun *die optimale Leistung in der Prüfung zu erreichen* (Leistung = power and performance) → "deliver the optimum performance in the examination"; the emoji kept.
- innenwiderstand: caption "Sinusgenerator mit 50 Ohm Innenwiderstand" and picture 1078 "50 Ohm als Kompromiss" → "50 Ω", the unit symbol after a number.
- netzgeraet_1: *"PE" ist die Abkürzung für den englischen Begriff "protective earth", der soviel wie Schutzerdung bedeutet* → ""PE" stands for "protective earth"": the German gloss only translates the English back (bracket rule); the slide note likewise.
- netzgeraet_1: *Schutzkontaktstecker (kurz Schukostecker)* → "Schuko plug (earthed plug)", as ND109; *Schutzkontakt* → earthing contact; *Schmelzsicherungen, in denen ein dünner Draht schmilzt* → "wire fuses, in which a thin wire melts"; *Abschaltzeit* → breaking time, *Auslösezeit* → tripping time; markings F / MT / T unchanged.
- netzgeraet_1 slides: *Schuko-Stecker haben keinen Verpolschutz für L- und N-Leiter* → "Schuko plugs do not prevent L and N from being swapped".
- batterien_und_akkus: *Akkumulatoren, kurz Akkus genannt* → "Accumulators, or rechargeable batteries as they are usually called"; *Akkus* → rechargeable batteries, *Batterien* → batteries ("non-rechargeable batteries" in "meistens Akkus, manchmal aber auch Batterien"), see DECISIONS.md; *Fieldday* → Field Day (glossary §2 *Fieldday-Contest*).
- batterien_und_akkus: *Lithium-Eisen-Phosphat-Mischungen (LiFePO4)* → "lithium iron phosphate compounds (LiFePO4)"; *Notebooks* → notebook computers; *Kfz-Sicherungen* → automotive fuses; *Mülltonnensymbol* → wheelie bin symbol (British).
- akku: *Akku* → battery throughout (LiFePO4 context), "rechargeable batteries" at first mention; *4 in Serie und das 2 mal parallel* → "4 in series, with 2 of these strings in parallel"; *Balancer, Batteriemonitor* kept as balancer, battery monitor.
- akku slides: *30C Constant / 40C Burst* → "30C constant / 40C burst"; *Kabelquerschnitt ist zu beachten* → "Mind the cable cross-section".
- photovoltaik: *Photoelement* → photovoltaic cell; *Stränge / Reihen* → strings, as AD301; *Solarzellenverbund* → array / interconnected solar cells.
- spannungswandler: *DC/DC-Wandler* → DC–DC converter, as AB213; *Step-UP-Wandler (Hochsetzsteller)* → "step-up converter (boost converter)", *Step-DOWN-Wandler (Tiefsetzsteller)* → "step-down converter (buck converter)" (glossary §5), the German capitals not carried over; photo captions *Abwärts- (Buck) Aufwärts- (Boost) Wandler* → "Buck-boost (step-down/step-up) converter"; slide note "0,5V bis 25V … 25W" → "0.5 V to 25 V … 25 W".
- gleichrichter_2: *im Kapitel "Gleichrichter I" der Klasse E* → "in the Class E chapter "Rectifiers I"": the section titles (toc) are not translated yet; the title is rendered so that it can be matched later.
- gleichrichter_2: *Bemessung von Diode und Kondensator* → "choosing the diode and the capacitor"; *ein zwanzigstel* → "one twentieth"; slides *Für die Diode ist die Spitzen-Spitzen-Spannung relevant* → "the peak-to-peak voltage is what matters".
- brueckengleichrichter: *Durch den geringen Aufwand* → "Because it takes so little effort"; tip *die "Striche" der Dioden* → "the "bars" of the diodes"; indepth list: type designations (26 MB 20 A, B80 C 5000/3300, BY 225, FPU 4M …) unchanged, *Anschlussfolge* → order of the terminals.
- vollweggleichrichter, AD307, AD308: *Mittelanzapfung* → centre tap; *Nulllinie* → zero line.
- restwelligkeit: *oszilloskopiert* → "displaying … on the oscilloscope"; *galvanische Kopplung* → "DC-coupled (galvanically coupled)", the established English name with the German's word beside it; button labels "GD", "AC/DC" unchanged.
- schaltnetzteil_1: *Schaltnetzteil (engl. switched-mode power supply)* → "switch-mode power supply", the gloss dropped (bracket rule), as ED302/ED303; *(siehe Abschnitt: Spannungsstabilisierung)* → "(see the section: Voltage stabilisation)".
- schaltnetzteil_1 slides: *Wo Licht ist, ist auch Schatten* → "there is no light without shadow"; *Kurzwellenbereich* → HF range.
- AB211, AD303, AD304, AB214: decimal commas in `0{,}9`, `1{,}5`, `0{,}8` written `0{.}9` …, as in AD101.

## Suspected errors in the German original

- slides/akku.md — "Der Akku wäre in 128 Sekunden entladen": at 126 A a 4.2 Ah battery lasts 4.2/126 h = 120 s. The commented-out section text says 108 s; both are wrong. Translated as written.
- slides/photovoltaik.md (AD301) — the result line names the total current $I_{0,\mathrm{ges}}$, though the "required" line and the given quantity use $I_{k,\mathrm{ges}}$ / $I_k$ (short-circuit current). Kept.
- sections/innenwiderstand.md — "Koaxialkabel mit … etwa 30 Ω können besonders hohe Leistungen übertragen, da der Strom im Kabel geringer verteilt wird": the reason given is unclear; the 30 Ω optimum for power handling comes from the trade-off between the breakdown voltage and the heating of the inner conductor. Translated as written, without a sharper reason.
- sections/innenwiderstand.md — "Da die Quellenspannung $U_q$ im Leerlauf, also ohne Belastung $U_q=U_L$ ist": $U_L$ is otherwise the voltage across the load; at open circuit the terminal voltage $U_k$ equals $U_q$.
- solutions/AD306.md — the calculation is labelled $U_{\mathrm{sek}} = U_{\mathrm{prim}}/8$, but it divides the *peak* primary voltage ($230 \cdot 1.414$) and so gives the peak secondary voltage $\hat{U}$ (40.65 V), not the RMS $U_{\mathrm{sek}}$. The result agrees with answer a.
- solutions/AD309.md — "Die Amplitude der Brummspannung beträgt genau ein Kästchen" (3 V): one square is the peak-to-peak ripple; the amplitude is 1.5 V, as answer c's "±1.5 V" shows.
- sections/restwelligkeit.md — "Ihre Frequenz beträgt 100 Hz, da auch die negative Halbwelle in den positiven Bereich gespiegelt wird": true only for full-wave (bridge or centre-tap) rectifiers; the section opens with "eines Gleichrichters" in general, and the half-wave rectifier of gleichrichter_2 gives 50 Hz.
- sections/restwelligkeit.md — button "GD": on oscilloscopes it is usually labelled GND. Kept as written.
- sections/gleichrichter_2.md — "Wir rechnen: $U_{\mathrm{sperr}} = 2 \cdot \hat{u}$" uses lower-case $\hat{u}$ while the rest of the section writes $\hat{U}$.
- sections/brueckengleichrichter.md — "(vgl. Abbildung [ref:a_netzteil_Ucs] verbaut": closing bracket missing; kept. The picture ident `a_brueckenlgeichrichter` (typo) is markup and kept.
- sections/brueckengleichrichter.md — item 2: "B80 C 5000/3300 … C kapazitive Last max. 2500 µF": the 2500 µF is not part of the designation and comes from the data sheet; harmless, but reads as if it were decoded from the code.
- sections/akku.md — "$\qty{3,3}{\volt} \cdot 4 = \qty{13,2 }{\volt} \cdot 1 = \qty{13,2}{\volt}$": the "· 1" (parallel strings) is attached to the result rather than written as $3.3 \cdot 4 \cdot 1$; kept.
- Typos with no effect on the English: sections/innenwiderstand.md "Ideallfall", "angeben" (for *angegeben*), "kennen gelernt"; sections/netzgeraet_1.md "die aktuell fließenden Stromstärke", "zuviel"; sections/batterien_und_akkus.md "Kurzschlusstrom"; sections/akku.md "geschalten", "belasten.Beschrieben" (space missing), "Zellen/ Akkus", comment "Endladestrom"; sections/gleichrichter_2.md "Um so größer", "des Kondensator", "Wir setzten"; sections/restwelligkeit.md "In der Folgenden Frage", "muss Frequenz als auch"; sections/spannungswandler.md "Step-UP", "Step-DOWN"; sections/brueckengleichrichter.md "dass der dieser"; slides/vollweggleichrichter.md ident "Vollwegleichrichter".
