# pitanja_04 — translation report

175 questions (ED5, ND2, AD7, AD8, AE1–AE4, EE1–EE4, NE1–NE4, NF1, AF1,
EF1, NF201, AF224–AF231), 835 fields. `qbank-prevedi.py`: 0 refused,
0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §2: *QSO-Partner / Funkpartner* → the other station; *Funkrunde* → net.
- §5: *Schwingungserzeuger* → generator of oscillations; *Teilerverhältnis* →
  division ratio; *Frequenzsynthesizer* → frequency synthesiser;
  *Regelschleife* → control loop; *Quarzgenerator* → crystal oscillator;
  *symmetrisches Dämpfungsglied* → symmetrical attenuator.
- §6: *Spiegelselektion* → image rejection; *Kanalabstand / Kanalraster* →
  channel spacing; *Nachbarkanalstörungen* → adjacent-channel interference;
  *Begrenzerverstärker* → limiting amplifier; *Vorstufenrauschen*;
  *Empfängerstummschaltung* → receiver muting (squelch); *Passband-Tuning*;
  *Satellitenempfangsanlage*; *Fernspeisespannung* → remote supply voltage;
  *Handfunkgerät* → handheld transceiver; *Datenanschluss* → data port;
  *Drehwinkelgeber* → rotary encoder.
- §7: *Spitzenhub* → peak deviation; *unterdrücktes Zweiseitenband-
  Trägersignal* → DSB suppressed-carrier signal; *Splatter-Erscheinungen*;
  *Einton- / Zweiton-Testsignal*.
- §8: *Paritätsprüfung*, *Prüfsumme*, *Nutzdaten* → user data;
  *Zeit-/Frequenz-/Codemultiplexverfahren (TDMA/FDMA/CDMA)* → … multiple
  access; *Spreizcodierung* → spreading codes; *Kanalstörung* → channel
  impairment; *Umschaltgeschwindigkeit*; *paketvermitteltes Netz /
  Paketweiterleitung*; *Internetprotokoll* → Internet Protocol; *Teilnetz /
  Standardgateway / Gegenstelle*; *Stationskennung / Reflektor*.

## Added to `DECISIONS.md`

*symmetrisches Dämpfungsglied* → symmetrical attenuator (not balanced);
*…multiplexverfahren (…MA)* → … multiple access; made-up acronym expansions
in distractors get a made-up English expansion of the same acronym.

## Judgement calls

- EE101, AE214, AE203, AE201, NE208, NE207, NE206, AE401, EE407, EE406:
  picture answers have empty text; only the question was translated.
- NE209 c: *Der "Untere Schmalband Betrieb" ist aktiviert* (a fake expansion
  of USB) → 'The "Ultra Small Bandwidth" mode is activated.'; d *Die
  Unterspannung der Batterie ist erreicht* → "The battery has reached its
  undervoltage level." (keeps a U…B echo without forcing one).
- AD805, AD806: *symmetrisches Dämpfungsglied* → "symmetrical attenuator";
  "50 Ohm System" → "50 Ω system".
- EE409–EE411: *Zeit-/Frequenz-/Codemultiplexverfahren (TDMA/FDMA/CDMA)* →
  "time-/frequency-/code-division multiple access", as the abbreviations read.
- AF227: *Signal-Rausch-Abstand* → "signal-to-noise ratio"; distractors c/d
  play on *Abstand* (spacing) and lose a little plausibility in English, as
  there is no English "signal-to-noise spacing".
- NE405: *Linkstrecken* → "links", so that distractor d ("a list of links")
  keeps the German word-play with *Links*.
- AE101: the AFuV definition of occupied bandwidth follows the RR 1.153
  wording; *Amateurfunkverordnung* written out in full form from the
  glossary.
- AE301: answers are indirect questions in German ("Wie schnell sich …");
  English "It determines how fast …" in all four, so they answer the stem.
