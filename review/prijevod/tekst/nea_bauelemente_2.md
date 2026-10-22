# nea_bauelemente_2 — translation report

Chapter "Bauelemente (2/2)" (Components, part 2): 6 sections, each with its
slides, and 30 solutions. 42 files:

- `contents/sections/` and `contents/slides/`: `diode_1.md`,
  `halbleiter_2.md`, `diode_2.md`, `transistor_1.md`, `transistor_2.md`,
  `integrierte_schaltkreise.md`.
- `contents/solutions/`: `AB104.md`–`AB109.md`, `AC401.md`–`AC408.md`,
  `AC501.md`, `AC503.md`–`AC505.md`, `AC515.md`–`AC523.md`,
  `AF425.md`–`AF427.md`.

`revizija-guard.py --brojevi`: 42 files checked, *struktura netaknuta*.
German-word grep: no hits outside `%` comments (left in German, as markup),
idents and file names, the place name *Würzburg*, and the German names kept
on purpose (*Kleiner Radiomann*, the mnemonic *Pfeil Nach Platte*).

Embedded questions looked up in English and the prose aligned with them:
EC501–EC522, EC601–EC615, AB104–AB109, AC401–AC408, AC501–AC524,
AC601–AC604, AF425–AF427.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

34 rows: *Energiebandlücke / Bandlückenenergie*, *Valenzband / Leitungsband
/ Valenzbandkante*, *Element- / Verbindungshalbleiter*, *dotierbar / n- /
p-Dotierung*, *Elektronenfehlstelle / Defektelektron* (electron vacancy),
*Diffusionsstrom / Feldstrom* (drift current), *Raumladungszone*,
*Sperrsättigungsstrom / Sättigungsstrom*, *Temperaturspannung*,
*Sperrdurchbruch / Zener-Spannung / Kathodenstrich*,
*Metall-Halbleiter-Übergang*, the case of *pn / npn / n-Kanal*,
*antiparallele Dioden*, *geklippt*, *Fotowiderstand*, *nicht-sperrender
Kontakt*, *galvanisch getrennt*, *Masseschleife / Netzbrummen* (earth loop,
mains hum), *gegen Masse / Massepotential* (chassis), *Ausgleichsströme*,
*spannungsgesteuerte Stromquelle*, *Stromverstärkung B /
Stromverstärkungsfaktor*, *Leckstrom*, *Schalttransistor / Ansteuerung /
Steuerspannung*, *Serien-Gegenkopplung*, *Regelbetrieb*, *Relais hat
angezogen*, *Kanalwiderstand / Kanalstrom*, *Bulk-Schicht*, the FET
electrode names with their German glosses, *Wehr / Steuerkanal /
Steuerklappe*, *Kleiner Radiomann*, *Pfeil Nach Platte*, *HF-Abblockung /
Betriebsspannungsleitung*.

## Added to `DECISIONS.md`

None. The mnemonic *Pfeil Nach Platte* follows the existing mnemonics
entry; the dropped "(engl. …)" / "dt. …" glosses follow the bracket rule.

## Judgement calls

