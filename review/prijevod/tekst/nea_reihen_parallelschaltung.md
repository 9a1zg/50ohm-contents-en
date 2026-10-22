# nea_reihen_parallelschaltung — translation report

Chapter "Reihen- und Parallelschaltung von Bauelementen" (Series and
parallel connection of components): 9 sections, each with its slides, and
15 solutions. 33 files:

- `contents/sections/` and `contents/slides/`: `reihe_parallel_widerstand.md`,
  `reihe_parallel_widerstandsnetz_1.md`, `reihe_parallel_widerstandsnetz_2.md`,
  `spannungsteiler_1.md`, `spannungsteiler_2.md`, `brueckenschaltung.md`,
  `reihe_parallel_kondensator.md`, `reihenschaltung_spule.md`,
  `reihe_parallel_gemischt.md`.
- `contents/solutions/`: `AD101.md`–`AD115.md`.

`revizija-guard.py --brojevi`: 33 files checked, *struktura netaknuta*.
German-word grep: no hits outside `%` comments (left in German, as markup),
picture idents (`E 63. Spannungsteiler`, `a_Brückenschaltung`,
`a_Spule mit Anzapfungen`, `a_Netzteil BEKO PA …`), the subscripts
`R_\mathrm{ges}`, `C_\mathrm{Spule}` and the German word *Scheinwiderstand*
named on purpose.

Embedded questions looked up in English and the prose aligned with them:
ED101–ED124, AD101–AD115 (e.g. ED101's "How is the voltage divided between
two resistors connected in series …" quoted in spannungsteiler_1; AD111
"bridge diagonal"; AD115 "converts more power into heat").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

22 rows: *Ersatzwiderstand / Widerstandsnetzwerk*, *hintereinander
geschaltet*, *Bruchrechnung*, *Methode des scharfen Hinsehens* (solving by
inspection), *gemischte Schaltung(en)* (series-parallel circuits), the
*Variante 1 / 2* slide headings, *Gesamt- / Einzelbelastbarkeit*,
*Teilströme* (branch currents), *Grenzfall / Schleifer*, *Maschenregel /
Knotenregel / Kirchhoff'sche Gesetze* (loop rule / junction rule),
*Spannungsteilerverhältnis* (divider ratio), *abgeglichene Brücke /
Brückenspannung*, *Wheatstone-Messbrücke / Widerstandsmessbrücke*,
*Messwerk* (meter movement), *Multiplikator / Messbereichsmultiplikator /
Großer Drehknopf*, *Messpunkt*, *Durchschlag*, *Vorsilbe*,
*Endstufennetzteil*, *Teilabschnitte (zwischen Anzapfungen)*, *komplexe
Größe / Real- / Imaginärteil / komplexe Ebene*, *Wirkwiderstand* beside
*Blind-* and *Scheinwiderstand*.

## Added to `DECISIONS.md`

None. The *Scheinwiderstand* naming follows the existing glossary row (§14,
from nea_bauelemente_1); everything else is a single term.

## Judgement calls