- AE302, NE308, NE307: *CW-Morsetelegrafie* → "CW Morse telegraphy";
  *…-Sprechfunk* → "… voice" (glossary).
- AE304, EE302: stems recast ("the result is that …", "the advantage of …")
  so each answer continues them grammatically; answers parallel.
- ED502–ED505: *Wie verhält sich die Frequenz* → "What happens to the
  frequency", so the stem does not presuppose a change (answer d: "remains
  stable").
- AE202 stem ends "approx." as the German ends "ca." with no ellipsis.
- AE211 d *Reichweite in CW* → "communication range in CW", so it is not
  read as dynamic range.
- EE206 b/d: *Störungen von / bei Stationen* both → "Interference to
  stations …" (both distractors).
- AE422 d *Überreichweiten anderer OFDM-Sender* → "Signals from distant OFDM
  transmitters via enhanced propagation".
- NF101–NF105: *Anzeige 1/2/3/4* → "display element 1/2/3/4" (to keep it
  apart from "the display of a transceiver"); *Amplitudenspektrum* →
  "Spectrum display" (glossary).
- AF104: the German "er" for the radio amateur avoided ("The amateur then
  switches on a power amplifier"); *100-fach* → "100 times".
- EE405 c: the German's LaTeX `pla\^it` kept unchanged.
- Suspected slips in the German, translated normally: NE102, EE205 b/c,
  NE209 c, NE308 d, NF107 b/c, NF113 c, AE410 d, EE401 b, AF226 a, AF230,
  AF231 have trailing spaces; AE301 a and EE408 d end in a newline; NE206
  and NE310 c have double spaces; AE402 b and EE404 d contain non-breaking
  spaces — all dropped. AF101 "Um wie viele" vs AF102 "Um wie viel" (same
  question type) → both "By how many".

## Provjera

175 questions checked (all five fields against the German from
`upstream/main`), 10 fields in 8 questions changed via
`pitanja_04.provjera.json` (`--retranslate`: 0 refused, 0 warnings):
6 style, 2 meaning, 2 answer balance (AF227), plus one glossary fix.

- AD801, AD802 question: "What does this circuit show?" → "What does this
  circuit represent?" — a circuit does not "show"; same form as EF101,
  ED208–ED215.
- AE422 question: "With which type of channel impairment …" → "For which
  type …" (idiom).
- AE422 d: "distant OFDM transmitters" → "other OFDM transmitters" — the
  German says *anderer*; "distant" added information.
- EE402 question: "fed in as an AF audio signal" → "fed in as an audio (AF)
  signal" (tautology).
- EE413 c: "The remote station …" → "The remote end …" — *Gegenstelle* in
  IP is the peer; "remote station" is the glossary term for *Remote-Station*
  (remotely controlled station). Glossary row changed to "remote end (peer)".
- NE401 d: "not loaded unnecessarily" → "not occupied unnecessarily"
  (*belastet* of a band is occupancy, not electrical load).
- AF227 a, b: "It states by what ratio …" → "It states how many times
  stronger …". With *Signal-Rausch-Abstand* → "signal-to-noise ratio", the
  word "ratio" in a/b echoed the stem and pointed straight at the a/b pair,
  while c/d lost their German echo of *Abstand*; without the echo the four
  answers are about as balanced as in German. Meaning of a/b unchanged.
- AF230 question: "rather negligible" → "largely negligible" (calque of
  *eher*).

Judgement calls reviewed and kept: NE209 c "Ultra Small Bandwidth" is as
plainly made up as *Unterer Schmalband Betrieb* and still spells USB;
NF101–NF105 "display element N" reads correctly with every answer; NE405
"links"; AE301, AE304, EE302 stems. The three new DECISIONS.md entries are
correct and stay as written (*symmetrical attenuator* is the standard
English term for equal input/output impedance; *…MA* expanded as *multiple
access*; made-up acronym expansions).
