# nea_personenschutzabstand_2 — translation report

Chapter "Personenschutzabstand (2/2)" (Safety distance for the protection of
persons, part 2): 4 sections, each with its slides, and 11 solutions. 19
files:

- `contents/sections/` and `contents/slides/`: `naeherungsformel_1.md`,
  `naeherungsformel_2.md`, `personenschutzabstand_3.md`,
  `personenschutzabstand_richtantennen.md`.
- `contents/solutions/`: `AK105.md` … `AK115.md`.

`revizija-guard.py --brojevi`: 19 files checked, *struktura netaknuta*.
German-word grep: the only German left is the `%TODO` comment and the URL in
naeherungsformel_1, the formula subscripts and symbols (`P_\text{Sender}`,
`a_{\textrm{Kabel}}`, `P_{Sender}`, `\textrm{Faktor}_\textrm{FmodPers}`), and
the formula-sheet section name in brackets in AK105 (*Pegel*,
*Strahlungsleistung und Gewinn*). Line counts, trailing spaces and final
newlines are as in the German.

Embedded questions looked up in English and the prose aligned with them:
EK105, EK106, EK108, AK102–AK115 (EK105 "measurements of the E- and H-field
components, simulations or near-field calculations", "reactive near field";
EK106 "far-field approximation formula"; AK102 "wave impedance of the
medium"; AK103 "near-field calculations (simulations)"; AK104 "power at the
feed point of the antenna", "attenuation factor"; AK105 "area that is not
controllable", "critical angle", "direction of maximum radiation"; AK106–AK112
"limit for the protection of persons", "modulation method" / "transmission
method"; AK115 "effective radiated power (ERP)").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

12 rows: *Näherungsformel / Fernfeld-Näherungsformel / Fernfeldformel /
Abstandsformel*; *Fernfeld (bzw. strahlendes Nahfeld) / Freiraum*;
*Erläuterungen zur BEMFV* (link text); *Umrechnungsfaktor
Faktor_FmodPers*; *Strahlungskeule / Hauptstrahlungskeule / Winkeldämpfung*;
*Hilfsmittel der Bundesnetzagentur* and the formula-sheet sections *Pegel*,
*Strahlungsleistung und Gewinn*; the solution headings of AK106–AK115; the
solution headings of AK105; *Leistungszusammenhang EIRP und ERP*;
*Bonusfrage*; *Portabelbetrieb*; *Feldwellenwiderstand im Vakuum /
Wellenwiderstand des Mediums*.

## Added to `DECISIONS.md`

None. The unit follows the entry of nea_personenschutzabstand_1 (*gain
factor*, *wave impedance* / *impedance of free space*, EIRP written
"equivalent isotropically radiated power") and the formula-sheet keyword
entry (nea_bauelemente_1).

## Judgement calls

- *Näherungsformel* → "approximation formula", *Fernfeld-Näherungsformel* → "far-field approximation formula" (EK105, EK106), *Fernfeldformel* → "far-field formula", *Abstandsformel* → "distance formula"; *Fernfeld (bzw. strahlendes Nahfeld)* → "far field (or radiating near field)".
- naeherungsformel_1: *Erläuterungen zur BEMFV* (link text, a short name) → "Explanations of the BEMFV", as written, rather than the full title used in nahfeld; URL unchanged.
- naeherungsformel_1: *plus der Gewinn von 2,15 dBi für den isotropen Strahler (der Antennengewinn bezieht sich auf den Dipol)* → "plus the gain of 2.15 dBi for referring it to the isotropic radiator" — a literal "for the isotropic radiator" would read as the isotropic radiator's own gain.
- naeherungsformel_1: *Auf diesen Sachverhalt zielt die folgende Frage ab* → "The following question addresses exactly this point"; *Die gerundet berechnete Leistung* → "The power calculated with the rounded factors"; *ein richtiger Sicherheitsabstand* → "a real safety distance".
- naeherungsformel_2: *Dabei bezeichnet $Z_0$ den Feldwellenwiderstand des freien Raums* → "the impedance of free space" (glossary §14, DECISIONS.md), and *nähert sich dieser … an* → "it approaches", as the German says (see errors); elsewhere *Feldwellenwiderstand* → "wave impedance"; caption "Variation of the wave impedance across the near-field and far-field regions (logarithmic)", in the form of the nahfeld captions.
- naeherungsformel_2: the Federal Network Agency at first mention in the section as "Federal Network Agency (Bundesnetzagentur, BNetzA)"; in the solutions, as in AK103, "the Federal Network Agency's examination aids" (glossary §14 *Hilfsmittel (Prüfung)*).
- personenschutzabstand_3 and naeherungsformel_2 slides: *nach § 9, BEMFV* → "under Section 9 BEMFV" (EK105), *In § 8 BEMFV ist … festgelegt* → "Section 8 BEMFV lays down"; short citations, as in part 1; *Bei der Anzeige* → "When a fixed amateur radio installation is notified".
- personenschutzabstand_3 and slides: `$\textrm{Faktor}_\textrm{FmodPers}$` kept: it is the name of the field in the BEMFV notification that the reader has to fill in, a symbol like the German subscripts, not a word written as a quantity; *Umrechnungsfaktor* → "conversion factor"; *Spitzenleistung (PEP)* → "peak envelope power (PEP)", *mittlere Leistung* → "mean power" (glossary §7).
- personenschutzabstand_richtantennen: *Winkeldämpfung* → "off-axis attenuation" (glossary §14), *Strahlungskeule* → "radiation lobe", *Hauptstrahlungskeule* → "main lobe" (glossary §9); *unbedingt eingehalten werden müssen* → "must be complied with without fail"; *halbiert sich … auf die Hälfte* → "is halved".
- AK105: *im Kapitel "Pegel"* → 'in the section "Levels" (*Pegel*)', *im Kapitel "Strahlungsleistung und Gewinn" von Antennen* → 'in the section "Radiated power and gain" (*Strahlungsleistung und Gewinn*) of antennas', formula-sheet section names as keywords (DECISIONS.md); headings *Teil 1/2 des Lösungsansatzes* → "Approach, part 1/2", *Einsetzen* → "Substituting".
- AK106–AK115: headings *Benötigte Formeln* → "Formulas needed", *Angaben aus der Aufgabenstellung* → "Data from the question", *Lösungschritte* → "Solution steps", *Interpretation* kept; *Der Grenzwert für den Personenschutzabstand ist* → "The limit for the protection of persons is", as the questions word it; *Da es sich um einen Dipol handelt, gilt:* → "Since it is a dipole:"; *Die Sendeleistung beträgt 100 Watt* → "The transmit power is 100 W" (unit symbol).
- AK115: *Die äquivalente Strahlungsleistung beträgt: $P_\mathrm{ERP}$* → "The effective radiated power is" (the symbol decides, DECISIONS.md, AK115).
- slides: *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", *Bonusfrage* → "Bonus question", as in earlier units; *Gilt nur im Freiraum* → "Only valid in free space".
- slides/naeherungsformel_2: *effektive isotrope Strahlungsleistung (EIRP)* → "equivalent isotropically radiated power (EIRP)": the abbreviation decides (DECISIONS.md; see errors); note *für Amateurfunk relevant nur ATV … und SATV* → "the only ones relevant to amateur radio are ATV … and SATV".
- Decimal commas in formulas, including `0{,}25` → `0{.}25` and bare `1,64` → `1.64`, as earlier units.

## Suspected errors in the German original

- sections/naeherungsformel_2.md — "Dabei bezeichnet $Z_0$ den Feldwellenwiderstand des freien Raums. … nähert sich dieser mit zunehmendem Abstand von der Antenne dem Fernfeldwert $Z_0 \approx 120\pi\,\Omega$ an": $Z_0$ is itself the constant far-field value; what approaches it with distance is the distance-dependent wave impedance $Z_\mathrm{F}(d)$ of the nahfeld section. Translated as written.
- slides/personenschutzabstand_3.md — the solution slide after `[question:AK114]` is a copy of the one after AK115 ($P_\mathrm{ERP} = 100$ W, $d = 100$ m, 0.7 V/m); AK114 is a dipole fed with 10 W at 10 m, answer 2.2 V/m (solution AK114). Translated as written.
- slides/naeherungsformel_2.md — "die effektive isotrope Strahlungsleistung (EIRP)": mixes *effektive* (ERP) with *isotrope* (EIRP); the formula that follows is the EIRP. Written as EIRP.
- solutions/AK106–AK112 — the transmitter power is written $P_\mathrm{ERP}$ ("Die Sendeleistung beträgt 100 Watt: $P_\mathrm{ERP} = 100$ W", AK106) and the formula $P_\mathrm{EIRP} = P_\mathrm{ERP} \cdot 10^{(g-a)/10}$ is introduced as the "Leistungszusammenhang EIRP und ERP", although the power in it is the transmitter output (AK107's result is "die maximale Ausgangsleistung des Senders"; AK113 writes $P_S$ under the same heading). Translated as written.
- solutions/AK113.md — step "2. Berechnung von $d$" calculates $E$; the data list numbers "3." twice. Translated as written.
- solutions/AK105.md — "$\qty{-6}{\dB}$-Dämpfung": an attenuation of −6 dB would be a gain; either −6 dB or an attenuation of 6 dB. Translated as written.
- sections/naeherungsformel_1.md — `$\qty{1,5}{dB}$` without backslash, so the unit is not typeset as the dB symbol (left unchanged); "plus der Gewinn von 2,15 dBi für den isotropen Strahler": the 2.15 dBi is the dipole's gain over the isotropic radiator (rendered as described above).
- Typos with no effect on the English: sections/naeherungsformel_1.md "zu Berechnen" (*berechnen*), "Wir finden Sie" (*sie*), "Das Fernfeld einer Strahlungsquelle, ist" (stray comma) and "($E$), der magnetischen" (*und* missing), "können wir … ermittelt werden" (mixed construction), "wenn der er", "Das wie oben schnell geprüft werden" (*kann* missing); sections/personenschutzabstand_richtantennen.md "über den … Bereich hinweg, also dem Bereich" (*den*), "halbiert sich … auf die Hälfte" (redundant); sections/personenschutzabstand_3.md "wird Leistung am Speisepunkt …, der Gewinnfaktor und die Entfernung gebraucht" (*werden*, article missing); solutions AK106–AK113 "Lösungschritte" (*Lösungsschritte*); AK105 "vom vorgegeben Wert" (*vorgegebenen*), 'im Kapitel "Strahlungsleistung und Gewinn" von Antennen' (*von Antennen* outside the quoted name); AK106 "das $\qty{10}{\meter}$ Band" (hyphen); slides/naeherungsformel_2.md "Sicherheitsabstandberechnung" (*Sicherheitsabstandsberechnung*).

## Provjera

All 19 files compared paragraph by paragraph with the German of
`a6a8a6e~1`; the embedded questions (EK105, EK106, EK108, AK102–AK115)
looked up in English. The translation is complete and faithful, the
calculations and every number match, and the prose follows the questions'
wording ("far-field approximation formula", "reactive near field",
"measurements of the E- and H-field components, simulations or near-field
calculations", "limit for the protection of persons", "area that is not
controllable", "critical angle", "direction of maximum radiation",
"effective radiated power (ERP)").

Changes: omission 0, meaning 1, technical 0, style 5, glossary 0.

- slides/naeherungsformel_1.md (meaning): the EK105 slide note *Liegt im
  Nahfeld, was wir vorher ausgerechnet haben* said "It lies in the near
  field, as we calculated before"; the German says that what we calculated
  before lies in the near field — now "What we calculated before lies in
  the near field".
- slides/naeherungsformel_1.md (style): bonus question "Is the calculated
  5 m not in the near field …?" → "Isn't the calculated 5 m in the near
  field …?", the natural English form of the negative question.
- sections/naeherungsformel_1.md (style): "We find it on the formula sheet"
  → "We can find it …"; "plus the gain of 2.15 dBi for referring it to the
  isotropic radiator" → "… to refer it to the isotropic radiator" (the
  translator's judgement call kept, wording smoothed).
- sections/naeherungsformel_2.md (style): "on the form of the antenna" →
  "on the type of antenna", as the same section says "many types of
  antenna" for *Antennenformen*.
- sections/personenschutzabstand_richtantennen.md (style): "The most power
  is radiated" → "Most power is radiated".

The 12 glossary rows are kept: they follow §1.4, §9 and §14 and the wording
of EK105, EK106, AK102 and AK105. No DECISIONS.md entry was needed, and the
other judgement calls are kept — *Faktor_FmodPers* as a symbol, "impedance
of free space" for $Z_0$ with its slip translated as written, EIRP for
*effektive isotrope Strahlungsleistung (EIRP)* by the existing decision,
"effective radiated power" in AK115, the solution headings, and "an
attenuation of −6 dB" in AK105 as the German writes it. The suspected
errors in the German, among them the AK114 slide copied from AK115, are
confirmed and stay listed for DARC.

`revizija-guard.py --rev a6a8a6e~1 --brojevi`: 19 files, *struktura netaknuta*.
