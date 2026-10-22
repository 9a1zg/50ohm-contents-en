# nea_digitale_uebertragungsverfahren_2 — translation report

Chapter "Digitale Übertragungsverfahren (2/3)" (Digital transmission methods,
part 2): 14 sections, each with its slides, and 3 solutions. 31 files:

- `contents/sections/` and `contents/slides/`: `datenuebertragungsrate.md`,
  `symbole_symbolrate.md`, `iq_verfahren.md`, `ask_fsk_afsk.md`, `mapping.md`,
  `psk.md`, `qam.md`, `symbolumschaltung_bandbreite.md`, `afsk.md`,
  `shannon_hartley_gesetzt.md`, `quellencodierung.md`, `kanalcodierung.md`,
  `fehlererkennung.md`, `fehlerkorrektur.md`.
- `contents/solutions/`: `AA104.md`, `AE405.md`, `AE406.md`.

`revizija-guard.py --brojevi`: 31 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comment of
symbolumschaltung_bandbreite (unchanged) and the applet label *Erneut
übertragen*, kept in brackets on purpose (DECISIONS.md). Line counts, blank
and whitespace-only lines (ask_fsk_afsk line 18, shannon_hartley_gesetzt line
15, the leading empty line of symbolumschaltung_bandbreite), trailing spaces
and the final-newline state are as in the German in every file except
slides/fehlerkorrektur.md, which is one line shorter because a bullet that
only gave the English term was dropped (judgement calls).

Embedded questions looked up in English and the prose aligned with them:
EA106, EE401, AA104, AE405, AE406, AF633, EE101, EE406, EE407, AE401–AE404,
AF632, AE415, AE214, AJ220, AJ221, EE408, AE416–AE420, AE408–AE414 (e.g.
EE401 "frequency range used", "amount of data transmitted per unit of time";
AE405/AE406 "symbol frequencies", "baud"; AF633 "in-phase", "90 ° phase-shifted";
AE404 "varying the amplitudes of two carriers phase-shifted by 90 ° and adding
them"; AE415 "speed of switching between different symbols"; AJ220 "key
clicks"; EE408 "audio frequency-shift keying (AFSK)"; AE416 "Shannon–Hartley
theorem", "highest theoretically achievable data rate"; AE408 "source coding";
AE409 "adding redundancy"; AE411/AE412 "check bit (parity bit)", "user data";
AE410 "cyclic redundancy check (CRC)", "checksum method"; AE413
"retransmission"; AE414 "forward error correction (FEC)").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

24 rows: *Datenübertragungsrate / Datenrate / binäre Zahlen, die sogenannten
Bits*; *Symbolfrequenz / Symbolgröße / Symbolgrenze / Symbolintervall /
Symbolumschaltung*; *Bit/Symbol* in units; *Zeicheneinheiten*;
*I/Q-Darstellung / I/Q-Ebene / I-Achse / Signalpunkt / Konstellationspunkt /
Signalzustand*; *Zeigerdarstellung / komplexer Zeiger / Signalzeiger*;
*In-Phase Component / Quadrature Component*; the keying methods with the
German's bracketed English names (ASK, FSK, PSK, QPSK, AFSK, quaternary ASK);
*Mapper / Bitstrom / Bitkombination / Bitfolge*; *Entscheidungsbereich /
Entscheidungsgrenze / Empfangswert*; *I/Q-Modulator / gewichtet / Wertepaar /
Freiheitsgrade*; *Schweizer Taschenmesser*; *DA-Wandler*; *Sprechfunkgerät*;
*Quelle / Senke / Irrelevanz*; *Codec / Codec2*; *Prüfbit (Parity Bit) / Even
Parity / Odd Parity*; *Mehrbitfehler / Ein-Bit-Fehler / Restwahrscheinlichkeit
/ Ausweisnummer*; *erneute Übertragung / Neuübertragung*; *Paritätsprüfung
schlägt fehl / erweiterter Hamming-Code*; the FEC sentence that only gives the
English term; *Spitzfindigkeit:*; *Rauschenergie*; applet control labels.

## Added to `DECISIONS.md`

One entry (Course text):

- Labels in the applets: English, with the German label in brackets, since
  the applets are still German — 'The button "Transmit again" (*Erneut
  übertragen*)' (psk slides), as the formula-sheet keywords and the Annex 1
  columns; the bracket goes when the applets are translated.

## Judgement calls

