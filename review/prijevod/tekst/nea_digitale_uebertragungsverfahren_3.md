# nea_digitale_uebertragungsverfahren_3 — translation report

Chapter "Digitale Übertragungsverfahren (3/3)" (Digital transmission methods,
part 3): 5 sections, each with its slides, no solutions. 10 files:

- `contents/sections/` and `contents/slides/`: `sende_empfangsketten.md`,
  `vielfachzugriff.md`, `ofdm.md`, `synchronisation.md`,
  `polarmodulation.md`.

`revizija-guard.py --brojevi`: 10 files checked, *struktura netaknuta*.
German-word grep: no hits; the only non-ASCII German is the picture ident
`a_sdr_empfänger` (unchanged). Line counts, blank lines (the leading empty
line of sections/synchronisation, the two trailing blank lines of
slides/vielfachzugriff), trailing spaces (slides/sende_empfangsketten,
sections/ and slides/vielfachzugriff, slides/synchronisation), the double
spaces after two full stops in sections/polarmodulation and the
final-newline state are as in the German in every file.

Embedded questions looked up in English and the prose aligned with them:
AF626–AF629 ("transmit path" / "receive path"; the prose keeps the
glossary's *transmit / receive chain* for *Sende- / Empfangskette*), EE409–EE411
("time-division / frequency-division / code-division multiple access",
"Simultaneously, using spreading codes, in the same frequency range",
"Alternating rapidly in time on the same frequency"), AE421, AE422
("orthogonal frequency-division multiplexing (OFDM)", "narrow-band
interference", "multipath propagation"), AE407 ("synchronisation",
"Establishing time alignment between transmitter and receiver").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

10 rows: *De-Mapper / I/Q-Demodulator / Sender-Prozess / Empfänger-Prozess*;
*Zugriffsverfahren / Störanfälligkeit / Bandbreiteneffizienz / Spreizcode*;
*Mobilfunksystem / schnurloses Telefonsystem / satellitengestütztes
Navigationssystem*; the multiplexing captions *… mit drei Signalen*;
*Trägerabstand / Frequenzfehler / Dopplerverschiebung / frequenzselektives
Fading*; *Intersymbolinterferenz oder Symbolübersprechen*; *Synchronisierung /
zeitliche Übereinstimmung*; *Grundfrequenz (Polarmodulation) / Wellenzug*;
*momentane Amplitude / Phase / Amplitudenpfad / Phasenpfad / aufprägen*;
*Blick über den Tellerrand*.

## Added to `DECISIONS.md`

None. Everything followed existing entries (the TDMA/FDMA/CDMA rule, the
bracket rule, Figure capitalisation).

## Judgement calls

- Throughout: *Abbildung [ref:…]* / *(vgl. Abbildung [ref:…])* → "Figure [ref:…]" / "(see Figure [ref:…])"; *HF-Träger* → RF carrier; *NF-Verstärker* → AF amplifier; *Daten* as a plural ("the encoded data are"), as most of the earlier units; *Teilnehmer* and *Nutzer* both → user (§14 *Teilnehmer (Netzwerk)*), "their" for the singular user.
- sende_empfangsketten: *A/D-Umsetzer* / *D/A-Umsetzer* → "analogue-to-digital converter" / "digital-to-analogue converter" (§8; the German gives no abbreviation); *versieht … gezielt mit Redundanz* → "deliberately adds redundancy"; *sollte für Prüfungsfragen gut eingeprägt werden* → "it should be memorised well for the examination questions"; the step lists as imperatives ("compress the data", "add redundancy …"), as the German infinitives; *Für einen Empfänger funktioniert das Ganze rückwärts* → "works in reverse"; *Wir fassen … zusammen* → "We sum up"; the receiver's *Leistungsverstärker* kept as "power amplifier" (see errors); *De-Mapper* → "de-mapper"; captions *SDR Sender / Empfänger für Sprachkommunikation* → "SDR transmitter / receiver for voice communication".
- vielfachzugriff: where the German gives the abbreviation, *Frequenzmultiplex (FDMA)* etc. → "frequency-division multiple access (FDMA)" (§8, DECISIONS.md); *Frequenzmultiplexverfahren (FDMA – Frequency Division Multiple Access)* → "frequency-division multiple access (FDMA)" (the English expansion only repeats the term; bracket rule); slide bullets *Time Division Multiple Access – Zeitmultiplexverfahren* → "Time-division multiple access", as digital_voice; captions without an abbreviation (*Frequenzmultiplexing*, *Zeitmultiplexverfahren mit drei Signalen*) → "Frequency-division multiplexing", "Time-division multiplexing with three signals" (§8 note); *geringem Interferenzbedarf* → "low interference requirements" (see errors); *Mobilfunksysteme* → "mobile phone systems" (GSM, AMPS, UMTS); *Dem stehen jedoch … gegenüber* → "Against this, however, stand …"; *getrennt und nacheinander … gesandt* (slide) → "split up and sent one after another"; *codiert (gemischt)* → "encoded (mixed)".
- ofdm: *Beim orthogonalen Frequenzmultiplexverfahren, (Orthogonal Frequency-Division Multiplexing, OFDM)* → "In orthogonal frequency-division multiplexing (OFDM)" (bracket rule; §8); *ein sogenanntes "Übersprechen"* → 'what is known as "crosstalk"' (§14); the slide note *OFDM: Orthogonal Frequency-Division Multiplexing* kept as an expansion of the abbreviation, lower case; *Übersprechen: Gegenseitiges Stören untereinander* → "Crosstalk: mutual interference between the carriers" ("between the carriers" makes the German *untereinander* explicit, since the slide has no other subject); *Intersymbolinterferenz oder Symbolübersprechen* → "intersymbol interference, or crosstalk between symbols" (English has only the one term); *die wir einige Kapitel zuvor kennengelernt haben* → "that we met a few chapters ago"; *Im Falle von Mehrwegeausbreitung* → "where there is multipath propagation" (AE422).
- synchronisation: *Synchronisierung* → synchronisation (§8, AE407); *die zeitliche Übereinstimmung ist hergestellt* → "time alignment has been established", AE407's wording; *sich auf den Beginn der Sendung einstellen* → "adjust to the start of the transmission"; slide *Dient dazu, dass …* → "Enables the receiver to recognise …".
- polarmodulation: *[index:Polarmodulation]* → `[index:Polar modulation]`; *als Blick über den Tellerrand* → "as a look beyond the syllabus" (the sentence before says there is no examination question); *wenn ich … hinein zoome* → "when you zoom in, in time, on …" (the German's generic *ich* as generic *you*, as for *du*/*wir*); *Wellenzug* → "cycle" (one period of the wave; "wave train" means a group of waves in English); *Grundfrequenz* → "base frequency", not the glossary's *fundamental frequency* (§3), which here would suggest harmonics — the carrier frequency the phase is shifted from; glossary row added; *Schaltendstufe* → switching amplifier (§6), *Endstufe* → output stage, *Endstufentransistoren* → output transistors (§6); *Klasse-E-Verstärker*, *"Klasse D"-NF-Verstärker*, *Klasse E* → "class E amplifier", '"class D" AF amplifiers', "class E", lower case (§14); *manipuliert* → "manipulated", as the German; *aufgeprägt* → "impressed"; *Schaltnetzteil-Technologie* → "switch-mode power supply technology" (§5); *Metallkühlkörper* → "metal heatsinks"; *klassisch analog* → "conventionally analogue"; *billiger als eine Pizza* kept; caption *Polar Modulator* → "Polar modulator" (sentence case); slide heading *Vorteil im Funkgerät* → "Advantage in the radio"; *Stromverbrauch* → "current consumption".

## Suspected errors in the German original

- sections/sende_empfangsketten.md — receive chain: "Die Antenne empfängt das Signal, das durch einen Leistungsverstärker verstärkt wird". A receiver amplifies the antenna signal with a (low-noise) preamplifier, not a power amplifier; the sentence mirrors the transmit chain. Translated faithfully ("power amplifier").
- sections/vielfachzugriff.md — FDMA "eignet sich besonders für Systeme mit wenigen Nutzern und geringem Interferenzbedarf": *Interferenzbedarf* ("need for interference") makes no sense; perhaps *geringer Interferenzgefahr* or *geringem Bandbreitenbedarf* was meant. Rendered "low interference requirements".
- slides/vielfachzugriff.md — FDMA slide: "Das digitale Signal wird auf mehrere Frequenzen aufgeteilt / Dadurch kann mehr Bandbreite verwendet werden" describes one signal spread over several frequencies (closer to a multicarrier method such as OFDM), whereas the section and EE410 describe FDMA as separating users by frequency. Kept.
- slides/vielfachzugriff.md — the FDMA picture `[picture:845:e_vielfachzugriff_cdma:…]` carries the same ident as the CDMA picture 846 on the same slide set; probably `e_vielfachzugriff_fdma` was meant. Harmless while neither is referenced. Kept (idents never change).
- sections/polarmodulation.md and slides — "Wirkungsgrade von mehr als 80–90 %" ("more than" with a range); kept as "more than 80–90 %" (the slide has $\eta \approx$ 80–90 %).
- Typos with no effect on the English: slides/vielfachzugriff.md "über die dieselbe Frequenz", "zum decodieren"; sections/ofdm.md stray comma "Frequenzmultiplexverfahren, (Orthogonal …"; sections/polarmodulation.md "es ergibt sich die gewünschten Hüllkurve"; slides/polarmodulation.md "kleiner ausfallen das spart Gewicht" (missing comma); sections/sende_empfangsketten.md "Symbole z. B. Amplitude" (missing comma).

## Provjera

All 10 files compared paragraph by paragraph with the German of 795b529~1;
embedded questions AF626–AF629, EE409–EE411, AE421, AE422, AE407 checked
against the English bank. Nothing dropped or added. All 10 glossary rows
kept (one amended); no DECISIONS.md entry needed. Judgement calls kept,
except *manipuliert* and the generic *ich* phrasing (below). Suspected
errors in the German confirmed as listed. Guard `--rev 795b529~1
--brojevi`: struktura netaknuta.

Changes: omissions 0, meaning 1, technical 1, style 6, glossary 1.

- ofdm (section): *Frequenzabweichungen zwischen Sender und Empfänger* "frequency deviations" → "frequency offsets": *deviation* is the FM *Hub*, and §14 *Frequenzabweichung* says not *deviation*; "frequency errors" would repeat the *Frequenzfehler* they cause. Glossary row *Trägerabstand / Frequenzfehler …* amended accordingly.
- vielfachzugriff (section): *indem ihnen der Zugriff zeitlich aufgeteilt wird* "by dividing up their access to it in time" (as if the users did it) → "share the same frequency channel, with access to it divided among them in time".
- vielfachzugriff (section): "Against this, however, stand comparatively complex signal processing …" → "On the other hand, it involves comparatively complex signal processing …".
- vielfachzugriff (slides): "put back together" → "reassembled".
- sende_empfangsketten (section): "it should be memorised well" → "it should be learnt by heart".
- ofdm (section and slides): "error correction methods with redundant data transmission" → "… using redundant data transmission".
- polarmodulation (section): "when you zoom in, in time, on any signal …" → "when you zoom in on any signal … along the time axis".
- polarmodulation (section): *manipuliert* "manipulated" → "varied".
