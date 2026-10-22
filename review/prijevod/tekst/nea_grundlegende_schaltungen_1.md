# nea_grundlegende_schaltungen_1 — translation report

Chapter "Grundlegende Schaltungen (1/3)" (Basic circuits, part 1): 6 sections,
each with its slides, and 10 solutions. 22 files:

- `contents/sections/` and `contents/slides/`: `schwingkreis_1.md`,
  `schwingkreis_2.md`, `oszillatoren.md`, `oszillator_vco.md`,
  `oszillator_tcxo_ocxo.md`, `oszillator_gpsdo.md`.
- `contents/solutions/`: `AD201.md`, `AD202.md`, `AD203.md`, `AD208.md`–`AD212.md`,
  `AD224.md`, `AD225.md`.

`revizija-guard.py --brojevi`: 22 files checked, *struktura netaknuta*.
German-word grep: no hits outside picture idents (`e_frequenzabhängiger_widerstand`,
`a_vco_schaltung` …), the `[include:applet_schwingkreis]` target, the two
commented-out picture lines in slides/schwingkreis_1.md (`%`, left in German
as markup), and the German words named on purpose (*Schwingkreis*,
*Schwingkreise*, *Leitkreis*, *Reihenschwingkreis* / *Serienschwingkreis*,
*Quarz*). Line counts and final-newline state are the same as in the German.

