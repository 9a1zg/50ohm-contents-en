# swl_1 — translation report

Chapter "SWL-Kurs (1/2)": 13 sections, each with its slides, no solutions.
26 files:

- `contents/sections/` and `contents/slides/`: `swl_vorwort.md`,
  `swl_was_ist_swl.md`, `swl_erste_empfangsstation.md`,
  `swl_modulationsarten.md`, `swl_bedienung.md`, `swl_steckverbinder.md`,
  `swl_ionosphaere.md`, `swl_sporadic_e.md`, `swl_elektrische_sicherheit.md`,
  `swl_antennensicherheit.md`, `swl_rufzeichen.md`, `swl_landeskenner.md`,
  `swl_frequenzbereiche.md`.

`revizija-guard.py --brojevi`: *struktura netaknuta*. German-word grep: no
hits outside the German names kept on purpose (*Kurzwellenhörer*,
*Höramateur*, *Hauptverwaltung für das Post- und Fernmeldewesen des
Vereinigten Wirtschaftsgebietes*, *Deutsche Empfangsstation*, *OEsterreich*,
*Schönes Polen*, *EspaniA*, *PAys-Bas*). Line counts, the trailing spaces
(sections: swl_erste_empfangsstation line 47, swl_modulationsarten line 17,
swl_steckverbinder line 3, swl_rufzeichen line 31), the space before the full
stop after *DE1JMU* and the missing final newlines (sections: swl_was_ist_swl,
swl_modulationsarten, swl_bedienung, swl_sporadic_e,
swl_elektrische_sicherheit, swl_antennensicherheit) are as in the German.

