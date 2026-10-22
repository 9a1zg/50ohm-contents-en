# nea_antennen_uebertragungsleitungen_3 — translation report

Chapter "Antennen und Übertragungsleitungen (3/4)" (Antennas and
transmission lines, part 3): 17 sections, each with its slides, and 7
solutions. 41 files:

- `contents/sections/` and `contents/slides/`: `uebertragungsleitungen.md`,
  `uebertragungsleitungen_2.md`, `uebertragungsleitungen_3.md`,
  `wellenwiderstand.md`, `koaxsteckverbinder.md`, `steckverbinder_pl.md`,
  `steckverbinder_n.md`, `steckverbinder_bnc.md`, `steckverbinder_sma.md`,
  `kabeldaempfung_1.md`, `kabeldaempfung_2.md`, `skineffekt.md`, `swr.md`,
  `swr_2.md`, `swr_3.md`, `swr_meter_1.md`, `swr_meter_2.md`.
- `contents/solutions/`: `AG402.md`–`AG405.md`, `AI403.md`, `EG307.md`,
  `EG308.md`.

`revizija-guard.py --brojevi`: 41 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comments (uebertragungsleitungen,
uebertragungsleitungen_2, swr), which stay. Line counts, trailing spaces
(uebertragungsleitungen_2, koaxsteckverbinder, steckverbinder_n, swr, swr_2,
swr_meter_2, slides swr_3 and swr_meter_2, AG404), the double space in the
caption of picture 670 and the presence or absence of a final newline are as
in the German. Decimal commas became points.

