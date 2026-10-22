# nea_strom_spannung_widerstand_leistung_energie_2 — translation report

Chapter "Strom, Spannung, Widerstand, Leistung, Energie (2/3)" (Current,
voltage, resistance, power, energy, part 2): 13 sections, each with its
slides, and 7 solutions. 33 files:

- `contents/sections/` and `contents/slides/`: `spitze_effektiv_wert.md`,
  `oszilloskop_1.md`, `oszilloskop_2.md`, `ohmsches_gesetz.md`,
  `widerstandsfarbcode.md`, `widerstand_smd.md`, `leiterwiderstand.md`,
  `widerstand_materialien.md`, `widerstand_toleranz.md`,
  `widerstand_ntc_ptc.md`, `halbleiter.md`, `leistung.md`,
  `wechselstrom_leistung.md`.
- `contents/solutions/`: `AB101.md`, `AB102.md`, `AB301.md`, `AI105.md`,
  `AI305.md`, `AI306.md`, `NB505.md`.

`revizija-guard.py --brojevi`: 33 files checked, *struktura netaknuta*.
German-word grep: no hits outside `%` comments (kept, as the brief says),
idents and the formula subscripts (`P_\text{Wechselstrom}`,
`\hat{U}_\mathrm{gemessen}`, `A_\text{Dr}`), which stay German.

Embedded questions looked up in English and the prose aligned with them:
EB401–EB411, EI301–EI304, AI301–AI306, NA203, NB501–NB505, NC102–NC110,
EC101–EC117, AB101–AB103, NC401–NC404, NB703, NA204, NA210, NA211,
NB601–NB606, AB301, AI105.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

24 rows: *Spitzen- oder Scheitelwert*, *Spitzen-/Effektiv-/Spitzen-Spitzen-
Spannung*, *bedrahtet*, *Kästchen* (oscilloscope), *Gitter*, *AUTO-/SINGLE-
Taste / X-Position*, *Triggerspannung / Triggereinrichtung*, *Prüfspitze /
Krokodilklemme*, *Masseverbindung / Bezugsmasse* (probe), *Teilverhältnis*,
*Typschild*, *Wickelwiderstand / Wickelkörper*, *Überlastbarkeit*, *Manganin
/ Konstantan*, *aufgedampft / Träger*, *Kaltleiter / Heißleiter* as a
material property, *NTC (englisch …)*, *Einschaltstrombegrenzung*,
*Thermoelement*, *Platine*, *Bauform*, *Merkhilfe*, the *Vertiefung:* label,
*Kurze Wiederholung*.

## Added to `DECISIONS.md`

Nothing: every choice here is a single term (glossary) or follows an
existing rule (bracket rule, units after a number, word subscripts).

## Judgement calls

