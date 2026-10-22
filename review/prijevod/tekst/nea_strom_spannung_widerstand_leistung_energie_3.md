# nea_strom_spannung_widerstand_leistung_energie_3 — translation report

Chapter "Strom, Spannung, Widerstand, Leistung, Energie (3/3)" (Current,
voltage, resistance, power, energy, part 3): 5 sections, each with its
slides, and 16 solutions. 26 files:

- `contents/sections/` and `contents/slides/`: `leistung_2.md`,
  `dezibel_1.md`, `dezibel_2.md`, `ladung_energie.md`, `bauelemente.md`.
- `contents/solutions/`: `AA102.md`, `AA103.md`, `AA105.md`–`AA112.md`
  (no AA104), `AB502.md`, `AB503.md`, `AD426.md`, `AD427.md`, `AD428.md`,
  `AF428.md`.

`revizija-guard.py --brojevi`: 26 files checked, *struktura netaknuta*.
German-word grep: no hits outside the formula subscripts
`g_\text{Verstärkung}`, `p_\text{Eingang}`, `p_\text{Ausgang}` (AA107,
AA109; also `p_\text{Sender, Ausgang}`, `g_\text{Endstufe}`), which stay
German.

Embedded questions looked up in English and the prose aligned with them:
EB503–EB514, EA107, AA102, AA103, AA105–AA112, AB502, AB503, AD426–AD428,
AF428, NC201, NC301, NC501, NB202.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

22 rows: *Leistungsfaktor / Verhältnisfaktor* (dB context → power ratio /
ratio), *Logarithmieren / Potenzieren*, *Zehnerlogarithmus*, *Eulersche
Zahl*, *Bel* as a table column, *Hilfsmaßeinheit / Pseudoeinheit*,
*(Dezibel) bezogen auf / Bezugswert*, *Signalkette*, *Referenzstrahler*,
*vorzeichenrichtige Subtraktion*, *Hilfsmittel* (examination),
*Gegeben / Lösungsweg / Abkürzung* as solution headings, the formula
sheet's section names, *Energiegehalt*, *Stromrechnung / Stromverbrauch*,
*Zimmerlautstärke*, *Handfunke*, *effektive Leistung* of an EME station,
*frequenzerzeugende Stufe*, *Gehörlosenlehrer*, *Bauformen* in the
component photos, *Strom/Leistung über Zeit* (slides).

## Added to `DECISIONS.md`

Nothing: every choice here is a single term (glossary) or follows an
existing rule (word subscripts, units after a number, *Figure* before a
reference, *chassis* / *earth*).

## Judgement calls

- dezibel_1, dezibel_2 (sections, slides, tables): *Leistungsfaktor* → "power ratio", *Verhältnisfaktor* / *Verhältniswert* → "ratio": English *power factor* is cos φ, and the questions already write "(as a power ratio)"; table headers "≈ Power ratio", "≈ Voltage ratio", captions "Important power ratios in dB".
- dezibel_1: *Zehnerlogarithmen* (bracket after *dekadischer Logarithmus*) → "base-ten logarithm", an alternative English name as the German gives an alternative German one; *technisch-wissenschaftlicher Taschenrechner* → "scientific calculator" (glossary); `\text{Nullen}`, `\text{Verhältnisfaktor}` → `\text{zeros}`, `\text{ratio}` (running words in `\text{}`).
- dezibel_1 slides: *effektive Leistung EME-Station* (100 kW) → "Effective radiated power, EME station" — the figure includes antenna gain; *RMS power* (§11) would be the wrong sense; *Lautes / Leises KW-Signal* → "Loud / Quiet HF signal" (KW → HF, *laut / leise* kept apart from *stark / schwach*); *Zimmerlautstärke* → "normal room volume"; column "Bel" → "Bels"; *dezi wie in dezimeter* → "deci as in decimetre"; calculator keys "*log* key", "*=* key".
- dezibel_2: *Achtung, hier ist … gemeint* → "Note: what is meant here is …"; *Lektion* → "lesson"; *Versuche … mit deinem Wissen zu lösen* → "Try to solve the question with what you know"; slides *liegt bei P = 1 mW vor* → "corresponds to P = 1 mW"; `\text{Faktor 10}` → `\text{factor 10}`.
- leistung_2: `\text{ bzw. }` → `\text{ or }`; *Abschlusswiderstand* → "terminating resistor" (§11), *reiner Wirkwiderstand* → "pure resistance"; *effektive Leistung* (EB513) → "RMS power" (§11, AI105); EB513's missing full stop after "12.5 V" supplied; *Hochfrequenz – also der Wechselspannung* → "radio frequency – that is, of AC voltage".
- ladung_energie: *Akkus oder Batterien* → "batteries or rechargeable batteries", *Batterien und Akkumulatoren* → "batteries and rechargeable batteries" (glossary *Akku*); *Energie pro Zeit* → "energy per unit time"; slides *Strom über Zeit / Leistung über Zeit* → "Current times time / Power times time" ("over time" would read as division beside $Q = I\cdot t$); the garbled *in Joule (J) auf Sekunde bezogen* → "in joules (J), with time in seconds" (checker; first "based on the second").
- bauelemente: *Spule* → "inductor" (NC301); *Schaltzeichen und Bauformen* → "Circuit symbol and types of …" (not *package style*, which suits semiconductors but not inductors); slides *Masse* → "Chassis" (NB202, glossary §4), *Nicht zu verwechseln mit der Erdung* → "Not to be confused with earthing"; *Klasse E und A* → "Classes E and A".
- Solutions: headings *Gegeben / Lösungsweg / Abkürzung* → "Given / Solution / Shortcut" (*Abkürzung* here is a short cut, not an abbreviation); the formula-sheet section names in brackets → "(levels, gain, power)", "(levels, power and voltage levels)", lower case as descriptions; *Hilfsmittel* → "examination aids"; *Eingangsleitung* (typo, AA106, AA107) → "Input power".
- AB503: the label *Strom:* before $R = 100 Ω$ translated faithfully as "Current:" (see errors below).
- AA107 shortcut: *Damit entspricht der Ausgangspegel genau der Verstärkung von 10 dBW* → "The output level is then exactly the gain, at 10 dBW", keeping the German's dBW (see errors).
- AD426: *HF-Ausgangsleistung* → "RF output power" (as the question).