- Throughout: *Datenübertragungsrate* and *Datenrate* → "data rate" (EA106, EE401, §8); *Übertragungsverfahren* → transmission method; *Modulationsverfahren* → modulation method; *Phasenlage* → phase (§14); *Zeiger* → phasor (§14 *Zeigerdiagramm*); *Hochfrequenzträger* / *HF-Hardware* → RF carrier / RF hardware; *Kurzwelle* → HF; *WLAN* → Wi-Fi; *Klasse E* → Class E; *Abbildung [ref:…]* → "Figure [ref:…]"; *sogenannte* → "what is known as" / "known as"; *gegeben / gesucht / Lösungsweg* on slides → "given / required / Solution"; German „…" → "…".
- Units: `\bit\per\text{Symbol}`, `\bit\per{Symbol}` and `\text{Symbol}\per\second` → `symbol` (a running word inside the unit, as `\text{Bits}` → `\text{bits}` in the previous unit); the subscripts $R_\mathrm{Daten}$, $R_\mathrm{Symbol}$ stay (word subscripts are symbols, DECISIONS.md); *Einheit ist Baud* → "unit is the baud", the symbol after numbers (`\baud`).
- datenuebertragungsrate: *in Form von binären Zahlen …, den sogenannten Bits* → "in the form of binary digits, known as bits" (a bit is a binary digit; "binary numbers" would be loose in English); *in der Umgangssprache von der Datenübertragungsrate als Bandbreite gesprochen* → "in everyday language the data rate is spoken of as bandwidth"; *widrige Bedingungen* (slide) → "poor conditions"; *Funkbedingungen* → propagation conditions (§2 *Funkwetter*).
- symbole_symbolrate: *umgetastet* → "shifted" (AE405 "shifted between two symbol frequencies"); *bereits aus Klasse E bekannte Frequenzumtastung (Frequency-Shift Keying, FSK)* → "frequency-shift keying (FSK), already familiar from Class E" (bracket rule); *Zeitdarstellung* → time domain; slide bullets *2 Symbole → 1 Bit/Symbol* → "2 symbols → 1 bit/symbol", plural "bits" from two on.
- iq_verfahren: *I/Q-Darstellung* → "I/Q representation"; *In-Phase Component* / *Quadrature Component* in lower case (the German already gives the English names); *Anschaulich kann man sich vorstellen* → "It helps to picture it like this"; *Für mathematisch Interessierte* → "For the mathematically minded"; `\text{Amplitude und Phase}`, `\text{Träger}` → `\text{amplitude and phase}`, `\text{carrier}` (running words in an underbrace); *(vgl. [ref:a_iq_ebene])* without *Abbildung* kept as "(see [ref:a_iq_ebene])".
- ask_fsk_afsk, mapping, psk: captions *Amplitudenumtastung (Amplitude-shift Keying)* → "Amplitude-shift keying" (bracket rule); *ASK (Amplitude-Shift Keying) im zeitlichen Verlauf* → "ASK (amplitude-shift keying) over time" (the expansion explains the abbreviation and stays); *Baustein* → "building block"; *Spitzfindigkeit:* → "Splitting hairs:"; *Randbemerkung:* in a slide note → "Side note:"; *nicht eindeutig festgelegt* → "not fixed" (the next sentence asks for a unique assignment, so "not unique" would contradict it); *Entscheidungsbereiche* → decision regions.
- psk slides: the applet label *„Erneut übertragen"* → 'The button "Transmit again" (*Erneut übertragen*)' — new DECISIONS.md entry; *Mit zunehmendem Rauschen steigt die Wahrscheinlichkeit für Symbol- und damit Bitfehler* → "As the noise increases, so does the probability of symbol errors, and with them bit errors".
- qam: *gewichtet* → "weighted" (the German's word; AE404 says "varying the amplitudes"); *DA-Wandler* → "D/A converters"; *Software Defined Radios (SDR)* → "software-defined radios (SDR)" (§6); *zum gewünschten Signalpunkt* → "desired signal point" (not *wanted*, the receiver's sense, §6); *Schweizer Taschenmesser der Modulatoren* → "Swiss Army knife of modulators"; *Betrag des Signalzeigers* → "magnitude of the signal phasor"; *3-stellige Bitfolge* → "3-digit bit sequence", keeping the digit.
- symbolumschaltung_bandbreite: *Zeicheneinheiten zur Übertragung des Informationsgehaltes* → "signalling units used to transmit the information content"; *andere Funkverbindungen beeinträchtigen* → "impair other radio communication"; *sogenannte Tastklicks* → "what are known as key clicks" (§6, AJ220); *Umschaltung zwischen zwei Symbolen* → "the signal switches between two symbols".
- afsk: *hörbare Frequenzen (Niederfrequenz)* → "audible frequencies (AF)" (NF → AF); *Sprechfunkgerät* → "voice radio"; *Aussendung per Funk* → "transmission by radio"; *digitales Verfahren im Amateurfunk* (APRS) → "digital mode in amateur radio"; *APRS (Automatic Packet Reporting System)* kept, the expansion explains the abbreviation; *Mikrofon- und Lautsprecheranschluss genügen* → "A microphone and loudspeaker connection is all that is needed".
- shannon_hartley_gesetzt: *Shannon-Hartley-Gesetz* → "Shannon–Hartley theorem" (§8, AE416); *Merkhilfe* → memory aid; *das Hamnet* → "Hamnet" as the German writes it; *Rauschenergie* → "noise energy", as the German says; *Nutzsignal* → wanted signal; *wenige Zeichen pro Zeit* → "a few characters per unit of time"; *Durch ein SNR von …* (slide solutions) → "With an SNR of …"; *Signal-Rauschverhältnis* (slide spelling) → signal-to-noise ratio.
- quellencodierung, kanalcodierung: *Quelle (Sender) … Senken (Empfänger)* → "a source (transmitter) … sinks (receivers)"; *Redundanzen … Irrelevanzen* → "redundancy … irrelevance" (uncountable in English); *Nutzdaten* → user data (§8, AE412); *Codec2* unchanged; *Quellencodierer / Kanalcodierer* → source encoder / channel encoder (§14).
- fehlererkennung: *Prüfbit … auch Parity Bit genannt* → "the check bit. It is also called a *parity bit*" (two English terms, as AE411, so the sentence stays); *Even / Odd Parity* in lower case; captions *Das Byte mit Even Parity Bit* → "The byte with an even parity bit"; *Bei einer Fehlerübertragung* (slide) → "If an error occurs in the transmission"; *Ausweisnummern* → identity card numbers.
- fehlerkorrektur: *Im Englischen wird dieses Verfahren als Forward Error Correction (FEC) bezeichnet* dropped and the abbreviation moved to the first mention, "*forward error correction* (FEC)" — bracket rule, as §14 *Rauschsperre … Squelch*; the slide bullet *Im Englischen spricht man von Forward Error Correction (FEC)* dropped likewise (the slide heading already reads "Forward error correction (FEC)"), so slides/fehlerkorrektur.md is one line shorter; *die nebenstehende Vertiefung* → "the *In depth* box alongside"; *nicht prüfungsrelevant* → "not required for the examination"; *umgekehrt* (a bit) → inverted; *ähnlich einem Kreuzworträtsel* → "similar to a crossword puzzle"; *fehlerhafte Bit-Standort* → "position of the faulty bit"; the empty picture captions `[picture:683:hamming1: ]` … unchanged.
- solutions: AA104 *Ausschlussverfahren: … Hertz ist eine Frequenz* → "By elimination: … the hertz is a frequency", as the earlier solutions' "the volt is a voltage"; *logarithmische Hilfsmaßeinheit* → "logarithmic auxiliary unit" (§14); the trailing spaces of AA104 (line breaks) kept.