- spitze_effektiv_wert: *Spitzen- oder Scheitelwert* → "peak (or crest) value" (English has both names); *Spannungsfestigkeit* → "voltage rating" (glossary), *bedrahtete Elektrolytkondensatoren* → "leaded electrolytic capacitors"; caption "16 Volt und 25 Volt" → "16 V and 25 V" (symbol after a number); *einen ohmschen Widerstand erwärmen* → "heat an ohmic resistor" (the thing heated, not the quantity).
- spitze_effektiv_wert slides: *Lösungsweg auf nächster Seite* → "Solution on the next page", headings "### Solution", as in earlier units; *Ergebnis von vorher ×2* → "Previous result ×2".
- oszilloskop_1: *Kästchen* → "square", *Skalenteil / Division* → "division" (EI301); "50 Nanosekunden … 500 Millivolt" → "50 ns … 500 mV"; *X-Position* (knob label) → "X position"; *stehendes Bild* → "stationary picture" (AI302); *Gitter* → "grid".
- oszilloskop_2: the gloss *(engl. trigger = „auslösen")* dropped (bracket rule: it only translates the English word back), *(engl. jitter)* → "(jitter)", which names the effect; *Masseverbindung* of a probe → "earth connection", slides *Bezugsmasse* → "Reference (earth) connection" — the probe's clip is tied to the oscilloscope's earthed screen, and the house style has *earth*, never *ground*; *Innenwiderstand* of the scope → "internal resistance" (glossary), although English data sheets say "input resistance".
- oszilloskop_2 slides: *gegeben / gesucht* → "given / required", as AI104; *PEP-Leistung* (solutions AI305, AI306) → "the PEP".
- ohmsches_gesetz: *Proportionalitätsfaktor* → "constant of proportionality" (glossary §3); *Verbraucher … üben einen Widerstand aus* → "loads … present a resistance"; *Formelsammlung* → "formula sheet"; the `%` comments (including the disabled photo) left in German.
- widerstandsfarbcode: table header and colour names translated (*Grau* → "Grey", British); table caption *Widerstandsfarbcodes Tabelle* → "Resistor colour code table"; *Vertiefung:* → "*In depth:*"; the German's unclosed bracket "(siehe Tabelle …," closed in English.
- widerstand_smd: *(deutsch: oberflächenmontiertes Bauelement)* dropped — it translates the English name back into German; *ganz ohne Durchkontaktierung* → "with no through-holes at all" (for a component's leads, not the PCB *via*); the doubled unit "$\qty{11000}{\ohm}$ Ohm" written once.
- leiterwiderstand: *Kaltleiter / Heißleiter* as properties of materials ("Die meisten Metalle sind Kaltleiter") → "PTC conductors / NTC conductors", after "In Class E we already met the concept of PTC and NTC thermistors": calling a metal a *PTC thermistor* would make it a component. New glossary row.
- leiterwiderstand slides: the list says *Zink* where the section's table says *Zinn* (same value 0.11); each translated as written, "Zinc" and "Tin" (see errors below).
- widerstand_materialien: *Künstliche Antennen, also Dummyloads* → "dummy loads" (bracket rule, as DECISIONS.md *künstliche Antenne (Dummy Load)*); *ungewendelte Metalloxidschichtwiderstände* → "metal-oxide resistors without a spiral cut" (EC107); *weitgehend induktionsarm* → "has, for the most part, low inductance"; *weniger induktionsarm* → "their inductance is not as low"; *Wickelwiderstände* → "wound resistors"; *Wickelkörper* → "former".
- widerstand_ntc_ptc: the German names the components *Kaltleiter / Heißleiter* and then says they "are also called NTC (englisch Negative Temperature Coefficient) and PTC"; in English the names are already PTC / NTC thermistor, so the sentence becomes "*NTC* stands for negative temperature coefficient and *PTC* for positive temperature coefficient" (it keeps the expansion, which is information). Slides *Englisch: Negative Temperature Coefficient Thermistor* → "Full name: negative temperature coefficient thermistor"; captions *NTC-/PTC-Widerstand* → "NTC / PTC thermistor".
- halbleiter: the memory aid "add the initial letters A and K" → "add the letters A and K (the usual abbreviation for the cathode)" — *K* is the German initial and is also the usual symbol in English diagrams, but not the English initial; *LED (englisch "light-emitting diode")* → "LED" with the gloss dropped; *Bauformen* → "package styles".
- leistung: *Typschild* → "rating plate"; *LED-Leuchtmittel* → "LED lamp".
- wechselstrom_leistung, AI105: *Thermoumformer* → "thermocouple converter" (glossary §11, AI105); *Thermoelement* → "thermocouple".
- NB505: the German answer "$\qty{40,000}{\ohm}$" (decimal comma) → `\qty{40.000}{\ohm}`, matching the English answer "40.000 Ω".

## Suspected errors in the German original

- sections/leiterwiderstand.md — table *Zinn* 0,11, slides/leiterwiderstand.md list *Zink* 0,11 for the same value. 0.11 Ω·mm²/m is tin; zinc is about 0.06. The slide should say *Zinn*. Translated as written ("Tin", "Zinc").
- solutions/AB101.md and slides/leiterwiderstand.md — the same calculation (ρ = 0.018, l = 1.8 m, d = 0.2 mm) gives 1.03 Ω in the solution and "≈ 1.02 Ω" on the slide; 0.018 · 1.8 / 0.0314 = 1.03. The exam's correct answer, 1.02 Ω, corresponds to ρ ≈ 0.0178. The solution also writes ρ as "0,018 mm²/m", without the Ω.
- solutions/AB102.md — stops after stating the cross-section; the value of $l$ (41.7 m) is never calculated.
- sections/wechselstrom_leistung.md and solutions/AI105.md — "Die Erwärmung ist also proportional zur Stromstärke": the heating power is proportional to the *square* of the current, which is exactly why a thermocouple converter reads the RMS value. Translated faithfully.
- slides/widerstand_ntc_ptc.md (notes) — "Der erste Pfeil die Temperatur an, der zweite Pfeil die Leitfähigkeit" (verb *gibt* missing), with "Hier: Hohe Temperatur, hohe Leitfähigkeit" for the NTC symbol; the section says the second arrow shows the *resistance* (ϑ↑↓ = resistance falls). The note's reading gives the right result only because it swaps resistance for conductivity. Translated faithfully.
- sections/widerstand_materialien.md — metal-film resistors "sind temperaturunabhängig", while the table in the same section (and EC102) says *geringe Temperaturabhängigkeit*. Translated as written.
- sections/leiterwiderstand.md — resistivity defined "bei $\qty{20}{\degree}$": plain degrees, not °C (`\degreeCelsius`). Formula left unchanged.
- slides/spitze_effektiv_wert.md — RMS definition "der Wert, der in einem Widerstand zu einer vergleichsweisen Gleichspannung in Leistung umgesetzt wird" is garbled (*vergleichbaren*, and *zu* makes no sense); translated by its evident meaning, "in the same way as a comparable DC voltage".
- sections/spitze_effektiv_wert.md — "Wenn nicht die Spannungs-, sondern die Leistung …": dangling hyphen with no compound to complete it; translated as "not the voltage but the power".
- sections/widerstandsfarbcode.md — "(siehe Tabelle [ref:…]," bracket never closed; closed in English.
- sections/widerstand_smd.md "$\qty{11000}{\ohm}$ Ohm" and sections/widerstand_toleranz.md "$\qty{1000}{\ohm}$ Ohm" — unit written twice; written once in English.
- Typos with no effect on the English: sections/spitze_effektiv_wert.md "Den Spitzenwert eine Wechselspannung" (*einer*), "Für Sinusförmige", "Wenn man weiß, das" (*dass*); slides/spitze_effektiv_wert.md caption "Peridoendauer"; sections/oszilloskop_1.md "Skaltenteile", "lässt ich"; slides/oszilloskop_1.md "eine Oszilloskops"; slides/oszilloskop_2.md "Zeigt den zeitlichen Verlauf von Spannungen dar" (*Stellt … dar*), caption "Oszillokops"; slides/ohmsches_gesetz.md "Spannungesquellen", "Stromfluß", "der elektrischer Spannung, dem elektrischem Strom"; sections/widerstandsfarbcode.md "vom dem aufgedruckten Wert", "mithilfe des Farbcode"; sections/wechselstrom_leistung.md "vernüftigen", "eine großen Bereich", "Zusammenhänge, bei denen … gerechnet werden können" (*kann*); slides/halbleiter.md "Materialen".

## Provjera

Checker: all 33 files compared paragraph by paragraph with the German
(`git show ceec8fa~1:<file>`); embedded questions read in English
(EB401–EB411, EI301–EI304, AI301–AI306, AI105, NA203, NA204, NA210, NA211,
NB501–NB505, NB601–NB606, NB703, NC102–NC110, NC401–NC404, EC101–EC117,
AB101–AB103, AB301). Nothing dropped or added; numbers, formulas and markup
intact; no German left outside `%` comments and formula subscripts.
`revizija-guard.py --rev ceec8fa~1 --brojevi`: 33 files, *struktura
netaknuta*.

Changes: omission 0, meaning 0, technical 0, style 4, glossary 2.

- widerstand_materialien: *Ein einfach gewickelter Drahtwiderstand* "A simple wound wirewound resistor" → "A wirewound resistor with a simple winding" (style; the German contrasts a plain winding with non-inductive ones).
- halbleiter: "the letters A and K (the usual abbreviation for the cathode)" → "the letters A and K, the usual symbols for anode and cathode" (style; K is the standard symbol in English too, but not an initial).
- wechselstrom_leistung: "These can also be distorted rather than, for example, a pure sine-wave voltage" → "They can also be distorted, rather than being, for example, a pure sine-wave voltage" (style, grammar).
- wechselstrom_leistung slides: "heat radiated at a resistor" → "heat radiated by a resistor" (style).
- oszilloskop_2 slides and glossary §14: *Bezugsmasse* "Reference (earth) connection" → "Earth reference" (glossary; the bracket read as an afterthought).
- Glossary §14: the *NTC (englisch …)* row gave a sentence as its English; reworked into a term row, NTC / PTC (negative / positive temperature coefficient), with the sentence as the example (glossary).

Judgement calls reviewed and kept: *Kaltleiter / Heißleiter* as a material
property → PTC / NTC conductor; *Innenwiderstand* of the scope → internal
resistance (glossary), as for any voltmeter; probe *Masseverbindung* → earth
connection (house style *earth*); *Kästchen* → square beside *division*; the
dropped *(engl. trigger …)*, *(deutsch: …)* and *LED (englisch …)* glosses
(bracket rule); NB505 `\qty{40.000}{\ohm}` matching the English answer. The
other 22 new glossary rows are kept as they are. No DECISIONS.md entry was
added, and none is needed. The suspected errors in the German are confirmed
(tin/zinc 0.11; 1.03 vs 1.02 Ω; heating "proportional" to current rather than
its square; NTC note reading conductivity for resistance; metal-film
"temperaturunabhängig").