- All files: *Spannungsteiler* → potential divider (glossary §5), *unbelastet / belastet* → unloaded / loaded; *Lösungsweg / gegeben / gesucht* → "Solution / given / required", *Formelsammlung* → formula sheet, as in earlier units.
- reihe_parallel_widerstand, reihe_parallel_kondensator: *Gemischte Schaltung(en)* → "series-parallel circuit(s)", the English textbook term for both variants, rather than "mixed circuits"; *gemischte Schaltungstechnik* → "series-parallel combinations".
- reihe_parallel_widerstand: *"Methode des scharfen Hinsehens"* → "solving by inspection", the established English phrase for the same thing; a literal "method of sharp looking" means nothing in English.
- reihe_parallel_widerstand: *"Widerstands-Normreihe"* → the so-called "preferred-value series" for resistors (glossary §4); slides *Normreihe* (capacitors) → "the preferred values".
- reihe_parallel_widerstand slides: *Bei einer Reihenschaltung teilen sich die Spannungen auf* → "the voltage divides", *Ströme* → "the current divides" (singular, as English says it).
- reihe_parallel_widerstandsnetz_2 slides: *Maschen- und Knotenregel* → "Loop rule and junction rule", note *Kirchhoff'sche Gesetze* → "Kirchhoff's laws".
- reihe_parallel_widerstandsnetz_2, brueckenschaltung: *Wheatstone Messbrücke / Wheatstone-Messbrücke* and slide note *Messbrücke nach Wheatstone* → "Wheatstone bridge"; photo caption *Widerstandsmessbrücke nach Wheatstone (Pontavi)* → "Wheatstone resistance measuring bridge (Pontavi)".
- brueckenschaltung: *Messwerk* → "meter movement"; *Messbereichsmultiplikator* → "range multiplier"; *den Großen Drehknopf* → "the large knob" (German capital not carried over); *in der nebenstehenden Vertiefung* → "in the *In depth* box alongside".
- brueckenschaltung, AD113: *gegen Masse gemessen* → "measured with respect to chassis" (glossary §14 *gegen Masse*); *Betriebsspannung* → operating voltage (glossary §5).
- spannungsteiler_1: *5-mal größer* → "5 times as large"; *6-mal kleiner* → "smaller … by a factor of 6" (keeps the digit and avoids "6 times smaller"); *hochohmig / niederohmig* → "of high / low resistance".
- spannungsteiler_1: the German ".:" after *Formelsammlung finden* and the stray space in *Wortwahl :* not carried over.
- spannungsteiler_2 slides: *Voraussetzung: Strom der Versorgung bricht nicht ein* → "Assumption: the supply current does not collapse", as written (see errors); *Bei der Dimensionierung* → "When choosing the values" (as the checker of nea_bauelemente_2).
- reihe_parallel_kondensator: photo caption *Parallelschaltung von 7 × 10000 µF in einem Endstufennetzteil* → "7 × 10000 µF connected in parallel in the power supply of a power amplifier".
- reihe_parallel_kondensator slides: *entscheidend für das Entstehen / die Entstehung des elektrischen Feldes* → "what determines how the electric field builds up".
- reihenschaltung_spule: *Bei einer Spule in Reihenschaltung* → "When inductors are connected in series" (plural, the evident meaning); *Spule* → inductor for the component, coil for the winding (glossary §4); *selbstgebautes Antennenanpassgerät* → "home-built antenna tuning unit".
- reihe_parallel_gemischt: *Der normale ohmsche Widerstand wird als Wirkwiderstand R bezeichnet* → "is called the resistive part, or simply the resistance $R$"; *Scheinwiderstand $|Z|$* → "the impedance $|Z|$ (in German *Scheinwiderstand*)", the German word named once as in kondensator_2 / spule_2; *Wechselstromwiderstand* → "AC resistance".
- reihe_parallel_gemischt slides: *Wicklungskapazität* → inter-winding capacitance, note *Eigenkapazität einer Spule* → "Self-capacitance of an inductor" (glossary §14, AD103).
- AD101: the decimal commas in `0{,}01` … written `0{.}01`, so the guard still sees the same digit groups and LaTeX renders a point.
- AD115: *mehr Leistung in Wärme umgesetzt* → "more power is converted into heat", the wording of the question's answers.

## Suspected errors in the German original

