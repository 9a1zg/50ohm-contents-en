# nea_sicherheit — translation report

Chapter "Sicherheit" (Safety): 13 sections, each with its slides, and 4
solutions. 30 files:

- `contents/sections/` and `contents/slides/`: `antennen_baurecht_haftung.md`,
  `antennen_energieleitungen.md`, `elektrische_geaete_oeffnen_1.md`,
  `elektrische_geaete_oeffnen_2.md`, `n_blitzschutz.md`, `blitzerdung.md`,
  `blitzschutz.md`, `schutzerdung_1.md`, `schutzerdung_2.md`,
  `statische_aufladung.md`, `antennen_beruehrung_1.md`,
  `antennen_beruehrung_2.md`, `strahlengang_aufenthalt.md`.
- `contents/solutions/`: `AK201.md`, `AK202.md`, `AK203.md`, `AK204.md`.

`revizija-guard.py --brojevi`: 30 files checked, *struktura netaknuta*.
German-word grep: the only German left is the `%` comments
(statische_aufladung, strahlengang_aufenthalt), the idents, the `<tipp>` tag
(see errors), and the German names in brackets at first mention: *Verband der
Elektrotechnik Elektronik und Informationstechnik e. V.* (n_blitzschutz,
section and slide note) and *Bundesamt für Strahlenschutz*
(strahlengang_aufenthalt). Line counts, trailing spaces and final newlines
are as in the German, except solutions/AK201.md, which is one line shorter
(see judgement calls).

