# Final consistency pass over the exam question bank

All 1750 questions (8750 fields) read with Python, German from
`upstream/main`, English from the working tree, after the ten batches
`pitanja_01`–`pitanja_10` had each been translated and checked. Fixes are in
`zavrsni.json`, applied with `qbank-prevedi.py --retranslate`: 105 fields in
42 questions, 0 refused, 0 warnings. No answer changed its meaning and no
answer's correctness changed.

## 1. Units after a number — 92 fields

The rule (symbol after a number, DECISIONS.md) came after batches 01 and 02.
Every "… ohm(s)" after a digit became "… Ω", in running text and in
attributive use ("a 50 Ω dummy load", "Ten 500 Ω carbon-film resistors"),
always for the whole answer set: AB101, AB102, AB205–AB208, AB301, NB505,
EB507–EB509, EB512–EB514 (batch 01); EC105, EC106, EC113, EC116, EC304,
EC515, EC516, EC522, AC106, AC305, AC306, AC522, AC604, AD104, AD105,
AD109, AD110, AD112 (batch 02). AB301 also "0.5 amperes" → "0.5 A".

Left as they are: the unit name where the unit itself is meant (NA201–NA203,
EA101, EA102 "ohm (Ω)", AA101 "ohm", AC110/AC209 "ohms per farad / henry");
AG411 "almost zero ohms" (a number written as a word); AK103's
`30 Ohm` inside the display formula (formulas stay as in the German);
"Kilowatt" in BA102/BA103 (a spelling-alphabet code word, DECISIONS.md);
times in prose ("60 seconds", "6 minutes", "67 hours and 30 minutes"),
which are not SI electrical units and read as the German does.

## 2. Fields identical to the German — 0 changed

675 fields are identical to the German and contain letters outside `$…$`
(the ~203 counted beforehand excluded unit-only fields such as "40 W").
All were read. They are numbers with unit symbols, formulas, call signs and
prefixes, Q codes and operating abbreviations (CW, SSB, VOX, PTT, OCXO …),
connector names (BNC, SMA, N, PL), "Region 1–4", UTC times, and words that
are the same in English (Diode, Transistor, Emitter, Amplitude, Gold,
Aluminium, horizontal, Squelch, Sampling, Firewall, Watchdog, Interferometer,
Multimeter, Synchronisation, Fading, Backscatter, Block 1–3). The only
German words are deliberate: BE104 c "EA6VQ, es ruft Sie DF1KW, bitte
kommen." (the reply in German to an English CQ is what makes it wrong,
batch 09), BD209 "/Ausbildung" (DECISIONS.md, call sign suffixes), the
spelling-alphabet distractors of BA101–BA110 (DECISIONS.md), and outside
identical fields the German titles in brackets (VC104, VE501), "Watt-Wächter"
(VC121) / "Watt Wächter" (VE515), spelt as the German spells each, and the
Mögel–Dellinger effect.

## 3. Double spaces — 0 changed

The raw text has 8 double spaces, all inside `$…$` (EB505, EB506
`…;  …`), left untouched. The larger count seen beforehand (~162) comes
from stripping the formulas out of a field, which leaves two spaces where
`$R$` or similar stood; the text itself has none.

## 4. Spelling — 5 fields

British spelling with -ise, licence/license, metre/meter, centre, colour,
analogue, aluminium, grey, neighbour, "call sign" (175 times, never
*callsign* or *call-sign*) were already consistent; "Organization for
Standardization" (VA407) is ISO's proper name, "program" (BG103) is a
computer program. One deviation from the glossary's *S meter*: "S-meter
reading" → "S meter reading" in AA114, AF101, AF102, AF105, EI202 d, as in
NF101–NF104, NF301, AF103, AF104 and "SWR meter reading" (NG302).

## 5. Terms the checkers changed late — 1 field (plus 6 below)

Every glossary row that a checker or a later batch changed (`git log -p --
TRANSLATION_GLOSSARY.md`) was checked against every question whose German
uses the term: *Querwiderstand* (AC517, AC518), *Gegenstelle* (EE413),
*Vorteiler* (AI302 attenuator, AI504 prescaler), *Schleifendipol* /
*Faltdipol*, *Erregerfrequenz* / *Erregung* (AG111–AG113, AG203–AG206),
*Gleichwellenfilter* (AG109), *Mantelwellen* / *Mantelstrom* /
*stromkompensierte Drossel* / *Mantelwellendrossel*, ERP and EIRP forms,
law names (every *Amateurfunkgesetz*, *-verordnung*, *Funkanlagengesetz*,
*Telekommunikationsgesetz*, BEMFV, EMVG, 26. BImSchV, BImSchG, FreqV …),
*Landeskenner*, *Fuchsjagd*, *Nachprüfung*, *quasi-optische Sichtweite*,
*verbrummt*, *höchste durchlässige Frequenz*, *Einstrahlung*,
*Sperrtopfantenne*, *Strahlungsdichte*, *Verkürzungsfaktor* (antenna /
cable), *Umwegleitung*, *Öffnungswinkel* / *Halbwertsbreite*,
*Strombauch*, *Zweidrahtleitung*, *Thermoumformer*, *Überreichweiten*,
*Sprung*. All already used the current term. One later rule not yet
applied in batch 01:

- EB514: "A 50 ohm dummy load (artificial antenna)" → "A 50 Ω dummy load":
  *künstliche Antenne (Dummy Load)* is "dummy load" without a bracket that
  only repeats it (DECISIONS.md, bracket rule, AI601–AI603).

## 6. Same German, same English — 8 fields

Identical German fields were grouped; 15 groups had more than one English
form. Six were the ohm fields above (EC116/EC117 "220 Ohm", EC112/EC113,
EC515/AG416 "70 Ohm", AC522/AG305 "ca. 820 Ohm", AB207/ED104 "4 Ohm").
Changed besides:

- NG101: "Which component does this circuit symbol represent?" → "… the
  circuit symbol …", as the ten other questions with the same German stem.
- EB501 c, EB502 a, c: "antenna feed line" → "antenna feeder", the
  glossary's *Antennenspeiseleitung* (AG501 c, d, same German).
- EB501 d, EB502 d: "its gain" → "its gain (as a power ratio)", the
  glossary's *Gewinnfaktor* (AG501 a, same German).
- AG501 d: "supplied by a transmitter to the antenna feeder" → "supplied to
  the antenna feeder by a transmitter", the word order of AG501 c, EB501 c
  and EB502 a (and of RR 1.157 / 1.158).
- EJ215 b: "on another frequency band" → "on a different frequency band",
  as EE206 b.

Kept, because the answer set around them differs: AF412 b / AF413 b ("a
selective RF amplifier" after "It is ...", the bare form after "It is a
..."), AI609 c "An SWR meter" (an answer set with articles) beside the bare
"SWR meter" of NI201 and AI615, EI501 a / AI614 b (article in the answer or
in the stem), BB104 c / BB105 a (BB105's stem ends "Only stations ..."),
ED206 c "an inductor" / AG108 a "A coil" (the component vs a loading coil,
glossary *Spule*), EE205 b / NE306 b (gerunds vs imperatives, parallel to
their own answer sets).

## Meaning

No meaning problem found; nothing in this pass changes what a question asks
or which answer is correct.