- All files: the case of *pn-Diode*, *npn / pnp*, *n-Kanal / p-Kanal* follows the German in each place ("pn diode", "npn transistor", "n-channel FET"; "NPN" where the German writes NPN), as the glossary does for *n-dotiert*; the bank's English has N-channel / NPN because its German does.
- diode_1, diode_2, halbleiter_2: *Schwellspannung / Schwellenspannung* → threshold voltage, *Durchlassspannung* → forward voltage, as EC503 / EC504 / AC403; *Verarmungszone* → depletion region, *Sperrschicht* → depletion layer, *Raumladungszone* → space-charge region, each as the German writes it (glossary §4, AB108, AB109).
- diode_1 slides: *Z-Diode* → "Zener diode" throughout; the note "aber Z-Diode blieb als Name" → "but the name Zener diode has stuck"; *Eine spezielle Bauform haben wir schon als LED kennengelernt* → "We have already met one special type of diode: the LED".
- halbleiter_2: *Feldstrom* → "drift current", the English term for the current the junction field drives; *Elektronenfehlstelle* and *Defektelektron* → "electron vacancy" (transistor_1, transistor_2, AB107), not "defect electron".
- diode_2: *antiparallele Dioden* → "diodes in inverse parallel" (glossary §14); *nicht-sperrende Kontakte* → "non-rectifying contacts"; *Masseschleifen* → "earth loops"; *in einem Gehäuse* (optocoupler) → "in one package".
- transistor_1: indepth *im Englischen auch BJT: Bipolar Junction Transistor, dt. bipolarer Sperrschicht-Transistor* → "also called a BJT, short for bipolar junction transistor"; *MOSFET steht für metal-oxide-semiconductor field effect transistor, dt. Metall-Oxid-…* → the English expansion only (bracket rule: the German gloss only translates the English back).
- transistor_1: *Elektronenröhre* → "thermionic valve" / "valve" (glossary §4); *in den zwanziger Jahren* → "from the twenties onwards", *in den 50er Jahren* → "in the '50s" (the guard keeps the numbers as written).
- transistor_1: *aus dem "Kleinen Radiomann" des Kosmos-Verlags* → "from the "Kleiner Radiomann" (little radio man) kit published by Kosmos": the name stays German, *kit* says what it is.
- transistor_1 slides: *Merksatz für PNP → Pfeil Nach Platte* kept in German with "(arrow towards the plate)", as the country-prefix mnemonics and memory rhymes (DECISIONS.md).
- transistor_2: the FET electrode list drops the glosses *(engl. source)*, *(engl. drain)*, *(englisch für Gatter)*: "*Source*: this is the "source" of the charge carriers", "*Drain*: this is where the charge carriers in the channel flow away ("drain")"; the slides likewise.
- transistor_2, AC519, AC522, integrierte_schaltkreise: *Masse / Massepotential / gegen Masse* → chassis / chassis potential / to chassis (glossary §4, EC612).
- transistor_2: *Spannungsteiler* → potential divider (glossary §5), *Basisspannungsteiler* → base potential divider (AC516), *Querstrom* → divider current, *Querwiderstand* → lower divider resistor (AC517, AC518); *zugedreht* → "turned down".
- integrierte_schaltkreise: *Für Hochfrequenz besitzt die Drossel einen hohen Widerstand* → "a high impedance" (it is a reactance); *Kurzwellensender* → "HF transmitter"; *130nm* → "130 nm"; slides *Integrated Circuit (IC): Integrierte Schaltungen* → "*Integrated circuit (IC)*", the German gloss dropped.
- integrierte_schaltkreise slides: *Anschluss 2 und 4 liegen auf Masse gegenüber U_CC* → "Terminals 2 and 4 are at chassis potential with respect to $U_{\textrm{CC}}$".
- AC402: *physikalische Stromrichtung von - nach +* → "electron flow, from - to +" (glossary §14).
- Headings *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", *Ansatz* → "Approach", as in earlier units.

## Suspected errors in the German original

- slides/diode_2.md (photodiode) — "Elektronen bewegen sich zum p-Gebiet, Löcher zum n-Gebiet": the field of the space-charge region drives electrons to the n-side and holes to the p-side, which is why the photocurrent flows against the normal diode current, as sections/diode_2.md says. Translated as written.
- sections/transistor_2.md — "Beim Sperrschicht-FET trägt das Gate den Kanal": evidently "den Pfeil" (in the JFET symbol the arrow is on the gate, while in the insulated-gate FET it sits between channel and bulk). Translated as written ("the gate carries the channel").
- slides/transistor_2.md — "*selbstleitend*/*selbstsperrend*: Gate durchgehend/gestrichelt": it is the channel line between source and drain that is continuous or broken, as the section says. Translated as written.
- sections/transistor_2.md — "die sogenannte technische Stromrichtung ist entgegen der Ladungsträger-Flussrichtung definiert": true for electrons (n-channel), not for holes in a p-channel FET, which the same paragraph has just introduced.
- solutions/AC517.md — the intermediate results are named $U_1$, $I_1$, but the final formula divides $U_{R_1}$ by $I_{R_1}$ (AC518 keeps $U_1 / I_1$). Translated as written.
- Typos with no effect on the English: sections/diode_1.md "Kennline" (captions 861, 862), "Kennlinen" (858), "verschienden"; sections/halbleiter_2.md "Zonnen", "Löcher bewegen sind", "ein Gebiet …, die man"; sections/transistor_1.md "Spannungsabhängig" (for *-abhängigkeit*), "beginnt, Wasser zu fließen"; sections/transistor_2.md "augeschaltenen", "eingesschalteten" (captions 1071, 1072), "Es empfiehl sich" (also AC504), "sowohl Elektronen also auch", "im einen unbelasteten", "in sofern", "Wenn R_1 … nicht von Strom durchflossen" (verb missing); slides/diode_1.md "Sperichtung" (caption 549); slides/transistor_1.md "Je Art des bipolaren Transistor"; slides/transistor_2.md "p-dotieren", "n-dotieren", "Basistrom", "Sperichtung", "Basis ist über $R_1$ ist"; slides/integrierte_schaltkreise.md "ohmschmer".