Embedded questions looked up in English and the prose aligned with them:
ED201–ED216, AD201–AD229, AD601–AD606, AD611, ED501–ED507, EF207, EF304,
AF215 (e.g. ED214/ED215 "rejector circuit" / "acceptor circuit", ED216
"ceramic or air-spaced capacitors", AD205 "band-pass filter", AD213–AD217
"push the turns of the coil closer together", "insert a ferrite core",
AD220 "0.7 times the maximum voltage", AD229 "critical coupling", AD601
"voltage-controlled oscillator", AD602 "temperature-compensated crystal
oscillator", AD611 "frequency instability", AF215 "thermally insulated as
well as possible", EF207 "screened by a metal case").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

23 rows: *RC-Glied / RL-Glied / LC-Glied* (RC / RL / LC network), *Flanken
(Filter)*, *Frequenzweiche / Antennenweiche* (frequency splitter / antenna
splitter), *Duoband-Antenne / UKW-Duoband-Gerät*, *Direktfunk / Relaisfunk*,
*Bauvorschlag / Berechnungsprogramm*, *Stimmgabel / Rechteckimpuls*,
*Serienschwingkreis bzw. Reihenschwingkreis*, the *Schwingkreis* naming
sentence, *Betragsfrequenzgang* (magnitude response), *Thomsonsche
Schwingungsformel / Schwingkreisformel* (Thomson's formula), *Güte (im
Englischen Q-Faktor)*, *unterkritische Kopplung / Durchlassbereich / Delle*,
*Schwingquarz / Quarz*, *Wirkkette*, *Frequenzabweichung / Sollfrequenz*
(frequency error / nominal frequency), *geregelte Heizung*,
*Rubidium-Frequenznormal*, *GNSS*, *GPSDO*, *Kurzzeitstabilität / Alterung*,
*ein Impuls pro Sekunde*, *Mit eingesetzten Werten:*.

Corrected: the existing row *Leitkreis* said "coupled-circuit band-pass
filter"; no translated text used it, and drawing 1039 shows a series LC
circuit in series with the signal path, not coupled circuits. Now "series
pass circuit (*Leitkreis*)" with the reason.

## Added to `DECISIONS.md`

None. The choices of note (the *Schwingkreis* gloss, *Leitkreis*, the
*Quartz* slide note) apply existing rules (the *Scheinwiderstand* naming,
the bracket rule, the *Relais / Repeater* rule) and are recorded in their
glossary rows.

## Judgement calls

- All files: *Schwingkreis* → tuned circuit, *Reihen- / Serienschwingkreis* → series tuned circuit, *Parallelschwingkreis* → parallel tuned circuit, *Saugkreis / Sperrkreis* → acceptor / rejector circuit, *Hochpass / Tiefpass / Bandpass / Bandsperre* → high-pass / low-pass / band-pass / band-stop filter, *Grenzfrequenz* → cut-off frequency, *Güte / Gütefaktor* → Q factor, *Kapazitätsdiode* → varactor diode, *Spannungsteiler* → potential divider (glossary §4, §5; ED2xx, AD2xx).
- schwingkreis_1: the German calls the frequency-dependent opposition of a capacitor or inductor its *Widerstand*; kept as "resistance", as kondensator_2 did ("behaves like a frequency-dependent resistance"), and *Widerstand* the component → resistor.
- schwingkreis_1: *Aus diesem Grund spricht man von einem Schwingkreis* → "This is why it is called a tuned circuit (in German *Schwingkreis*, literally "oscillating circuit")": the sentence argues from the German word; "tuned circuit" alone would lose the point.
- schwingkreis_1: *Leitkreis* → "series pass circuit (in German *Leitkreis*, …)", caption "series pass circuit": English has no established name for this topology (see glossary).
- schwingkreis_1: "Der Frequenzgang eines Hochpasses ist qualitativ in [ref:e_hochpass_frequenzgang] gezeigt" → "… in Figure [ref:…]": the German leaves out *Abbildung*; the reference renders as a bare number.
- schwingkreis_1: the *H* memory aid works in English as in German: "an upright *H* – as in *H*igh-pass".
- schwingkreis_1: *Antennenweiche* → "antenna splitter", *Frequenzweichen* → "frequency splitters"; *UKW-Empfänger* → "VHF receiver"; *UKW-Radiosender* → "VHF FM broadcast transmitter" (glossary §10 *UKW-Rundfunk*); *UKW-Duoband-Gerät* → "VHF/UHF dual-band radio", since the 70 cm band it also covers is UHF in English.
- schwingkreis_1: in the LC oscillation paragraph, *Das Magnetfeld der Spule entlädt sich / ist abgebaut* → "collapses / has collapsed", the English idiom for a magnetic field; the capacitor still "discharges".
- schwingkreis_1: *Ein Serienschwingkreis seriell im Signalweg* / *parallel am Signalweg* → "in series in the signal path" / "in parallel across it".
- schwingkreis_2: *Die Güte eines Schwingkreises (im Englischen Q-Faktor)* → "The Q factor of a tuned circuit": the bracket only gives the English term (bracket rule); slide bullet *Auch Q-Faktor* → "Also called the quality factor", so the bullet keeps a job.
- schwingkreis_2: *In der Formelsammlung finden wir sie beim Thema "Schwingkreise"* → "under the topic "tuned circuits" (*Schwingkreise*)", the formula-sheet rule (DECISIONS.md).
- schwingkreis_2: *Diese Kopplung kann je nach Anwendung … erfolgen* → "this coupling can be … (a)." — the verb at the end of the German list moved before it; *unterkritisch* → under-critical, beside the glossary's loose / critical / over-critical; *Durchlassdämpfung* → passband loss; *Durchlasskurve* → passband curve (glossary §5, §6).
- schwingkreis_2: `0{,}707`, `0{,}7` → `0{.}707`, `0{.}7`, as in earlier units.
- slides/schwingkreis_2: *Oder Serienschwingkreis* → "Called *Reihenschwingkreis* or *Serienschwingkreis* in German", as the *Relais / Repeater* sentence in relaisfunkstellen: English has one term, and the bullet would otherwise repeat the heading. *Resonanzfall* (heading) → "Resonance".
- slides/oszillatoren: note *Im Englischen mit t: Quartz* → "In German spelt without the t: Quarz", the mirror of the German remark, so the note keeps information instead of being emptied.
- oszillatoren: *Schwingquarz* → crystal (glossary §4 *Quarz*); the slide's *Quarz (Siliziumdioxid $SiO_2$)* is the material → "quartz crystal".
- oszillator_vco: *spannungsgesteuerte Oszillator VCO - Voltage controlled oscillator* → "voltage-controlled oscillator (VCO)": the German pairs the German and English names, which are one in English. *Grenzschicht* → junction (glossary §4), "the width of the junction", "widens / narrows".
- oszillator_tcxo_ocxo, oszillator_gpsdo: *Frequenzabweichung* → frequency error, not "deviation" (FM *Hub*); *Sollfrequenz* → nominal frequency; *Wandern* → drift; *3 cm-Band bzw. 10 GHz-Band* → "the 3 cm band, i.e. the 10 GHz band"; *RC-, LC- oder VCO-Oszillator* → "an RC oscillator, LC oscillator or VCO".
- oszillator_tcxo_ocxo: the English expansions of XO, TCXO, OCXO written in lower case and hyphenated as AD602 does ("temperature-compensated crystal oscillator"); the slide's German spelling *Oszillator* in "Oven Controlled Crystal Oszillator" not carried over.
- oszillator_gpsdo: *Satellitennavigationssysteme, englisch Global Navigation Satellite Systems (GNSS)* → "global navigation satellite systems (GNSS)" and *GPS-synchronisierter Oszillator oder englisch als GPS-Disciplined Oscillator (GPSDO)* → "GPS-disciplined oscillator (GPSDO)" (bracket rule); *Funkverbindung auf einer fest vereinbarten Frequenz* → "a contact on a pre-arranged frequency"; *Empfangsbereich* → "receive passband" (the SSB filter of the sentence before).
- Solutions: *Thomsonsche Schwingkreisformel* → "Thomson's formula"; *Mit eingesetzten Werten:* → "Substituting the values:", also inside `\text{}` in AD225; bare decimal commas in formulas (`4,7 \cdot`) → points; *induktiver Widerstand* → inductive reactance (glossary §3); AD203 *zur Abblockung von Störungen* → "to decouple interference" (glossary §5 *Abblockkondensator*).

## Suspected errors in the German original

- slides/schwingkreis_2.md (Parallelschwingkreis) — "Theoretisch ist die Impedanz bei Resonanzfrequenz unendlich hoch / Praktisch bestimmt das Bauteil mit dem geringsten Widerstand die Gesamtimpedanz": at resonance $X_L = X_C$, and in practice the impedance is limited by the losses ($R_P$); the component with the lower resistance dominates only away from resonance, as the section says. Translated as written.
- slides/schwingkreis_1.md — "kein Elektrolyt, da diese nur bei Gleichspannung funktionieren": electrolytic capacitors are polarised and need a DC bias, but they do work with AC (e.g. as AF coupling capacitors); the section gives the relevant reasons (frequency-dependent capacitance, high internal resistance at RF). Kept.
- slides/oszillatoren.md — "Quarz wird mit einem (schlechten) LC-Oszillator zum stabilen Schwingen angeregt": in a crystal oscillator the crystal takes the place of the LC tuned circuit as the frequency-determining element of the amplifier's feedback loop; it is not excited by a separate LC oscillator. Kept.
- sections/schwingkreis_2.md — "Die Güte eines Schwingkreises … wird durch das Verhältnis der Blindwiderstände … zum ohmschen Verlustwiderstand bestimmt": true for the series loss resistance ($X_L/R_S$); for the parallel circuit the formula given just below is the inverse ratio $R_P/X_L$. Kept.
- sections/schwingkreis_1.md — LC oscillation paragraph: "Sobald das Magnetfeld jedoch aufgebaut ist, entlädt sich der Kondensator vollständig" puts effect before cause (the field reaches its maximum when the capacitor has discharged); "Das Magnetfeld … entlädt sich" (a field collapses). Kept in meaning.
- slides/schwingkreis_1.md — picture 591 (low-pass response) has the ident `e_hochpass`, the same as picture 592 (high-pass response). Markup, kept.
- Typos with no effect on the English: sections/schwingkreis_1.md "sogennantes", "in dem man" (indem), "in den Folgenden zwei Fragen", "Welche Schaltung … verwendet werden", "Im Idealen Fall", "bei der Resonanzfrequenz der sehr hoch", "umgehrter"; sections/schwingkreis_2.md "; Dafür"; slides/schwingkreis_1.md "eines Hochpass", "eines Tiefpass", "eines Serienschwingkreis", "eines Parallelschwingkreis"; slides/schwingkreis_2.md "in 1853" (English construction in German); sections/oszillatoren.md "Ihre" (capitalised); sections/oszillator_vco.md "Dies gilt für VCOs als auch für VFOs" (*sowohl* missing); sections/oszillator_tcxo_ocxo.md "verschiedene arten"; slides/oszillator_tcxo_ocxo.md "Crystal Oszillator".

## Provjera

Checked all 22 files against `18db99b~1` paragraph by paragraph, and the
prose against the English ED201–ED216, ED501–ED507, AD201–AD229,
AD601–AD606, AD611, AF215, EF207, EF304. Complete: nothing dropped or added.
`revizija-guard.py --rev 18db99b~1 --brojevi`: 22 files, *struktura
netaknuta*.

Changes: omission 0, meaning 0, technical 3, style 9, glossary 1.

- Technical — sections/oszillator_vco.md, slides/schwingkreis_2.md: the
  *Grenzschicht* that widens and narrows with the reverse voltage is the
  depletion layer, not the junction itself → "the width of the depletion
  layer at the PN junction", "the depletion layer widens / narrows",
  "narrower depletion layer in the varicap"; glossary row *PN-Übergang /
  Grenzschicht* given a note to that effect.
- Technical — oszillator_vco: *in Sperrrichtung betrieben* → "operated with
  reverse bias" (was "in the reverse direction").
- Technical — oszillator_tcxo_ocxo: *thermisch abgeschirmt* → "thermally
  insulated", the wording of AF215 embedded right after it (was "thermally
  shielded"); *Verstärkungsfaktor* → "gain".
- Style — schwingkreis_1: the electric field "decays" through the inductor
  (was "discharges"); tuning fork "set vibrating when it is struck" (was "by
  a knock"); "depends only slightly on" (was "only a little"); *Wir halten
  fest* → "To sum up" (was "Let us note").
- Style — slides/schwingkreis_1 (×2): "The filter response is shown in one
  of the following questions" (was "comes in").
- Style — schwingkreis_2: attenuation "compared with the point of maximum
  transmission" (was "compared with the maximum passed").
- Style — oszillatoren: LC oscillator sentence recast, "whose
  frequency-determining elements form a tuned circuit …".
- Style — oszillator_tcxo_ocxo: "is preferable to" (was "is to be preferred
  to"); AD203: "to decouple the supply voltage of the circuit from
  interference" (was "to decouple interference on the supply voltage").

Judgement calls reviewed and kept: *Leitkreis* → "series pass circuit" with
the German word (drawing 1039 confirms a series LC in series with the signal
path; in English that is also an acceptor circuit, so no separate name
exists), the *Schwingkreis* gloss, the *Reihen-/Serienschwingkreis* and
*Quartz* slide notes, "Also called the quality factor", *Frequenzabweichung*
→ frequency error, the GNSS/GPSDO bracket rule, "Substituting the values:".
All 23 new glossary rows kept; the corrected *Leitkreis* row kept. The
suspected errors in the German are confirmed as listed (the slide claim that
at resonance the lower-resistance component sets the parallel circuit's
impedance; electrolytics "only work with DC"; the crystal "excited by a
(poor) LC oscillator"; Q as reactance over loss resistance holding only for
the series form).