## Suspected errors in the German original

- sections/symbole_symbolrate.md (and question AE406, which uses the same values) — the FT4 example: four symbol frequencies about $\qty{200}{\hertz}$ apart ($\qty{14081.20}{\kilo\hertz}$ … $\qty{14081.83}{\kilo\hertz}$, spacings 200, 210 and 220 Hz) and, in AE406 and its solution, a symbol rate of $\qty{23.4}{\baud}$. FT4 as specified in WSJT-X uses 4-GFSK at about 20.8 Bd with a tone spacing of about 20.8 Hz (occupied bandwidth about 83 Hz). The arithmetic of the example is right; only the "e.g. FT4" does not fit. Kept. Not checked against DARC's corrections page for AE406.
- slides/iq_verfahren.md — slide "Konstellationsdiagramm" shows `[picture:1060:a_konstellationsdiagramm:…]`, but in the section drawing 1060 is the I/Q plane with one signal point (`a_iq_ebene`) and the constellation diagram with four points is drawing 1059. The slide probably means 1059. Kept (ids never change).
- sections/fehlererkennung.md and slides — two different drawings (678, 679) carry the same ident `even_parity`; harmless while neither is referenced, but a `[ref:even_parity]` would be ambiguous. Kept.
- sections/iq_verfahren.md — "(vgl. [ref:a_iq_ebene])" lacks "Abbildung" before the reference, unlike the next one. Kept.
- Typos with no effect on the English: sections/datenuebertragungsrate.md "kennen gelernt", "Sie gibt an wie viele" (comma); sections/psk.md "resultiert … zu einer Phasenverschiebung"; slides/shannon_hartley_gesetzt.md "Signal-Rauschverhältnis" beside "Signal-Rausch-Verhältnis"; slides/fehlerkorrektur.md "Anstelle eines einzelnen Prüfbit"; sections/afsk.md "nur wenige Daten pro Zeit"; the section ident `shannon_hartley_gesetzt` ("Gesetz") (idents never change).