- slides/reihe_parallel_gemischt.md (AD104) — "gegeben: $C = \qty{100}{\nano\farad}$" and 100 nF in the formula, while the question has 1 nF and the result 159 Ω is for 1 nF (100 nF gives 1.59 Ω). Translated as written.
- slides/reihe_parallel_gemischt.md (AD103) — the note "Einheitenpräfixe beachten und mit Kehrwerten rechnen": AD103 is a parallel connection whose capacitances are simply added; the reciprocals belong to AD101.
- slides/reihe_parallel_kondensator.md, Variante 2 — "Danach berechnet man die Parallelschaltung von $C_3$ und $C_{ges,r}$" with the product-over-sum formula: capacitances in parallel add ($C_{ges} = C_3 + C_{ges,r}$). Variante 1 writes $C_{Gp}$ in the denominator for $C_{\mathrm{ges,p}}$.
- slides/spannungsteiler_2.md — "$P_1 = U_1 \cdot I_1 = I_2 \cdot R_1$": should be ${I_1}^2 \cdot R_1$ (the next two lines have the squares).
- slides/spannungsteiler_2.md — "Voraussetzung: Strom der Versorgung bricht nicht ein": evidently the supply *voltage* must not collapse (a stiff source); with a falling load resistance the supply current rises, as the line above says.
- sections/reihe_parallel_widerstandsnetz_2.md (tip on AD110) — "$R_1 || R_2 = \qty{1100}{\ohm}$ sowie $R_3 || R_4 = \qty{110}{\ohm}$": with the question's values ($R_1 = R_3 = 2.2$ kΩ, $R_2 = R_4 = 220$ Ω) the pairs are $R_1 || R_3$ and $R_2 || R_4$, as the slides and solution AD110 say.
- slides/brueckenschaltung.md (AD113) — $U_A = \frac{R_1}{R_1+R_2} \cdot U = 1$ V is the voltage across $R_1$, not the potential of A, which the section and solution AD113 give as 10 V (across $R_2$, to chassis); the slide then takes $U_{AB} = U_B - U_A$. The 9 V agrees, the derivation contradicts the section.
- sections/reihe_parallel_kondensator.md — "Bei einer Parallelschaltung von gleich großen Kondensatoren verdoppelt sich die Kapazität": only for two capacitors (n equal capacitors give n times). The tip "immer größer als die kleinste Einzelkapazität" is true but weak: the total is greater than the *largest* (the mirror of the series tip).
- sections/reihe_parallel_kondensator.md — the series picture 823 has the same ident `e_3C-parallel` as the parallel picture 822, so "[ref:e_3C-parallel]" in "Bei einer Reihenschaltung …, wie in Abbildung … gezeigt" is ambiguous (the slides give 823 the ident `e_reihenschaltung_kondensatoren`).
- sections/reihe_parallel_kondensator.md, `%` comment — "*ED 118:* Reihenschaltung von …": ED118 is a parallel connection (not rendered).
- sections/spannungsteiler_2.md — "${32}{\milli\watt}$" lacks `\qty`, so it does not render as 32 mW. Kept as markup.
- solutions/AD114.md — "$… = \approx \qty{1,8}{\volt}$": stray "=" before "≈". Kept.
- sections/reihe_parallel_gemischt.md — the introduction announces "die Parallelschaltung von Spulen und Kondensatoren", but the section then covers capacitors in parallel and series and the impedance of series R–C and R–L circuits; no parallel L–C circuit is calculated.
- sections/reihenschaltung_spule.md and slides — "Bei einer Spule in Reihenschaltung addieren sich die Induktivitäten": *Spulen* meant.
- Typos with no effect on the English: sections/reihe_parallel_widerstand.md "Paralelschaltungen", "Sie vom gleichen Strom … durchflossen" (verb missing), "die Wert des Gesamtwiderstands", "der Strom teil sich", "das dreifache", "am Besten", "je nach dem"; sections/reihe_parallel_widerstandsnetz_2.md "wird er Gesamtwiderstand", "Wheatstone Messbrücke"; sections/spannungsteiler_1.md "finden.:", "Wortwahl :", "Das Schauen wir uns"; sections/spannungsteiler_2.md "exisiert", "eines Spannungsteiler"; sections/brueckenschaltung.md "verinfachten", "Großen Drehknopf", "Multiplikator der Werte" (comma missing); sections/reihe_parallel_kondensator.md "Widerstanden"; sections/reihenschaltung_spule.md "Spulten"; sections/reihe_parallel_gemischt.md "gelenrt"; solutions/AD111.md "(Unbelastet)".

## Provjera

All 33 files compared with the German (`a5fe954~1`) paragraph by paragraph,
embedded questions ED101–ED124 and AD101–AD115 looked up in English. Nothing
dropped or added; numbers, formulas and markup intact (`revizija-guard.py
--rev a5fe954~1 --brojevi`: 33 files, *struktura netaknuta*). The 22 glossary
rows are kept (one note reworded, below); no DECISIONS.md entry was needed.
All judgement calls are kept except where changed below; the list of
suspected errors in the German stands as written.

Changes: omission 0, meaning 0, technical 1, style 5, glossary 1.

- Technical — sections/reihe_parallel_gemischt.md: *Scheinwiderstand $|Z|$* was "called the impedance $|Z|$", two sentences before "the letter $Z$ is used for … the impedance"; now "the magnitude of the impedance, $|Z|$, which German calls the *Scheinwiderstand*", as kondensator_2 / spule_2 and the wording of AD104/AD105 ("the magnitude of the impedance $Z$"); the picture caption, the Pythagoras sentence and the AD105 lead-in follow.
- Glossary — §14 row *Wirkwiderstand* (from this unit): its note on *Scheinwiderstand* updated to the wording above.
- Style — reihe_parallel_gemischt: "reactances, as we have already met them with …" (German word order) → "reactances, which we have already met with …".
- Style — slides/reihe_parallel_kondensator: *entscheidend für das Entstehen des elektrischen Feldes* "what determines how the electric field builds up" → "it is the voltage that sets up the electric field" (twice); "to get from the preferred values to the value you need" → "to make up the value you need from the preferred values".
- Style — spannungsteiler_1: *hochohmig / niederohmig* "a resistor of high / low resistance" → "a high-value / low-value resistor".
- Style — reihe_parallel_widerstand: "An important method of solution is "solving by inspection"" → "An important technique is …"; "networks in which there is both a series and a parallel connection" → "networks with both …"; slide heading "… in series and parallel connection" → "… connected in series and in parallel".
- Style — AD115: *der untere Teilwiderstand* "the lower resistance of the potential divider" → "the resistance of the lower part of the potential divider".