Embedded questions looked up in English and the prose aligned with them:
NG201–NG208, NG301–NG303, NF101, NI201–NI203, EG301–EG316, EG401–EG403,
EI401–EI405, AG301–AG312, AG314, AG317–AG319, AG402–AG405, AI401–AI403
(EG301 "roughly constant in the RF range"; EG302 "unwanted radiation"; EG303
"N connector", "voltage rating"; EG304 "unbalanced", "two conductors are
shaped differently"; EG305 "open-wire feeder", "lower loss and a high voltage
rating"; EG306 "coupling into the mains supply"; NG206 "connector series are
best suited"; NG207 "losses increase with increasing length and frequency";
AG301 "screened"; AG302 "PTFE (Teflon)"; AG303 "characteristic RF
properties", "bending radius", "return loss"; AG304 "the resistance
terminating it"; AG305 "spacing between the parallel conductors"; AG311 "twin
feeder"; AG312 "common-mode component", "in antiphase"; AG314 "lower than in
free space"; AG317 "physical length"; AG318 "skin effect"; AI401 "two
directional couplers inserted in the line and operated in opposite
directions"; EG403 "delivered"; AG403 "dummy load", "antenna feeder").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

18 rows: *Stecker / Kupplung / Buchse / Einbaustecker (Koaxialsteckverbinder)*;
*Steckverbinder / Koaxialsteckverbinder / Stecker (als Typbezeichnung)*;
*Mittelstift / Kontaktöffnung / Außengehäuse*; *Winkeladapter /
Reverse-SMA-Steckverbinder / „Geschirmter Bananenstecker"*; *Schutzmantel /
Mantel / Kunststoffummantelung / Drahtgeflecht / Folie / Abschirmfolie*;
*Induktivitätsbelag / Kapazitätsbelag*; *Mittenabstand*;
*Querschnittsaufbau*; *Gegentaktströme / Gleichtaktströme*;
*Hochfrequenzeigenschaften / Biegeradius*; *Aufschäumung / geschäumt /
nicht-geschäumtes Polyethylen*; *geometrische ("mechanische") Länge*;
*Hin-Richtung / Rück-Richtung / Hinweg / Rückweg*; *Leitungsdämpfung /
verlustbehaftete Leitung*; *Stehwellenmessgerät, kurz SWR-Meter*;
*einschleifen (SWR-Meter)*; *Koppelleitung / kapazitive / induktive
Kopplung*; *„Skineffekt" vom englischen Wort „skin" für „Haut"*.

## Added to `DECISIONS.md`

1 entry (Course text): coaxial connectors — *Stecker* → plug, *Kupplung* →
socket, *Buchse* (built in) → panel socket, *Einbaustecker* → panel plug, as
the course defines them in koaxsteckverbinder; a bare *Buchse* with no
contrast stays *socket*; not *jack*; *Stecker* naming a connector type →
*connector* (EG303). The connector chapters that follow keep this.

## Judgement calls

- koaxsteckverbinder: *den männlichen Stecker und die weibliche Kupplung* → "the male plug and the female socket"; indepth *Buchse* / *Einbaustecker* → "*panel socket*" / "*panel plug*"; slides "Special form *panel socket*: socket built into equipment" (DECISIONS.md). Captions *PL-Einbaubuchse*, *N-Einbaubuchse* → "PL panel socket", "N panel socket"; *N-Buchse und N-Stecker* (uebertragungsleitungen_2) and *in eine N-Buchse* (steckverbinder_n) → "N socket".
- koaxsteckverbinder: *Löten oder Crimpen (Verpressen)* → "soldering or crimping": the bracket is the German word for the English loanword (bracket rule); *(Abschirmgeflecht, -folie)* → "(braided screen, screening foil)"; *Außengehäuse* → "outer body".
- uebertragungsleitungen_2 slides: *N-Stecker / BNC-Stecker / SMA-Stecker / UHF/PL-Stecker* in the list of types → "N connector" etc., as EG303; *Besonders geeignet ist der N-Stecker* → "The N connector is particularly suitable". slides/kabeldaempfung_1 *Auch Stecker können das Signal dämpfen* → "Connectors can also attenuate the signal", as the section's *Steckverbinder*.
- steckverbinder_sma: *der Mittelstift umgedreht (reverse) ist* → "the centre pin is reversed" (bracket rule); *Reverse-SMA* → "reverse SMA", not the trade term "RP-SMA", which the German does not use; *WLAN-Bereich* → "the Wi-Fi world" (glossary); *Für hohe und höchste Frequenzen sind N- und SMA-Steckverbindungs-Systeme am besten geeignet* → "The N and SMA connector series are best suited to high and the highest frequencies" (NG206).
- steckverbinder_pl slide note *"Geschirmter Bananenstecker"* (a nickname of the PL connector) → '"Screened banana plug"', kept literal; *für die gesamte Kurzwelle* → "for the whole of the HF range" (KW → HF); `$\qty{2}{\meter}$-Band` → `$\qty{2}{\meter}$ band`.
- steckverbinder_bnc: *um ca. 90° gedreht* → "turned through approx. 90°"; *Bajonett-Verschluss* → "bayonet coupling", *Schraubverbindung* → "screw coupling" (glossary §14).
- uebertragungsleitungen: *Schutzmantel* → "protective sheath"; *Kabeldämpfung* → "*cable loss*", plain *Dämpfung* → "attenuation" (glossary §9, NG207); *von hochfrequenten Schwingungen* → "of radio-frequency oscillations"; slide note *Umgangssprachlich: "Koaxkabel"* → 'In everyday speech: "coax"'.
- uebertragungsleitungen_2: *Paralleldraht-Speiseleitung (Oft auch Hühnerleiter genannt …)* → "open-wire feeder (often also called ladder line …)" (EG305, glossary §9); *Mantelwellen* → "*common-mode currents*", *Mantelwellensperre* → "common-mode choke" (glossary); *Einkopplungen erfahren* (slide) → "can have RF coupled into them", *Und Leistung zur Antenne geht verloren* → "And power intended for the antenna is lost".
- uebertragungsleitungen_3: *Hühnerleiter, auch als Zweidrahtleitung bezeichnet* → "Ladder line, also called twin feeder"; *Gegentaktströme / Gleichtaktströme* → "*differential-mode currents* / *common-mode currents*" (glossary §9, AG312); *Rückflussdämpfung gibt an, wieviele Reflexionen vorhanden sind* → "states how much reflection there is"; *Teflon (PTFE)* kept in the German order; *nicht-geschäumtes Polyethylen* → "non-foamed polyethylene"; *Verkürzungsfaktor* of the cable → "velocity factor" throughout (DECISIONS.md); *auf welche Länge ein Kabel mechanisch gekürzt werden muss* → "the length to which a cable must be physically cut".
- wellenwiderstand: *Induktivitäts- / Kapazitätsbelag* → "inductance / capacitance per unit length"; *Mittenabstand* → "centre-to-centre spacing"; *relative Dielektrizitätszahl* → "relative permittivity" (glossary §4); table cells "Property / Value / Impedance / Frequency range / …" with the `X:` and `l:` markers unchanged; *die genau denselben Widerstand aufweist* → "whose resistance is exactly the same as the characteristic impedance" (AG304 "the resistance terminating it"); *dann spricht man von Anpassung* → "the line is said to be matched"; slide *für Luft* → "for air".
- kabeldaempfung_1: *Leistungsfaktor* → "power ratio" (glossary §14, not *power factor*), also in the table header and caption; *Dreisatz* → "rule of three" (glossary); *Lösung:* under *Lösungsweg* → "Working:" (glossary); *im Anhang der Formelsammlung* → "in the appendix to the formula sheet"; slide note *ggf. hier zoomen* → "zoom in here if necessary".
- kabeldaempfung_2: *Kunststoffummantelungen* → "plastic sheaths"; *dämpfungsarm* → "have particularly low loss".
- skineffekt: *Diesen Effekt nennen wir "Skineffekt" vom englischen Wort "skin" für "Haut"* → 'We call this effect the "skin effect".' — the gloss only translates the English word back (bracket rule); the indepth box and the slide note otherwise complete.
- swr: *Speise- oder Fußpunktwiderstand* → "the feed-point impedance" (one English term, glossary §9/§14); *Meist wird die vom englischen Begriff "standing wave ratio" abgeleitete Abkürzung SWR verwendet* → "usually abbreviated to SWR", slide *Abkürzung SWR vom englischen "standing wave ratio"* → "Abbreviated to SWR"; *Stehwellenmessgerät, kurz SWR-Meter genannt* → "an *SWR meter*" (bracket rule: English has one name); *Man sagt auch: "Das SWR-Meter wird zwischen Transceiver und Antenne eingeschleift"* → 'This is also described as "inserting the SWR meter in the line between transceiver and antenna"' (NI202, AI401 "inserted in the line"); *siehe [ref:n_swr_display]* kept without "Figure", as the German; caption *Prinzipbild …* → "Schematic of an SWR meter between transceiver  and antenna"; *Kreuzzeiger* → "cross-needle display".
- swr_2: *als Formelsymbol $s$* → "with the symbol $s$"; *Verlustwiderstand* → "loss resistance" (glossary §4); *abgegeben* → "delivered" (EG403).
- swr_3: *Lastwiderstand* → "load resistance" (AI403 "load resistor" where the component is meant); `\text{für }` → `\text{for }` (running word in `\text{}`); *Speisewiderstand* → "feed-point impedance" (glossary); *der Widerstand eines Faltdipols knapp 240–300 Ω* → "the impedance of a folded dipole is roughly 240 Ω to 300 Ω" (and in the slides "just under 300 Ω", *$R_2$ … Widerstand Faltdipol* → "impedance of the folded dipole"), as AG405's solution calls it the *Speisewiderstand*; *Hin- / Rück-Richtung* → "on the way there / on the way back" (glossary); *abgeklemmte Antenne* → "disconnected antenna" (AG404); *Ein trügerischer Effekt* → "A deceptive effect".
- swr_meter_1: *Stehwellenmessgerät* → "SWR meter", *SWR-Messbrücke* → "SWR bridge" (glossary §11, EI403); *einschleifen* → "insert in the line"; *um Veränderungen der Speiseleitung auszuschließen* → "to rule out changes caused by the feeder".
- swr_meter_2: *Richtkoppler* → "directional coupler", *Koppelleitung* → "coupling line", *Abschlusswiderstand* → "terminating resistor" (glossary §11), *Messwerke eines Kreuzzeigerinstruments* → "meter movements of a cross-needle meter", *A/D-Umsetzer* → "A/D converter", *einstellbare Widerstände* → "variable resistors"; *Man misst hierzu die … Ausgangsspannungen zweier in die Leitung eingeschleifter Richtkoppler, die in gegensätzlicher Richtung betrieben werden* → "the output voltages of two directional couplers inserted in the line and operated in opposite directions are measured" (AI401's wording); slide *Gilt bei Last mit rein wirkwiderstandlicher Komponente* → "Applies to a load with a purely resistive component".
- Solutions: *künstliche 50 Ω-Antenne* (AG403) → "50 Ω dummy load" (AG403, bracket rule of DECISIONS.md); *Antennenleitung* → "antenna feeder"; *Faktor von 10* (AG404) → "a power ratio of 10"; EG308 *im Abschnitt Pegel* → "in the section on levels (*Pegel*)" (glossary §14, formula-sheet section names); *Einfache dB Überlegung* → "Simple dB reasoning"; the symbol $P_\mathrm{Ende}$ unchanged; a full stop added after the displayed sum in AG404, where the English sentence ends there.

## Suspected errors in the German original

- sections/wellenwiderstand.md — table a_rg58: the velocity of propagation is given as $\qty{0,66}{\percent}$; RG-58 has a velocity factor of 0.66, i.e. 66 %. Also "Ausbreitungsgeschwingkeit" (*Ausbreitungsgeschwindigkeit*). Kept as $\qty{0.66}{\percent}$.
- sections/swr_meter_2.md — pictures 1109 (left to right) and 1110 (right to left) both carry the ident `a_richtkoppler_rechts_links`, and both paragraphs refer to it, so the second reference cannot point at the right-to-left drawing. Kept.
- slides/skineffekt.md — the skin-effect drawing (picture 633) carries the ident `a_mantelwellen` ("common-mode currents"); probably a copied ident. Kept.
- slides/uebertragungsleitungen_3.md — "Mechanische Eigenschaften wie Biegeradius und Rückflussdämpfung": return loss is not a mechanical property; the section says it depends on the load and is therefore not a property of the cable. Translated as written.
- slides/swr_2.md — "Stehwellenverhältnis: Vorlaufende zu rücklaufender Energie": the SWR is not the ratio of forward to reflected energy (an SWR of 3 means a power ratio of 4, as the next bullet shows). Translated as written.
- sections/swr.md (indepth) — "sind noch die Werte 2 und 3 rechts markant": *rechts* has no reference in the text (presumably the meter scale of a figure). Translated as "on the right".
- sections/swr_3.md — "der Widerstand eines Faltdipols knapp $\qtyrange{240}{300}{\ohm}$": *knapp* ("just under") does not fit a range; the slide says "knapp 300 Ω". Rendered "roughly" in the section and "just under 300 Ω" on the slide.
- slides/swr_3.md (AG404) — "$P_R = \qty{-10}{\dB} \cdot P_V$" multiplies a level in dB by a power; what is meant is $P_R = 10^{-10/10} \cdot P_V$. Kept.
- Typos with no effect on the English: sections/uebertragungsleitungen.md "Eine weiteres" (*Ein weiteres*); sections/uebertragungsleitungen_2.md "Querschittsaufbau" (*Querschnittsaufbau*), "bei bestimmungsgemäßen Betrieb" (*bestimmungsgemäßem*); sections/koaxsteckverbinder.md "drauf geachtet" (*darauf*); sections/skineffekt.md "Feldfrei" (*feldfrei*); sections/swr_2.md "Leisung" (*Leistung*), "Reflektion" (*Reflexion*, also in swr_3); sections/swr_meter_2.md "Zu nächst" (*Zunächst*), "die die Ausgangsspannungen" (doubled), "gemessern" (*gemessen*).