Embedded questions looked up in English and the prose aligned with them:
VE602, VE603, VE604, VE707, NK311, EK201–EK203, EK206–EK211, AK201–AK204
(VE602 "building regulations of the relevant federal state"; VE707 "owner or
operator of the antenna installation", "damage to third parties"; NK311
"parts and cables … must not touch any power lines"; VE603 "recognised codes
of practice", "VDE standards"; EK203 "charged capacitors in the power
supply"; AK201 "high-value resistor with an adequate power rating"; EK209
"building earthing system", "building earth"; EK210 "single solid wire of
copper (16 mm²), aluminium (25 mm²) or steel (50 mm²)", "earthing conductor";
EK211 "lightning protection specialist", "lightning protection concept";
VE604 "applies to all amateur radio transmitting installations"; EK208
"screens … connected to each other and to the main earthing terminal";
AK202 "as low a resistance as possible", "for the protection of persons";
AK203 "separate earthing conductor", "equipotential bonding", "hot", "an odd
multiple"; EK206/EK207 "unearthed wire antennas", "rain or hail",
"high-value bleeder resistors", "without impairing the function of the radio
installation"; EK202 "injuries and burns from RF voltages"; AK204 "even at
low transmit powers of a few watts"; EK201 "staying in the direct beam of
transmitting antennas must be avoided").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

21 rows: *Dachständer / Freileitung / Energieversorgungsleitung*; *Bauamt von
Stadt oder Gemeinde / Nachbargrundstücke / Mitgliedsbeitrag /
Versicherungsleistung*; *Ehrensache / vor lauter Tatendrang*; *Netzseite /
Nennspannung des Netzes / Kondensatoranschlüsse*; *Entladewiderstand /
hochohmiger, isolierter Widerstand / Lichtbogenbildung / Leiterbahnen /
Pulsbetrieb*; *Isolierhandschuhe in einer ausreichenden Schutzklasse /
isoliertes Werkzeug*; *Blitzschutz-Zwischenstecker*; *Erdungsleitung (massiver
Draht, keine Litze) / Gebäudeerdung*; *Schraubanschluss Ground (GND)*;
*Potentialausgleichsschiene / Potentialausgleichsleiter / Ausgleichsstrom*;
*Elektroinstallation / Erdleitungen / Heizungsrohre*; *Spannungsbauch /
HF-Spannungsbauch*; *„heiß" / Herdplatte*; *Prasselstörungen /
Antennenzuführung*; *der Rothammel*; *erschrecken oder verkrampfen /
Sekundärunfall*; the section title *Gefahren durch elektrischen Strom*;
*direkter Strahlengang*; *Gewebe / Wärmeabfuhr / Hoden*;
*HF-Funkenüberschläge / Körperstrom*; *aus Sicht der Niederfrequenz*.

## Added to `DECISIONS.md`

None. The unit follows the glossary (§12 *earth* / *earthing*, *equipotential
bonding*, *main earthing terminal*, *lightning protection system*; §1.2
*recognised codes of practice*, *VDE standards*) and the earlier units'
renderings (*Caution* for the slide heading *Achtung*, as einbau_kfz; the
VDE at first mention and "If in doubt, get help from a more experienced
radio amateur or a qualified electrician", as gefahren; the Federal Office
for Radiation Protection box, word for word as personenschutzabstand_grenzwerte,
whose German it repeats).

## Judgement calls

- antennen_baurecht_haftung: *Baugenehmigung* → "building permit" (glossary §1.2, without its bracket in running text); *vorschriftsmäßig aufgebaut* → "erected in compliance with the regulations"; *der Betreiber … selbst voll verantwortlich* → "the operator is fully responsible for their own antenna installation" (singular *they*, DECISIONS.md); photo caption *KW* → HF.
- antennen_energieleitungen: *Dachständer* (no English counterpart, glossary §9 "describe as needed") → "roof-mounted support" in the text, "Roof-mounted support for an overhead mains line" / "… with overhead line" in the captions; *führen so die elektrische Energie vom Stromnetz zu* → "supply the house with electrical energy from the mains" (*mains*, glossary §12; not *grid*, which §14 keeps for the transmission network); *Energieversorgungsleitung* → "power line", as NK311.
- elektrische_geaete_oeffnen_1: *dürfen grundsätzlich nur von einer Elektrofachkraft durchgeführt werden* → "must, as a matter of principle, only be carried out by a qualified electrician"; *Bei Berührung besteht Lebensgefahr* → "Touching them is a danger to life" (glossary §12 *Lebensgefahr*).
- elektrische_geaete_oeffnen_2: *Ehrensache* → "a point of honour", *vor lauter Tatendrang* → "in all the eagerness to get on with the job"; *Transistorendstufen / Röhrenendstufen* → "transistor PAs / valve PAs" (glossary §14); *Die Belastbarkeit … an die Kapazität … anpasst* → "matched to the capacitance"; slide *Das Verhalten kann lebensgefährlich sein* → "This behaviour can be life-threatening", as written.
- n_blitzschutz: the VDE at first mention as in gefahren, "The Association for Electrical, Electronic and Information Technologies (Verband der Elektrotechnik Elektronik und Informationstechnik e. V.), VDE for short"; slide *Es gibt vom VDE die Norm VDE 0185-305* → "The VDE has issued the standard VDE 0185-305"; note *geben VDE-Normen zur Unfallverhütung raus* → "Publishes VDE standards for accident prevention".
- blitzerdung: *Blitzschutz-Zwischenstecker für Koaxkabel* → "in-line lightning protection adapters for coaxial cable"; *massiver Draht, keine Litze* → "solid wire, not stranded" (EK210); *Alu* → aluminium; *Gebäudeerdung* → "building earth" (EK209); the VDE guide as link text in English ("guide to protecting radio installations on buildings against lightning strikes"), as the BNetzA documents in nea_personenschutzabstand_1; slide *Ursache ist Induktion in Strom- oder Telefonienetz* → "induction in the mains or telephone network"; *Antennen-Standrohre* → "antenna masts" (EK211, glossary §12 *Standrohr*).
- blitzschutz: caption *Schraubanschluss Ground (GND) am TRX* → "Ground (GND) screw terminal on the TRX": *Ground (GND)* is the label printed on the radio and is kept; the text itself says *earth* / *earthing* throughout (glossary §12). *Anpassgerät* → "antenna tuning unit" (§9).
- schutzerdung_2: *Potentialausgleichsschiene im Keller* → "equipotential bonding busbar in the basement"; *Spannungsbauch* → "voltage antinode", as strom_spannung_speisung; *Die Funkamateure sagen, das Gehäuse ist „heiß"* → 'Radio amateurs say the case is "hot"', as AK203; *zurückschrecken* → "flinch back"; slide *berührungsempfindlich* → "sensitive to touch", as written (see errors).
- statische_aufladung: *Prasselstörungen* → "crackling interference"; *Ableitwiderstände* → "bleeder resistors" (EK207, glossary §12); slide note *Die 100 kΩ stammen aus dem Rothammel* → "comes from the Rothammel antenna book": "antenna book" added so that the English reader knows what *the Rothammel* is (the standard German antenna handbook); the `%` comment citing it stays German.
- antennen_beruehrung_1: *hohe hochfrequente Wechselspannungen* → "high AC voltages at radio frequency"; *erschrecken oder verkrampfen* → "give you a fright or make your muscles cramp", as gefahren's "fright … muscle cramp"; the section title *"Gefahren durch elektrischen Strom"* → *"Dangers of electric current"*, quoted in English (section titles are not yet translated; as wellenlaenge_2 "In the section on "Rearranging formulas""). *Ein(e) Sendeantenne in Betrieb berührt man nicht!* → "You do not touch a transmitting antenna in operation!" throughout.
- antennen_beruehrung_2: slide heading *Abhängigkeit von Antennentyp und Sicherheit* → "Dependence on the type of antenna, and safety", keeping the German's two topics.
- strahlengang_aufenthalt: *Strahlengang* → "direct beam", as EK201 (glossary §14 *Strahlengang* → radiation path stays for the optics of a dish); *Hoden* → "testes"; *grundsätzlich für alle Menschen* → "in principle for everyone"; link text *Hamnet* kept as written; *Deshalb wird speziell nach dem Umgang mit Mikrowellen gefragt* → "That is why there is a question specifically on handling microwaves"; slide note *Aufgrund der sehr unterhaltsamen Distraktoren* → "Thanks to the very entertaining distractors".
- AK201: *führen.* on its own line after the list (the German verb at the end of the sentence) cannot stay at the end in English: the verb moves up ("would lead to:") and the line with *führen.* and its blank line are dropped, so the file is one line shorter than the German. The doubled *dass* is not reproduced (see errors). `\kilo\Ohm` left unchanged.
- AK203: *elektrisch leitungsbedingt etwa λ/4 … lang* → "If the electrical length of the connection …, as a line, is about λ/4"; *verlustbehaftete HF-Transformationsleitung* → "lossy RF transformer section" (glossary §9 *Transformationsleitung*); *aus Sicht der Niederfrequenz* → "At low frequencies": here DC and the mains frequency, not audio, so not *AF*; *bei hochfrequentem Betrieb* → "At radio frequencies"; *als hoher Widerstand erscheinen* → "appear as a high resistance", as written.
- AK204: the list after *aus folgenden Gründen* recast as a list of clauses ("it can cause skin burns, …"); *5 bis 10 Watt* → "5 to 10 W" (unit symbol).

## Suspected errors in the German original

- sections/elektrische_geaete_oeffnen_2.md — the box is tagged `<tipp>…</tipp>`; the DARCdown tag is `<tip>`, so the box is probably not rendered as a tip. Tag left unchanged.
- slides/schutzerdung_2.md — "Hochfrequenzströme suchen oft eigene Wege – separate Erdungsleitungen können dadurch in Resonanz … geraten": the resonance comes from the length of the lead (next slide), not from RF "finding its own paths"; and "Das Sendergehäuse wird … berührungsempfindlich" means "sensitive to touch", where "dangerous to touch" is meant. Translated as written.
- slides/blitzerdung.md — "in ein vorhandenes *Blitzschutzkonzept* integriert": the section says *Blitzschutzsystem*; an antenna is integrated into the system and provided for in the concept (EK211). Translated as written.
- solutions/AK201.md — "Dieser wird so dimensioniert, dass: * dass der Anfangsstrom …" (*dass* twice); `\qty{100}{\kilo\Ohm}` uses `\Ohm`, where the course writes `\ohm` (as in AK103). Formula left unchanged.
- solutions/AK204.md — "* sie Hautverbrennungen verursachen können," after "aus folgenden Gründen potenziell gefährlich:" — the items mix a clause without conjunction (*sie … können*, plural for *Spannung*) with main clauses.
- Typos with no effect on the English: sections/elektrische_geaete_oeffnen_1.md "von Netz trennt" (*vom*); sections/elektrische_geaete_oeffnen_2.md "den vorhanden Schaden" (*vorhandenen*), "anpasst werden" (*angepasst*); slides/elektrische_geaete_oeffnen_1.md "Energie …, die gefährlich werden können" (*kann*); sections/antennen_energieleitungen.md and slides double space in the danger box; sections/blitzerdung.md "wenn er einschlägt wird", "keine Litze) deren", "muss man wissen was" (commas missing), "einer vorhanden Blitzschutzanlage" (*vorhandenen*), the indepth sentence without a full stop; sections/blitzschutz.md "einen spezieller Schraubanschluss" (*speziellen*); slides/n_blitzschutz.md "geben VDE-Normen … raus" (*gibt*, colloquial); sections/schutzerdung_1.md "alle elektrische leitende Teile" (*elektrisch*), "Ursachen haben z.B." (comma); sections/schutzerdung_2.md "Zwischen den verschieden Leiter" (*verschiedenen Leitern*), "bei einigen Amateurfunkbänder" (*-bändern*), "niederohmig sein um" (comma), "zurück schreckt" (*zurückschreckt*); sections/statische_aufladung.md "durch  Regen" (double space); sections/antennen_beruehrung_1.md "Ein Sendeantenne" (*Eine*); sections/antennen_beruehrung_2.md "Wo die Spannungsbäuche entstehen hängt" (comma), caption 852 "Deshalb ist Verletzungsgefahr" (article missing); sections/strahlengang_aufenthalt.md "über die biologische Wirkungen von hochfrequenten Felder" (*biologischen*, *Feldern*; the same box as in personenschutzabstand_grenzwerte).

## Provjera

All 30 files compared paragraph by paragraph with the German (`012cd61~1`),
and the prose checked against the English of the 18 embedded questions.
Nothing dropped or added; the AK201 restructuring (verb moved up, the
*führen.* line dropped) is right. The 21 glossary rows are kept, one
reworked; no DECISIONS.md entry was needed, and none is added. Every
judgement call in the report is kept. Guard (`--rev 012cd61~1 --brojevi`):
30 files, *struktura netaknuta*.

Changes: omission 0, meaning 0, technical 2, style 6, glossary 1.

- solutions/AK203.md (technical): "this low-resistance point can be transformed in impedance by the λ/4 line" → "the impedance of this low-resistance point can be transformed by the λ/4 line"; the first sentence reordered so that "as a line" qualifies the electrical length ("has an electrical length, as a line, of about λ/4").
- solutions/AK204.md (technical): *relevante Gefährdung* "a relevant hazard" (a calque) → "a significant hazard".
- sections/strahlengang_aufenthalt.md (style, 2): "at microwaves" → "at microwave frequencies".
- sections/elektrische_geaete_oeffnen_1.md (style): "How long for depends" → "How long they do so depends".
- sections and slides/antennen_beruehrung_1.md (style, 2): "a fall from the ladder" → "a fall from a ladder"; slide "fright and cramp" → "fright and muscle cramp", as gefahren.
- solutions/AK201.md (style): "within a reasonable time in practice" → "within a practicable time".
- TRANSLATION_GLOSSARY.md (glossary): the row *erschrecken oder verkrampfen* gave "get a fright or cramp up", which the text does not use; now "give you a fright or make your muscles cramp / fright and muscle cramp", as the text and gefahren have it.