Embedded questions looked up in English and the prose aligned with them:
VD102 ("authorisation to participate in the amateur service"), NE209 (USB
"upper sideband"), NF105 ("waterfall display"), NG202–NG205 ("RF connector
series"), NH101 (refraction, ionosphere), NH201 ("eleven-year solar cycle"),
NH306 ("1000 to 2000 km", "sporadic E"), NK305 ("supply leads", "same current
rating and the same tripping characteristic"), VE707 ("owner or operator",
"damage to third parties"), VD201 ("Call Sign Plan"), VD202 ("personal call
signs, … remotely controlled and automatically operating amateur stations,
club station call signs"), BD103–BD106 ("two- or three-letter suffix",
"Class A personal call sign"), BD303, BD305, BD311 (country names, "Czech
Republic" in the table as in internationale_landeskenner).
SWL004–SWL011 are in `contents/questions/fragenkatalog_swl.json`, which is
still German (outside this unit); the table and tip are written so that they
fit the German wording ("Welchem Amateurfunkband entspricht der
Frequenzbereich …") once it is translated.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

17 rows: *Kurzwellenhörer / Höramateur*; *DE-Prüfung / SWL-Prüfung*;
*DE-Kennzeichen / Hörerkennzeichen / SWL-Nummer / Mitgliedsnummer*;
*Hörbericht / Empfangsbericht / Empfangsrapport*; *Sendegenehmigung*;
*Weltempfänger / SDR-Stick / SDR-USB-Stick / Mini-Whip-Antenne*;
*Außenantenne / Zimmerantenne / Empfangsantenne / Empfangsanlage /
Empfangsstation*; *Typischer Einstieg*; *Signalstärkeanzeige*;
*Steckdosenleiste / Zuleitungen / netzspannungsführende Geräte*; *Ladegerät /
aufgeblähte Akkus*; *Miet-, Bau- und Denkmalschutzrecht*; *Hauptverwaltung für
das Post- und Fernmeldewesen des Vereinigten Wirtschaftsgebietes*; *Deutsche
Empfangsstation*; the SWL country-prefix memory aids (*Anfangsbuchstabe*,
*LuXemburg*, *Franz. PAys-Bas*); *Daumenregel / Faustregel / Faustformeln*;
*VFDB*.

## Added to `DECISIONS.md`

One entry (Course text): SWL course terms — *DE-Kennzeichen* → DE identifier
(not "DE call sign"), *DE-Prüfung* → DE examination, *Hörbericht* → listener
report; the German name *Kurzwellenhörer* kept, with the English in brackets,
where the text remarks on it. swl_2 follows this.

## Judgement calls

- swl_vorwort / swl_was_ist_swl: "trotz der deutschen Bezeichnung *Kurzwellenhörer*" kept as information about German usage, "Despite the German name *Kurzwellenhörer* (short-wave listener)"; the vorwort's *Ein Kurzwellenhörer wird international als SWL bezeichnet* → "A short-wave listener, in German *Kurzwellenhörer*, is known internationally as an *SWL*", so the contrast German name / international abbreviation survives. The German's English expansion *Short Wave Listener* kept as written; index term [index:Short-wave listener].
- swl_vorwort: closing *vy 73 (Viele Grüße) und 55 (Viel Erfolg) wünschen* → "vy 73 (best regards) and 55 (every success) from", the line break before the names kept; 73 as the abbreviation table's "Best regards"; *dieses Angebot* → "this" (the course and platform as a whole).
- swl_vorwort: *Amateurfunkkurs der Klasse N* (link text and slide) → "Class N amateur radio course"; *(z.B. ein SDR-Stick in [ref:…])* → "(e.g. an SDR stick as in [ref:…])", no "Figure" added since the German has none.
- swl_was_ist_swl: *Zulassung zum Amateurfunkdienst* → "authorisation to participate in the amateur service", the wording of VD102 embedded right after it; bare *Zulassung* (slides, tip in swl_erste_empfangsstation) → "licence" (§1.3).
- swl_was_ist_swl: *DOK des DARC-Ortsverbandes* → "the district local club identifier (Distriktsortskenner, DOK) of the DARC local club" at first mention, as N_Ende; *Ortsverband* → local club, *der örtliche Amateurfunkverein* → "the local amateur radio club", *der örtliche DARC-Ortsverband* → "the local DARC club".
- swl_was_ist_swl slide note: generic *Er kann sich trotzdem …* → "They can still …" (DECISIONS.md, generic *er*); *Amateurfunkgeschehen* → "amateur radio".
- swl_erste_empfangsstation: *Kurzwelle / Kurzwellenempfänger / Kurzwellenbänder* → HF / HF receiver / HF bands where a band is meant; "short wave" where the text speaks of the name or the waves (*nicht auf Kurzwelle beschränkt*, *Kurzwellen werden gebrochen*).
- swl_erste_empfangsstation slides: table *Gerät | Typischer Einstieg* → "Radio | Typical way in", caption *Empfänger für unterschiedliche Einstiegsbereiche* → "Receivers for different ways in"; *Ein Receiver ist ein reiner Empfänger* → "A *receiver* only receives" (the German glosses the English word).
- swl_modulationsarten / swl_bedienung: *Modulationsart* on the receiver → "mode", *Modulationsarten* as the concept and in headings → "types of modulation" (§14 row); *Sprechfunk* in the table → "Voice" (§2); *hochfrequente Trägerwelle* → "radio-frequency carrier wave"; *aufgeprägt* → "impressed on" (§14).
- swl_bedienung: *Amplitudenspektrum* kept as "amplitude spectrum" (§14), not glossed again; *HF-Verstärkung* → "RF gain"; caption 95 *Display mit Frequenzanzeige, …* → "Display with frequency display, …", as the earlier caption of the same photo (wasserfall).
- swl_steckverbinder: *System* → "series" (§14 *Steckverbindungs-System*, NG202–NG205); captions as the connector decision (DECISIONS.md): *N-Einbaubuchse und N-Stecker* → "N panel socket and N plug", *BNC-Winkeladapter mit Stecker und Kupplung* → "BNC right-angle adapter with plug and socket"; *N-Buchse* (no contrast) → "N socket"; *verkanten* → "force in at an angle".
- swl_ionosphaere: *Tote Zone* → skip zone (§10); slide note *Brechung beziehungsweise Refraktion* → "refraction" (one English word, §14); *höhere Kurzwellenfrequenzen* → "higher frequencies in the HF range"; *an diesen Bereichen* → "in these areas" (*Bereich* is neither *Region* nor *Schicht*).
- swl_sporadic_e: *Sporadic-E* → "sporadic E" (§10, §14), heading "Sporadic E"; *E-Region* → "E region" (DECISIONS.md, word for word); *eher geradlinig* → "more or less in straight lines".
- swl_elektrische_sicherheit: *Feinsicherungen* → miniature fuses, *Nennstrom* → current rating, *Auslösecharakteristik* → tripping characteristic (NK305); *Akkus* → "rechargeable batteries", then "batteries" (DECISIONS.md *Akku*); *Antennenleitungen* → antenna feeders; *Reparaturen … gehören in fachkundige Hände* → "should be left to qualified people".
- swl_antennensicherheit: *Denkmalschutzrecht* → "heritage protection law"; *lebensgefährlich* → "can be fatal"; *vorschriftsmäßig aufgebaut* → "erected in compliance with the regulations" (§12).
- swl_rufzeichen: the Bundesnetzagentur at first mention in the section and in the slides "Federal Network Agency (Bundesnetzagentur, BNetzA)", then "BNetzA"; *Rufzeichenplan* → "Call Sign Plan" (§1.2, VD201); in the indepth *de (= von)* → '*de* (= "this is")' (§14 voice procedure, abbreviation table DE → "This is"); *Hauptverwaltung … des Vereinigten Wirtschaftsgebietes* → "the Main Administration for Posts and Telecommunications of the United Economic Area" with the German name in brackets (no settled English name; the United Economic Area is the Bizone); *Deutsche Empfangsstation* kept in German with "(German receiving station)", because DE abbreviates the German words.
- swl_rufzeichen slides: table header *Beginn | Verwendung* → "Starts with | Use"; *SWL-Prüfung* kept as "SWL examination" (the German uses both names).
- swl_landeskenner: memory aids by the mnemonic decision (DECISIONS.md): *Anfangsbuchstabe* → "Initial letter" (France also starts with F), *LuXemburg* → "LuXembourg" (same letters), *Franz. PAys-Bas* → "French: PAys-Bas", *OEsterreich (Austria)* and *Schönes Polen (beautiful Poland)* as internationale_landeskenner; *Merkhilfe* → "Memory aid" (§14); *Schrägstrich* → "stroke" (§2).
- swl_frequenzbereiche: decimal commas → points in all `\qty`/`\qtyrange`; `\text{in~}` left as it is (the running word is "in" in both languages); *Nutzungsbestimmungen* → "conditions of use" (§14); *Faustformeln* → "rule-of-thumb formulas".

## Suspected errors in the German original

- sections/swl_ionosphaere.md and slides — "In Phasen hoher Sonnenaktivität gibt es mehr Sonnenflecken und dadurch werden höhere Kurzwellenfrequenzen häufiger … nutzbar": the sunspots are a sign of high activity, not its cause; the higher usable frequencies come from the stronger UV and X-ray radiation that ionises the F region more. A causal simplification. Kept ("and as a result").
- sections/swl_elektrische_sicherheit.md — "müssen Nennstrom und Auslösecharakteristik dem vorgesehenen Ersatz entsprechen": circular; what is meant is that the replacement must match the specified (original) values, as NK305 says ("same current rating and the same tripping characteristic"). Rendered "must match those specified for the replacement".
- sections/swl_antennensicherheit.md — "Für Schäden … haftet grundsätzlich der Betreiber der Antennenanlage", while the slide and VE707 say *Eigentümer oder Betreiber*. Not wrong ("grundsätzlich"), but the two places differ. Kept as each says.
- Typos with no effect on the English: sections/swl_vorwort.md "mit einem geeigneten Empfänger (z.B. ein SDR-Stick …)" (*einem SDR-Stick*); sections/swl_bedienung.md "USB (Oberes Seitenband bei SSB)" (*oberes*); sections/swl_was_ist_swl.md "*DE1JMU* ." (space before the full stop, kept).

## Provjera

Checked all 26 files paragraph by paragraph against `de26800~1`, the embedded
questions (VD102, NE209, NF105, NG202–NG205, NH101, NH201, NH306, NK305,
VE707, VD201, VD202, BD103–BD106, BD303, BD305, BD311) in English, the
glossary and DECISIONS.md. Nothing dropped or added; numbers, tables and
captions complete. Kept as they are: all judgement calls, the 17 glossary
rows (they agree with §2 *Kurzwellenhörer*, *Hörerkennzeichen* and the
N_Ende *DOK* row), the DECISIONS.md entry on the SWL course terms, and the
suspected errors in the German (all fair). *Zulassung zum Amateurfunkdienst*
as "authorisation to participate in the amateur service" kept, because VD102
follows it directly with that wording. `revizija-guard.py --rev de26800~1
--brojevi`: 26 files, *struktura netaknuta*.

Changes: omission 0, meaning 1, technical 0, style 7, glossary 0.

- swl_steckverbinder section and slide note: *nicht entscheidend* "does not
  matter" → "is not a deciding factor" (the German says it is not decisive,
  not that it is irrelevant).
- swl_vorwort section: *Schon mit einem geeigneten Empfänger* "Even with" →
  "With just" ("even" read as a concession).
- swl_steckverbinder section and slide: *verkanten* "force connectors in at
  an angle … by force" → "insert connectors at an angle" (no doubled
  "force").
- swl_bedienung slide note: "What the S meter shows exactly follows later" →
  "The exact meaning of the S meter reading is covered later".
- swl_ionosphaere slide note: "For a start, it is enough" → "At this stage,
  it is enough".
- swl_elektrische_sicherheit section: "A receiver also needs electrical
  energy" → "Even a receiver needs electrical power".
- swl_elektrische_sicherheit section and slide note: "can let leads and
  components overheat" → "can allow leads and components to overheat".
- swl_elektrische_sicherheit section: the German's prescriptive present
  (*werden nicht weiter benutzt*, *werden … verlegt*, *wird … nicht benutzt*,
  *werden nur dann getrennt*) as "should …" instead of statements of fact.
