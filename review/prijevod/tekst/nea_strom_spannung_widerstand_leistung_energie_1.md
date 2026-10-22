# nea_strom_spannung_widerstand_leistung_energie_1 — translation report

Chapter "Strom, Spannung, Widerstand, Leistung, Energie (1/3)" (Current,
voltage, resistance, power, energy, part 1): 12 sections, each with its
slides, and one solution. 25 files:

- `contents/sections/` and `contents/slides/`: `recht_zum_selbstbau.md`,
  `spannung.md`, `strom.md`, `gefahren.md`, `leiter_nichtleiter.md`,
  `stromkreis.md`, `physikalische_stromrichtung.md`, `spannungsmessung.md`,
  `strommessung.md`, `strom_spannung_messung_2.md`,
  `strom_spannung_messung_3.md`, `zeigerinstrumente_ablesen.md`.
- `contents/solutions/AI104.md`.

`revizija-guard.py --brojevi`: 25 files checked, *struktura netaknuta*.
German-word grep: no hits outside idents (`n_messgeraete_symbol_…gerät`) and
the intended German (the VDE's German name, the formula subscripts below).

Embedded questions looked up in English and the prose aligned with them:
VC109, VE401–VE405, VE601, NA201, NA202, NA208, NA209, NK301–NK304,
NB101–NB104, NB205–NB207, NB701, NB702, NC101, AB601, NI101–NI104,
EI101–EI104, AI101–AI104.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

20 rows: *behördliche Zulassung* (official approval), *EU-Konformitätserklärung
/ Importeure und Händler*, *Selbstbau*, *Hochspannungsleitungen im Stromnetz /
Höchstspannungsleitung*, *Blitzableiter*, *elektrische Stromstärke* (course
text), *Stromquelle* (course text), *physikalische Stromrichtung*, the water
circuit analogy, *Kipp-/Schiebeschalter*, *Herzstillstand / EKG*,
*Sekundärunfälle / Schreck*, the five safety rules, *Messleitung / Anschluss*,
*Zeigerinstrument / Zeiger / Zeigeranzeige*, *kleinste Auflösung /
Auflösungsvermögen*, *Messgenauigkeit*, *Kenngröße / Faustregel*,
*Stromteilung*, *reales Spannungs-/Strommessgerät*.

## Added to `DECISIONS.md`

Nothing: every choice here is a single term, recorded in the glossary.

## Judgement calls

- recht_zum_selbstbau: the VC109 answer wording taken over word for word ("transmitting equipment that is commercially available, home-built or converted to amateur frequencies"); *behördliche Zulassung* → "official approval" (not *licence*); *Aufgaben von Importeuren und Händlern* → "duties of importers and distributors" (EU wording); FuAG in full with the German name at first mention in section and slides, then "the FuAG", and "Radio Equipment Act" where the German writes *Funkanlagengesetz* again (as VE405).
- spannung: *Stromnetz* (high-voltage lines up to 380 kV) → "electricity grid", not the glossary's *mains*, which is the household supply; *Höchstspannungsleitung* (table) → "extra-high-voltage line", kept apart from the prose's *Hochspannungsleitungen* → "high-voltage lines", as the German does; *Aufgabe* (an exam question) → "question"; unit names in the prefix tables lower case ("1 kilovolt").
- strom: *Wir sprechen von der elektrischen Stromstärke* → "We speak of the electric current" — English has no separate word for *Stromstärke* (glossary §3, NA202 "electric current").
- gefahren: the VDE at first mention as "the Association for Electrical, Electronic and Information Technologies (Verband der Elektrotechnik Elektronik und Informationstechnik e. V.), VDE for short" (German name as the text spells it); *anerkannte Regeln der Technik* → "recognised codes of practice" (VE601); the AC/DC sentence → "Alternating voltage is also abbreviated "AC" (alternating current), and direct voltage "DC" (direct current)", the *englisch* glosses dropped; slides *Wechselspannung (AC)* → "Alternating voltage (AC)" so the bracket does not repeat "AC voltage".
- gefahren: the five safety rules in the established English short forms of DIN VDE 0105-100 / EN 50110 ("Isolate", "Secure against reconnection", "Verify that no voltage is present", "Earth and short-circuit", "Cover or fence off adjacent live parts" — the last one literal, as the German); *5 Sicherheitsregeln* → "5 safety rules of electrical work" (glossary), digit kept; *Schreck* → "fright"; *EKG* → "ECG".
- gefahren: *Störlichtbogen* → "arc fault" (NK302); slides *(Stör-)Lichtbogen* → "arc (arc fault)".
- stromkreis: *Stromquelle wie eine Batterie* → "power source", because *current source* is a circuit element in English; *Widerstand … wandelt Strom in Wärme um* → "converts electricity into heat" (*Strom* in its everyday sense); in the danger box *durch einen Widerstand, z. B. einen Verbraucher* → "through a resistance, e.g. a load" (the quantity, as a load is not a resistor); *technische Stromrichtung* → "conventional current flow" (NB702).
- physikalische_stromrichtung: *physikalische Stromrichtung* → "*electron flow*, the physical direction of current" (AB601's pairing); in the indepth on ions it stays "the physical direction of current", since *electron flow* would be wrong there; caption "Conventional current flow and electron flow".
- spannungsmessung / strommessung: *Messleitung* → "test lead", *Anschluss* (multimeter) → "socket"; *"COM" (englisch "common")* → `"COM" (for "common")`; *Kapitel Strom- und Spannungsversorgung* → "the chapter on power supplies" (catalogue heading, glossary §5); *Feinsicherung* → "miniature fuse".
- strom_spannung_messung_2 slides: *eingeschleift* → "with the meter inserted into the circuit" (EI101 "inserted into the circuit").
- strom_spannung_messung_3: *Verstärker (Power Amplifier, PA)* → "power amplifier (PA)" (bracket rule: the English name is not glossed back); *kleinste Auflösung* → "finest resolution", as AI104, also in the tip quoting it; the clock example "13 hours, 3 minutes and 10 seconds" (a clock time like "13:03" would change the numbers the guard checks); *fünf Prozent* → "five per cent".
- strom_spannung_messung_3 and slides: the subscripts `U_\text{Gemessen}`, `U_\text{Wahr}`, `P_{\textrm{Abw}}`, `U_{\mathrm{Abw}}` stay German (DECISIONS.md, word subscripts are symbols); the prose around them is English. They belong to the later one-pass treatment of word subscripts.
- zeigerinstrumente_ablesen: *Zeigerinstrument* → "analogue meter" (glossary §11), *Zeiger* → "needle", *Zeigeranzeige* → "needle display"; *Anschlag* → "end stop"; *das Komma … verschieben* → "move the decimal point".

## Suspected errors in the German original

- sections/strom_spannung_messung_3.md — "Neben dem idealen Strommesser enthält ein reales Spannungsmessgerät einen parallelgeschalteten Widerstand": the drawing (1004) shows an ideal *voltmeter* (circle with V) with R_i in parallel; an ideal ammeter in parallel would short R_i. Should be *Spannungsmesser*. Translated faithfully as "the ideal ammeter".
- sections/strommessung.md (danger box) and slides — "Strommessgeräte haben selber keinen Widerstand": strom_spannung_messung_2 and _3 say an ammeter has a *low* internal resistance, ideally 0 Ω; the N text overstates it.
- slides/recht_zum_selbstbau.md — "EU-Konformitätserklärung (*CE-Kennzeichnung*) … erstellen" equates the declaration of conformity with the CE marking; they are two different things (the marking is affixed on the basis of the declaration), as the section keeps them apart.
- sections/strom.md and slides (person box) — Ampère "in den 1820er Jahren die elektrische Spannung und den elektrischen Strom wissenschaftlich erklärte": Ampère's work of the 1820s was on electrodynamics (the forces between currents); he did not explain voltage. Translated faithfully.
- sections/spannung.md — the prose puts "bis zu 380 kV" on *Hochspannungsleitungen*, the table calls the same 380 kV line a *Höchstspannungsleitung* (380 kV is extra-high voltage). Each translated as written.
- Typos with no effect on the English: sections/strom.md "nach dem französischem Physiker" (*französischen*); sections/gefahren.md "Dazu werden die VDE-Normen herauszugeben", "beachten werden" (*beachtet*), "hervorgerufenden" (*hervorgerufenen*, also slides), "Austrittstellen", "Stromfluß" (twice), and the VDE's name with "und" (officially *Verband der Elektrotechnik Elektronik Informationstechnik*); slides/recht_zum_selbstbau.md "verschiede" (*verschiedene*); sections/spannung.md table "elektrostatisch aufgeladenen Antenne" (*aufgeladene*); slides/physikalische_stromrichtung.md "entgegen gesetzt", "*Physikalische*"; sections/strom_spannung_messung_2.md "Ein Strom- oder Spannungsmessung" (*Eine*), "beeinflußt"; sections/strommessung.md "hindurchfliesst"; slides/spannungsmessung.md "Subtrahieren"; sections/zeigerinstrumente_ablesen.md "ein Analoges Multimeter", "kann auf den kleinsten Bereich heruntergeschaltet, der …" (*werden* missing).
