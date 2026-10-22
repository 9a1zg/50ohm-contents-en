# nea_antennen_uebertragungsleitungen_2 — translation report

Chapter "Antennen und Übertragungsleitungen (2/4)" (Antennas and
transmission lines, part 2): 17 sections, each with its slides, and 15
solutions. 49 files:

- `contents/sections/` and `contents/slides/`: `fusspunktimpedanz_1.md`,
  `fusspunktimpedanz_2.md`, `elektrische_verlaengerung_verkuerzung.md`,
  `nvis.md`, `yagi_uda_2.md`, `yagi_uda_3.md`, `parabolspiegel_1.md`,
  `parbolspiegel_2.md`, `offsetspiegel.md`, `vor_rueck_verhaeltnis.md`,
  `halbwertsbreite.md`, `strom_spannung_speisung_1.md`,
  `strom_spannung_speisung_2.md`, `traps.md`, `antennengewinn.md`,
  `standortwahl.md`, `einbau_kfz.md`.
- `contents/solutions/`: `AG108.md`, `AG114.md`–`AG116.md`,
  `AG203.md`–`AG206.md`, `AG215.md`–`AG218.md`, `AG221.md`, `EG220.md`,
  `EG221.md`.

`revizija-guard.py --brojevi`: 49 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comments (antennengewinn,
standortwahl), which stay. Line counts, trailing spaces, the double spaces
(einbau_kfz), the leading blank line of einbau_kfz and the presence or absence
of a final newline are as in the German. Decimal commas became points, also
`0{,}1` → `0{.}1` (AG216), as earlier units wrote `0{.}707`.