## Suspected errors in the German original

- sections/dezibel_2.md, table a_spannungsverhaeltnisse — the row for 3 dB gives a voltage ratio of 1,14; it should be 1,41 (√2, as the power table's 1.5 dB row). Translated as written ("1.14").
- solutions/AB503.md — "Strom: $R = \qty{100}{\ohm}$": the label should be *Widerstand*. Translated faithfully ("Current:").
- solutions/AA107.md — shortcut: "der Verstärkung von $\qty{10}{\dBW}$": a gain is in dB, not dBW (the solution above it writes 10 dB). Translated faithfully.
- sections/dezibel_2.md (indepth) — asks why one may subtract 3 dB from a level of 9 dBm, but no such example appears in the text (the signal chains use 10 dBm, −10 dBm and a 20 dB attenuator).
- sections/ladung_energie.md — "Die folgenden beiden Prüfungsfragen betrachten genau dieses Szenario" (a resistor with a voltage across it): that is true of AB503, but AB502 is a power supply drawing 0.63 A at 230 V.
- sections/ladung_energie.md — "$\qty{3000}{\milli\ampere\hour} \cdot \qty{3,6}{\volt} = \qty{10.8}{\watt\hour}$": the product is 10 800 mWh; the result is right, but the equation skips the conversion.
- slides/dezibel_1.md — the third table (with the dBm column) repeats the ident and caption of the second, `e_dezibel_leistungen_bel` "Leistungen in mW und Bel".
- sections/dezibel_2.md — the voltage derivation uses $P_1/P_2$ where the power formula above uses $P_2/P_1$, and the text after it calls the ratio *$a$* while the formula names it $g$.
- solutions/AA109.md — the given values are named $p_\text{Sender, Ausgang}$ and $g_\text{Endstufe}$, the final step uses $p_\text{Eingang}$ and $g_\text{Verstärkung}$; "$10 \cdot \qty{3}{\dBm}$" puts a unit on a logarithm. Likewise solutions/AA111.md "$20 \cdot \qty{1.176}{\dB}$" (log 15 has no unit).
- slides/ladung_energie.md — "in Joule ($\unit{\joule}$) auf Sekunde bezogen" is garbled (probably *Wattsekunden*); translated by its evident meaning.
- Typos with no effect on the English: sections/dezibel_2.md and slides captions "Signalkette mit drei/zwei Verstärken" (*Verstärkern*), "können wir das Dezibel können auch verwenden" (verb twice), "schonmal", "Wieviel"; sections/leistung_2.md "Im letzen Schritt", "Das bedeutet die Spitzenspannung beträgt $\hat{U} = \qty{12,5}{\volt}$ Wir" (full stop missing); solutions/AA106.md and AA107.md "Eingangsleitung" (*Eingangsleistung*); AA107.md, AA109.md "durch einfach Addition" (*einfache*); AA108.md–AA110.md "aus den Hilfsmittel" (*Hilfsmitteln*); AA110.md "Wir setzten" (*setzen*).

## Provjera

Checker, 2026-10-22: all 26 files compared with the German of `00b4eb0~1`
line by line; embedded questions (EB503–EB514, EA107, AA102–AA112, AB502,
AB503, AD426–AD428, AF428, NB202, NC201, NC301, NC501) read in English. The
translation is complete and the numbers, formulas and markup are intact;
`revizija-guard.py --rev 00b4eb0~1 --brojevi`: 26 files, *struktura
netaknuta*. All judgement calls, the 22 glossary rows and the suspected
errors in the German are kept (the *Bel*, *effektive Leistung EME-Station*,
*Strom über Zeit* and *Bauformen* choices checked and found sound); one
glossary row added.

Changes: omission 0, meaning 1, technical 0, style 8, glossary 4.

- slides/ladung_energie.md: *in Joule auf Sekunde bezogen* "based on the second" → "with time in seconds" — the evident meaning (J = W·s against W·h); "based on the second" said nothing to an English reader (meaning).
- sections/dezibel_1.md, dezibel_2.md (3×): *Zusatz* to dB (dBm, dBi, dBd) "addition" → "suffix", the English word for it; glossary §14 row *Zusatz (an dB)* → suffix added (glossary).
- sections/dezibel_2.md indepth: "The bel and the decibel are an auxiliary unit (also called a pseudo-unit)" → "are auxiliary units (also called pseudo-units)"; "Why is it allowed" → "Why is it permissible" (style).
- sections/dezibel_2.md: *grundsätzlich* "basically" → "fundamentally"; *messen wir gern* "we like to measure" → "we usually measure" (style).
- sections/leistung_2.md (EB508): "When the current is known, too, the power can be calculated, with …" → "The power can also be calculated when the current is known, with …" (style).
- slides/dezibel_1.md: "not relative to the mW" → "not relative to mW"; slides/bauelemente.md: "In the simple cases" → "In simple cases"; solutions/AA107.md: the full sentence in brackets starts with a capital (style).