Embedded questions looked up in English and the prose aligned with them:
AG106–AG116, AG125–AG127, AG203–AG222, AG224–AG229, EG111–EG114,
EG203–EG212, EG218, EG220, EG221, EG223, EJ110, NK307–NK310 (EG207/EG208
"height at which it is installed", EG209–EG211 feed-point / input impedance
ranges; EG203–EG206 "current-fed", "voltage-fed", "antinode", "node";
AG203–AG206 "applies when the dipole is fed at 28 MHz"; AG207/AG208
"series-/parallel-resonant"; AG209 "essentially as a resistance"; AG106,
AG107 "electrical lengthening / shortening of the radiator"; AG108 "each
leg"; AG109–AG116 "trap dipole", "traps for the operating frequency",
"three-band dipole", "dual-band antenna"; AG125/AG224 NVIS, "skip zone";
AG126 "axis of radiation"; AG127 "offset dish", "feed antenna", "radiation
path"; AG212/AG222 "radiator", "beamwidth"; AG213–AG218 "front-to-back
ratio", "in the opposite direction to the beam"; AG219–AG221 "half-power
beamwidth (beam angle)"; EG113/EG114 "paraboloidal reflector", "parabolic
dish antenna"; EG112, EG223, EJ110 antenna location; NK307–NK310 "road
approval", "Arcing and vehicle fire", "middle of the metal roof").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

17 rows: *Aufbauhöhe*; *Speiseimpedanz / Speisewiderstand (Kurstext)*;
*stromgespeist / spannungsgespeist / Strom- und Spannungsspeisung*;
*Strombauch / Strombäuche (gezählt)*; *Anregung / Anregungsfrequenz
(Dipol)*; *mechanische / elektrische Länge*; *Verkürzungskondensator*;
*Bauform (Antenne)*; *Sperrkreis-Dipol, der auch als Trap-Dipol bezeichnet
wird / Trap (englisch für „Falle") / wirkt als Sperrkreis*; *Raumwelle mit
nahezu vertikalem Einfallswinkel (NVIS, "zu Deutsch")*; *Strahlenoptik /
Beugungseffekte / Schüssel*; *Strahlungsachse / Polarisationsebene*;
*Offsetspiegel (auch Offsetantenne genannt)*; *$\frac{Vor}{Rück}$*;
*Bodenverluste / Wechselwirkung mit dem Boden*; *Lichtbogen / Kabelbrand /
Fahrzeugbrand*; *Mittelkonsole / PKW / Gegenelement*.

## Added to `DECISIONS.md`

1 entry (Course text): words written as a quantity in a worked formula
($\frac{Vor}{Rück}$) are translated ($\frac{Front}{Back}$), as
$\textrm{Abw.}$ → "Dev."; the letter symbols derived from them ($P_V$,
$P_R$, $U_V$, $U_R$) stay, as in AG213/AG214 and the drawings.

## Judgement calls

- vor_rueck_verhaeltnis slides: $\frac{Vor}{Rück}$ → $\frac{Front}{Back}$ (DECISIONS.md); $P_V$, $P_R$, $P_S$, $g_D$, $g_d$, $U_V$, $U_R$, $U_D$, $P_{ERP}$ unchanged.
- *Speiseimpedanz*, *Speisewiderstand* and *Fußpunktimpedanz* → "feed-point impedance" throughout (glossary §9), also in strom_spannung_speisung_1, where the German argues from Ohm's law; there the bare *Widerstand* stays "resistance" ("the resulting resistance correspondingly low"), and *niederohmig / hochohmig* → "low-impedance / high-impedance" (EG204, EG205 "a low / high impedance").
- strom_spannung_speisung: *Strombauch / Spannungsbauch / Stromknoten / Spannungsknoten* → "current / voltage antinode / node" (EG203–EG205, glossary §9); the counted *Strombäuche* of strom_spannung_speisung_2 and AG203–AG206 likewise "current antinodes". *Anregung mit 28 MHz* → "fed at 28 MHz", *Anregungsfrequenz* → "operating frequency" (AG203–AG206, glossary §9 *Erregung*).
- traps: *der sogenannte Sperrkreis-Dipol, der auch als Trap-Dipol bezeichnet wird* → "the *trap dipole*", and *Trap (englisch für „Falle")* → "a *trap*": English has one name, and the gloss only translates the English word back (bracket rule). Where the German says what the circuit does at resonance (*wirkt als Sperrkreis*), "acts as a *rejector*" (glossary §5 *Sperrkreis*), in the section, slides and AG114, AG116, so that "the trap acts as a trap" is avoided; the caption of the generic frequency response *Parallelschwingkreis (Sperrkreis)* → "parallel tuned circuit (rejector)". *Verlängerungsspule* → "loading coil" (glossary §9).
- traps: *aus dem Abschnitt "Strom- und Spannungsspeisung II"* → "from the second section on current and voltage feeding", *im Abschnitt "Traps"* (strom_spannung_speisung_2) → "in the section on traps": section titles not yet translated, descriptive, as earlier units did for chapters.
- nvis: *von "NVIS" aus dem Englischen: Near Vertical Incidence Skywave. Oder zu Deutsch: Raumwelle mit nahezu vertikalem Einfallswinkel.* → '*"NVIS"*, for near vertical incidence skywave': the German rendering only translates the English expansion back (bracket rule), and "from the English" says nothing to an English reader. *Tote Zone* → "skip zone" (AG224); *flachere Abstrahlrichtung / flacher Abstrahlwinkel* → "lower angles / a low angle of radiation" (glossary, never "flat"); *Notfunkreferat des DARC* (link text) → "DARC emergency communications department (Notfunkreferat)" (glossary §14); *allen deutschen Amateurfunkklassen* → "all German licence classes".
- yagi_uda_2: *Strahlungsdiagramm (Richtdiagramm)* → "radiation pattern": both German words are one English term (glossary §9), so the bracket is dropped; *Hauptstrahlungsrichtung* → "direction of maximum radiation".
- fusspunktimpedanz_1: *die anliegende Spannung* (folded dipole) → "the applied voltage"; *Groundplane* alone → "ground plane", *Groundplane-Antenne* → "ground-plane antenna" (EG211, EG218); slide *Radiale um 45° nach unten abwinkeln ergibt zusätzliche Abstrahlung* → "Sloping the radials downwards at 45° gives additional radiation".
- fusspunktimpedanz_2: *besitzt … im Wesentlichen einen Wirkwiderstand* → "presents essentially a *resistance*" (AG209); *Wir erinnern uns:* → "Remember:"; slide *ab ca. 1‑λ Aufbauhöhe* → "from a height of about 1 λ above the ground".
- elektrische_verlaengerung_verkuerzung: *mit einer Länge von umgerechnet 0,625 λ* → "with a length of 0.625 λ" (*umgerechnet* only says that 5/8 has been converted); *Fusspunktspule* → "base loading coil" (glossary §9); *Verkürzungskondensator* → "shortening capacitor" (new row); slide *Die abweichende Speiseimpedanz* → "The departure from the expected feed-point impedance"; *bei idealer Erde* (caption) → "over perfect earth", as in unit 1.
- parabolspiegel_1: *Die sogenannten Mikrowellen* → "*Microwaves*, as they are called" (English *so-called* sounds sceptical); the German sentence that ends without a full stop before the indepth box is kept without one.
- parbolspiegel_2: *Erregerantenne* → "feed antenna" (AG225); *Hornstrahler* → "horn antenna", *Helixantennen* → "helical antennas", *Hohlleiter* → "waveguides"; *Außenwände* → "walls" (the wave runs inside the tube, so "outer walls" would mislead; *metallischen Außenwänden* → "metal walls"); slide placeholder *Bild eines Hornstrahlers folgt* → "Picture of a horn antenna to follow"; the `% TODO: Bild Helixantenne` comment unchanged.
- offsetspiegel: *Offsetspiegel (auch Offsetantenne genannt)* → "*offset dish* (also called an offset antenna)" (AG127); *Strahlengang* → "radiation path" (AG127).
- halbwertsbreite: *Öffnungswinkel oder Halbwertsbreite* → "*beamwidth* or *half-power beamwidth*" (glossary §9, AG221, AG222).
- antennengewinn: the German first sentence lacks its verb ("…, dass die Zusätze dBd und dBi, die … verwendet werden."); rendered with its evident meaning, "The chapter on decibels already touched on the suffixes dBd and dBi, which are used when antenna gains are stated" (listed below). *Zusätze* → "suffixes" (glossary §14).
- standortwahl: *so hoch und so weit entfernt wie möglich entfernt* → "as high and as far away as possible" (EG112; the doubled *entfernt* is listed below); slide *Hauptstrahlrichtung zeigt nicht auf das Gebäude und das der Nachbarn* → "does not point at the building or the neighbours' building".
- einbau_kfz: *Zulassung das Fahrzeugs* → "the road approval of the vehicle" (NK308, glossary §12); *Mobilfunkantenne / Mobilfunkanlage* → "mobile antenna / mobile installation" (glossary §13, not *mobile phone*); *Magnetfußantenne* → "magnetic-mount antenna"; *Gegengewicht / Gegenelement* → "counterpoise"; *PKW* → "car"; *im Kapitel Spannungsversorgung* → "in the chapter on power supplies"; *Stromkabel mit Sicherungshalter* → "Power cable with fuseholder"; the `%[class:N]` markers unchanged.
- Solutions: *Leistungsfaktor* (AG215) → "power ratio" (glossary §14, trap: not *power factor*); *entgegen der Hauptstrahlrichtung* → "in the opposite direction to the beam" (AG215, AG216); *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", *Tipp* → "Tip", *Rechnung* → "Calculation", as earlier units; AG218 *(es steckt ja eine Spannung darin!)* → "(they contain a voltage, after all!)".

## Suspected errors in the German original

- sections/antennengewinn.md — the first sentence has no main verb: "Im Kapitel Dezibel wurde schon angedeutet, dass die Zusätze $\unit{\dBd}$ und $\unit{\dBi}$, die bei der Angabe von Antennengewinnen verwendet werden." (the *dass* clause is never finished). Translated with its evident meaning.
- sections/strom_spannung_speisung_1.md (indepth) — "Aus diesem Grund ist ein mittengespeister Dipol nur bei ungeraden ganzzahligen Vielfachen der Grundfrequenz resonant": at even multiples the centre-fed dipole is resonant too, but parallel-resonant and of high impedance, as AG208 (embedded in strom_spannung_speisung_2) says; what the text means is that it is low-impedance (series-resonant) only at odd multiples. Translated as written.
- sections/fusspunktimpedanz_1.md — "ergibt sich … ein Speisewiderstand von genau 50 Ω" for radials sloping at 45°: the value is approximate (it depends on the slope, wire thickness and surroundings), and the same paragraph ends with the range 30–50 Ω. Translated as written ("exactly").
- sections/fusspunktimpedanz_1.md, sections/fusspunktimpedanz_2.md — caption "Fußpolimpedanz" for *Fußpunktimpedanz*. English "Feed-point impedance".
- sections/elektrische_verlaengerung_verkuerzung.md — caption of picture 650 writes `$\qty{5}{8}\lambda$`, i.e. the number 5 with the unit "8", for $\frac{5}{8}\lambda$; kept unchanged in the formula. Also "Eine von mehreren Möglichkeit" (*Möglichkeiten*), "Fusspunktspule" (*Fußpunktspule*).
- sections/strom_spannung_speisung_1.md and _2.md — the caption "Stromverteilungen bei verschiedenen Grundfrequenzen" (picture 1050): the figure shows one fundamental frequency and its multiples, not several fundamental frequencies. Translated as written. In _1 also "verschiedneen" (*verschiedenen*) and "die Strom und Spannungsverteilung" (*Strom- und*).
- sections/strom_spannung_speisung_2.md — "Freqeuenzen" (*Frequenzen*), "eine möglichkeit" (*Möglichkeit*).
- sections/standortwahl.md — "so hoch und so weit entfernt wie möglich entfernt": *entfernt* twice.
- sections/offsetspiegel.md, slides/offsetspiegel.md — "Stahlengang" for *Strahlengang* (once in each).
- sections/einbau_kfz.md — "die Zulassung das Fahrzeugs" (*des Fahrzeugs*).
- sections/nvis.md — "Weitere Informationen indest du" (*findest*); "Reflektion" for *Reflexion* (also in the slides).
- slides/strom_spannung_speisung_2.md — "Ungerade Frequenzen: zusätzliche Stromzufuhr" says little (odd multiples are meant, and nothing is "additional"); translated as written ("Odd frequencies: additional current feed").
- slides/vor_rueck_verhaeltnis.md (AG215, AG216) — the given gain is written $g_D$, but the formula uses $g_d$. Kept.
- Typos with no effect on the English: sections/yagi_uda_2.md "von dieser Antennen" (*diesen Antennen* / *dieser Antenne*), "kennen gelernt"; sections/parbolspiegel_2.md "Im Punkt vor dem Parabolspiegel wo" (comma); sections/vor_rueck_verhaeltnis.md "wieviel" (*wie viel*); sections/einbau_kfz.md "Stromfluß" (*Stromfluss*); sections/nvis.md "aufgehangen" (*aufgehängt*, twice).
