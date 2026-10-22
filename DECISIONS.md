# Decisions

Everything decided for the English translation that a reviewer should be able
to look up: what, when, and why. Conventions in day-to-day form are in
`TRANSLATION.md`; single terms in `TRANSLATION_GLOSSARY.md`, which is
authoritative. Choices about a single exam question are recorded in that
batch's notes, `review/prijevod/pitanja_NN.md` (translator's judgement calls
and the checker's "Provjera" section).

## Scope — decided by 9A1ZG, 2026-10-22

- **For DARC, a faithful translation** of the German original. Licence classes
  N, E and A, the Bundesnetzagentur and German law stay as they are: this is
  the German exam and course in English, not a localisation for another
  country.
- **British English** (IARU Region 1, RSGB usage).
- **A separate repository**, like the Croatian one, published on GitHub for
  DARC to take over. It keeps DARC's history so every change is visible.
- **Exam questions first**, then the course text, then picture descriptions
  and static pages.

## Language and form

- **Units after a number: always the symbol** (100 Ω, 4.7 kΩ), even where the
  German writes "Ohm"; the unit *name* only where the unit itself is meant.
  One answer set never mixes the two. (2026-10-22, after batches 01 and 02 had
  done it both ways; those two batches are aligned in a final pass.)
- **Decimal point**, not comma, also inside formulas (`\qty{29.7}{…}`). Every
  number stays the same number — the tooling refuses anything else.
- **Formulas and symbols unchanged**, German subscripts included
  (`R_\mathrm{ges}`), because they match the labels in the drawings, which are
  not translated yet.
- **German technical abbreviations become English** in running text: NF → AF,
  HF → RF, ZF → IF, KW → HF, UKW → VHF, EMV → EMC. Abbreviations of German law
  and institutions stay (AFuG, AFuV, BNetzA, EMVU, BEMFV).
- **Spelling with *-ise*** (authorisation, quantisation); ***call sign*** in two
  words, as in the ITU Radio Regulations.
- ***ca.* → approx., *etwa* → about**, consistently within an answer set.
- **Plain *you*** for both German *Sie* and *du*.

## Terms that needed a decision

- ***Oberwelle* keeps the German word in brackets** where a question turns on
  it, e.g. AB402 "The third overtone (Oberwelle) corresponds to … the fourth
  harmonic". German *n-te Oberwelle* is the (n+1)th harmonic; the bracket
  makes the trap visible to a reader who knows the German exam. — 9A1ZG,
  2026-10-22.
- ***Amateurfunkdienst* → amateur service** (ITU RR), not "amateur radio
  service".
- ***Zulassung zur Teilnahme am Amateurfunkdienst* → authorisation to
  participate in the amateur service**; *Amateurfunkzulassung* → amateur radio
  licence.
- ***Rufzeichenzusatz* → call sign suffix** (Ofcom usage) — note the clash with
  *Suffix*, the letters after the digit; the glossary explains how to keep both
  apart in one sentence.
- ***Internationales Buchstabieralphabet* → international phonetic alphabet**,
  lower case, so it is not read as the linguists' IPA.
- **Ionosphere: D, E and F *region***, as the German says, although RSGB texts
  often say "layer".
- ***Übertrager und Transformatoren* → signal and power transformers**,
  because English has one word for both.
- ***Rauschzahl*** is a noise **factor** where it is a ratio (F = 2) and a noise
  **figure** where it is in dB.
- ***Verkürzungsfaktor*** is the **velocity factor** for cables and the
  **end-effect (shortening) factor** for antennas.
- ***Querwiderstand*** in a voltage divider is the **lower divider resistor**,
  not "bleeder resistor", which is the power-supply discharge resistor
  (*Ableitwiderstand*). (Checker of batch 02.)
- ***Flanken-Diskriminator* → slope detector**; a bare *Diskriminator* stays
  **discriminator**. (Batch 03.)
- ***symmetrisches Dämpfungsglied* → symmetrical attenuator**, not "balanced":
  here *symmetrisch* means equal input and output impedance, while for
  feeders it stays *balanced*. (Batch 04, AD805, AD806.)
- ***Zeit-/Frequenz-/Codemultiplexverfahren (TDMA/FDMA/CDMA)* →
  time-/frequency-/code-division multiple access**, because the abbreviation
  the German gives spells *multiple access*; without an abbreviation they stay
  *…multiplexing*. (Batch 04, EE409–EE411.)
- **A distractor that is a made-up German expansion of an acronym** (NE209:
  "USB" as *Unterer Schmalband Betrieb*) gets a made-up English expansion of
  the same acronym and about the same plausibility ("Ultra Small Bandwidth"
  mode), rather than a literal translation that no longer spells it.
  (Batch 04.)
- **"What does the abbreviation X stand for?"** where X is English and the
  German answers are German terms (EF212, AGC): in German no answer spells the
  letters, in English the correct expansion does. Where a *faithful* rendering
  of a distractor can also fit the letters, choose it — *Automatische
  Gleichlaufsteuerung* → "Automatic ganging control" — so the correct answer
  does not stand out alone; never invent a distractor to do it. (Batch 05.)
- ***symmetrisch* on a circuit block is *balanced*** (AF306: *symmetrisches
  Filter* → "balanced filter", beside "balanced mixer"), as for feeders; only
  the attenuator, where it means equal input and output impedance, is
  *symmetrical* (batch 04). (Batch 05.)
- ***Verkürzungsfaktor* of an antenna → shortening factor** in exam
  questions (AG101–AG105, EG202), the glossary's bracketed form rather than
  "end-effect correction factor": it is what the German says, and the
  questions only multiply by it. Wherever the factor belongs to a cable or
  line it is the **velocity factor**, the established English term, with no
  exception — also EG201, whose correct answer defines it as a ratio of
  velocities (in English "shortening factor" is the antenna end effect, which
  would make distractor b, diameter to length, look right). (Batch 06;
  EG201 corrected by the checker.)
- **No echo the German does not have — but never at the cost of the
  established term.** Where the glossary would give a stem term and the
  correct answer the same English word although the German uses two
  different ones, the stem takes an alternative that is itself established
  English for the same thing, so the correct answer is not given away:
  *Mantelwellen* → "sheath currents" where the answer is *Gleichtaktanteile*
  → "common-mode components" (AG425, AG426), *stromkompensierte Drossel* →
  "current-compensated choke" (AG426). Where only the established term is
  accurate, it stays even if it echoes the answer (EG201 *velocity factor*).
  Same reasoning as the checker's AF227 fix in batch 04. (Batch 06, scope
  narrowed by the checker.)
- ***Mantelstrom* → sheath current** (EG404, AG428), the current on the
  outside of the braid; *Mantelwellen* stays *common-mode currents*. (Batch 06.)
- ***Eingangswiderstand* / *Fußpunktwiderstand* of an antenna → input /
  feed-point impedance**, not *resistance*: off resonance it is reactive, and
  the German itself calls it "rein kapazitiver Eingangswiderstand" (AG207,
  AG209). (Batch 06.)
- ***Cinch* → RCA (phono)**: a German trade name that English readers do not
  know for that connector (NG206). (Batch 06.)
- **Word subscripts in formulas stay German**, like `R_\mathrm{ges}`:
  `P_{\textrm{Sender}}`, `P_{\textrm{Verluste}}`, `G_{\textrm{Antenne}}`
  (AG502, EG502) are symbols, not prose, and the course text writes the
  same quantities as `P_\mathrm{Sender}` throughout. "Only words inside
  `\text{}` are translated" applies to running words in a formula, not to a
  subscript that names a quantity. (Batch 07.)
- ***äquivalente Strahlungsleistung (EIRP)*** without *isotrope*, and
  *gleichwertige isotrope Strahlungsleistung*, are written as the full
  established term **equivalent isotropically radiated power (EIRP)**
  (EG503–EG505, NG402): the abbreviation decides what is meant, and
  "equivalent radiated power" is not an English name for the EIRP.
  In German *äquivalente Strahlungsleistung* alone is the ERP (AG501,
  solution AK115), so EG503–EG505 are a slip in the German; their dBi
  figures confirm EIRP. (Batch 07; slip noted for DARC by the checker.)
  By the same rule AK115's *äquivalente Strahlungsleistung (ERP)* is
  written **effective radiated power (ERP)**, the ITU term (RR 1.162); its
  answer, 0.7 V/m from 100 W, is the ERP formula. AG501 alone keeps the
  German's "equivalent (effective)" pair, because it defines the term.
  (Batch 08, confirmed by the checker.)
- **The German generic *er* for a radio amateur** ("Er muss die Antenne
  drehen …", "erkennt er, dass …") is recast without a pronoun — "The
  antenna must be turned to …", "that "PY" has been worked" — or, where a
  pronoun is unavoidable, singular *they* (AH305). (Batch 07.)
- **Q code meanings in the ITU's English wording.** Where the German gives
  the German wording of a Q code, the English uses the established wording
  of the ITU Q code list (Rec. ITU-R M.1172, incorporated by reference
  in the RR; RR Appendix 14 is the phonetic alphabet and figure code) as
  radio amateurs use it — QRT "Stop sending.", QRZ? "Who is calling me?", QRN
  "I am troubled by static.", QSB? "Are my signals fading?" — not a fresh
  translation of the German, which is itself that list in German.
  Made-up meanings in distractors are translated faithfully. Two
  exceptions, where the ITU wording would not say what the German says:
  QTH "My location is ..." (*Standort* → location; the ITU has "My
  position is … latitude, … longitude"), and QRM / QRM? "I am being
  interfered with." / "Are you being interfered with?", the older wording
  that the German *Ich werde gestört / Werden Sie gestört?* follows (current
  M.1172: "Your transmission is being interfered with" / "Is my
  transmission being interfered with?", the other station's point of view,
  which would no longer match the German distractors). Glossary §2 lists
  them. (Batch 08, BB201–BB204; QRM corrected by the checker against the
  text of Rec. ITU-R M.1172.)
- **Spelling-alphabet distractors keep their words.** Wrong answers in
  "How is the call sign … spelt?" (BA101–BA110) use words of other spelling
  alphabets — *Nordpol*, *Ypsilon* (German DIN 5009), *Caesar*, *Queen*,
  *Baker*, *Santiago* … — and place names (*Guatemala*, *Honolulu*,
  *Oslo*). They are code words, not prose, and stay as the German writes
  them; translating *Nordpol* or *Ypsilon* would turn a real code word of
  another alphabet into a word that is in none. The one exception is
  *Amerika* → America, because the German otherwise writes these names in
  English (Denmark, Italy, Madagascar). (Batch 08.)
- **A bracket that only repeats the term in the other language is
  dropped**, as in EH202 (*Rückstreuung (Backscatter)* → "Backscatter"):
  *künstliche Antenne (Dummy Load)* (AI601–AI603) and *Abschlusswiderstand
  (Dummy Load)* (NJ202) → "dummy load"; *Received (empfangen)* → "Received"
  (BB110). A bracket that adds information stays, e.g. EH202 "Fluctuations
  in field strength (fading)", where the bracket gives the technical term.
  (Batch 08; examples corrected by the checker.)
- **Call sign suffixes in answers stay as the German writes them.** Wrong
  answers such as "DL1PZ/Ausbildung" (BD209) or "/RB or /Remotebetrieb",
  "/FB or /Fernbedient", "/F or /Fern" (BD208) are strings that would be
  transmitted as part of a call sign, and call signs are not translated;
  beside the correct "/Trainee" and "/Remote" they test, as in German,
  whether a German word may be used. An English "/Training" would test the
  difference between two English words instead. (Batch 09.)
- **RR provisions in the RR's own English wording.** Where the German
  paraphrases a provision of the Radio Regulations, the correct answer uses
  the RR's English wording, as for Q codes: RR 1.56 "duly authorised
  persons interested in radio technique solely with a personal aim and
  without pecuniary interest", "self-training, intercommunication and
  technical investigations" (VA102, VA104); RR 1.61 "accessory equipment
  necessary at one location" (VA201); RR 1.96 "a station in the amateur
  service" (VA202); RR 25.2 "communications incidental to the purpose of
  the amateur service as defined and … remarks of a personal character"
  (VA302); RR 25.2A "encoded for the purpose of obscuring … meaning",
  "earth command stations" (VA303). A distractor that sounds like the RR
  gets the same treatment (VA104 d, the older RR 25.2 "recourse to the
  public telecommunications service is not justified"); everything else is
  translated faithfully. Spelling stays *-ise*, as these are not direct
  quotations. German statutes have no official English text and are
  translated faithfully. (Batch 09.)
- **Band names beside the English abbreviation** (BC101–BC106: "Very High
  Frequency (VHF) oder Ultrakurzwelle (UKW)"): each German answer pairs the
  English band name with the German everyday name of the same band. In
  English the German name only repeats the English one, so it is dropped
  (bracket rule above): "Very High Frequency (VHF)", "Ultra High Frequency
  (UHF)" — UKW is VHF in English (TRANSLATION.md), and VHF / UHF are
  themselves the names English operators use. Where English has an
  everyday name of its own it stays: "High Frequency (HF) or short wave
  (SW)" (*Kurzwelle (KW)* only repeats *Short Wave (SW)*), "Medium
  Frequency (MF) or medium wave (MW)". The questions ask which range a
  band or frequency span belongs to; none turns on the metric names, so
  "metre waves" / "decimetre waves" (ITU-R V.431 metric / decimetric
  waves), which the translator first used, are not brought in: rare in
  English, they would put an unfamiliar label where the German reader sees
  a familiar one, and an English reader places the 2 m and 70 cm bands by
  VHF and UHF as readily as a German reader by UKW and Dezimeterwelle.
  The four answers stay the same set in
  every question, so the shorter VHF / UHF answers do not single out the
  correct one. (Batch 09; reworked by the checker.)
- **German statutes in exam questions: the English name, then the German
  short title and the abbreviation.** Where the German names a law by its
  one-word short title (*Amateurfunkgesetz*, *Funkanlagengesetz*,
  *Telekommunikationsgesetz*), every field that names it gets the glossary's
  English name with the German title and abbreviation in brackets — "Radio
  Equipment Act (Funkanlagengesetz, FuAG)" — also where the German leaves
  out the abbreviation (as BE406 c, VA406). Where the German writes the
  long formal title (*Gesetz über die elektromagnetische Verträglichkeit von
  Betriebsmitteln*, *Verordnung über das Nachweisverfahren zur Begrenzung
  elektromagnetischer Felder*), the English long title takes the
  abbreviation only — "Act on the Electromagnetic Compatibility of
  Equipment (EMVG)" — as the catalogue headings already do; a German title
  of a dozen words in brackets helps no one. Where the German gives both
  (VE505 "Funkanlagengesetz - FuAG"), so does the English, with a comma as
  in the glossary — also the 26. BImSchV's "(Ordinance on Electromagnetic
  Fields, 26. BImSchV)" (VE505, EK102). VC101, which
  asks which law it is and gives four bare titles, keeps four bare English
  titles, so that no answer stands out by a bracket. The German title goes
  in brackets only for the laws whose glossary row carries it (AFuG, AFuV,
  TKG, TTDSG, FuAG, and the repealed
  *Frequenznutzungsplanaufstellungsverordnung*, VD701); the other
  statutes and ordinances take the glossary's English name with the
  abbreviation — "Frequency Ordinance (FreqV)", "Federal Immission Control
  Act (BImSchG)", also where the German leaves the abbreviation out
  (VE511 d) — and a law the bank never abbreviates keeps its English name
  alone ("Administrative Enforcement Act", VE704). Where the German writes
  only the abbreviation (AFuG, AFuV, TKG, EMVG, BEMFV), so does the
  English. One law, one name across the whole bank. (Batch 10; scope
  stated by the checker.)
- ***verschlüsseln … zur Verschleierung* is *encrypt* in German law,
  *encoded* in the RR.** The AFuG / AFuV questions (VC124 d, VD103 a,
  VD104) say "encrypt(ed) … to obscure the content / its meaning": German
  statutes are translated faithfully, and the German means cryptography.
  The RR 25.2A question (VA303) keeps the RR's own "encoded for the purpose
  of obscuring … meaning". (Batch 10.)
- **"What does the German abbreviation X stand for?"** (VE501, EMVU): each
  answer that expands the abbreviation is translated and followed by the
  German expansion in brackets — "Electromagnetic compatibility with the
  environment (Elektromagnetische Verträglichkeit in der Umwelt)" — so the
  English reader can match the letters as the German reader does. Such a
  bracket adds information (bracket rule above) and goes with every
  expansion, the correct one and the distractors alike; an answer that is a
  description rather than an expansion (VE501 d, a citizens' initiative) is
  only translated. The counterpart of the EF212 rule for English
  abbreviations. (Batch 10.)
- ***Nachprüfung* as a sanction → re-examination** (VC122 *fachliche
  Nachprüfung* → "re-examination of competence"; VC123, VC125, VE704 bare
  *kosten-/gebührenpflichtige Nachprüfung* → "re-examination subject to a
  fee"). The glossary's earlier "inspection subject to a fee", written
  before any question used it, presumed that the station is what gets
  checked; *fachliche* in VC122 shows it is the person's competence, and
  "re-examination" covers the bare word without deciding more than the
  German. (Batch 10.)

## Course text

- **Numbered references are capitalised: *Figure*, *Table*.**
  *Abbildung [ref:…]* and *Bild [ref:…]* both become "Figure [ref:…]",
  *Tabelle [ref:…]* becomes "Table [ref:…]": the reference renders as a
  number, and English capitalises a numbered float. (Unit
  nea_erste_schritte.)
- **The pronunciation column of the phonetic alphabet uses the ITU's
  English respelling** (RR Appendix 14, as in the ICAO table): AL-FAH,
  BRAH-VOH, CHAR-LEE … KEH-BECK … ZOO-LOO, upper case with hyphens like the
  German. The German column (BRA-WO, TSCHA-LI, KWE-BECK) respells for German
  readers and would mislead an English one; as with Q codes, the
  established English wording of the same ITU list is used rather than a
  fresh respelling. Where the ITU gives two forms (Charlie, Uniform), the
  first. (Unit nea_erste_schritte, tables n_buchstabiertafel,
  n_buchstabiertafel_1/_2.)
- **On-air phrases in `<qso>` and in quoted calls use English voice
  procedure**, in the wording the exam questions already use: *hier ist* →
  "this is", *bitte kommen* → "over" (BE102), *Ist diese Frequenz frei?* →
  "Is this frequency in use?" (BE105 *besetzt* → "in use"), *wurde ich
  gerufen?* → "was I called?" (BE103). A German phrase the text quotes *as*
  German usage ("Allgemeiner Anruf") stays German with the English in
  brackets; digits spoken in German on national contacts (*Vier*) stay, as
  the text itself explains. A German gloss that only translates an English
  word back into German (*seek you, also "suche dich"*; *push to talk,
  also "drücken, um zu senden"*) is dropped, as in the bracket rule above.
  (Unit nea_erste_schritte.)
- **English names the German glosses are not glossed back.** Where the
  German text pairs an English name with its German counterpart, the
  bracket rule above applies to whole rows and list items as well. In the
  frequency-range table (frequenzspektrum, table
  n_frequenzspektrum_bereiche, section and slides) the German everyday
  names *(Kurzwelle) (KW)*, *(Ultrakurzwelle) (UKW)* and
  *(Dezimeterwelle)* only repeat the English row above them and are
  dropped, as in BC101–BC106; *(Langwelle) (LW)* and *(Mittelwelle) (MW)*
  become "(Long Wave) (LW)" and "(Medium Wave) (MW)", the English everyday
  names, capitalised like the other names in the table, and "Short Wave SW"
  stays. In the IARU band plan sections the
  German names the band plan's English labels in brackets ("Baken
  ("beacons")"); where the label is the English term itself the bracket is
  dropped ("Beacons"), where it differs it stays ("FM voice ("FM
  calling")", "Morse telegraphy ("CW")"). (Unit
  nea_elektrische_schwingungen_funkwellen.)
- **Ionosphere: *Region* → region, *Schicht* → layer, word for word.**
  The course text uses both and says why ("Diese Gebiete werden als
  *Regionen* bezeichnet (manchmal auch als "Schichten")", ionosphaere_2):
  the exam questions and most of the prose say *Region*, the slides and
  some paragraphs *Schicht* (D-Schicht, F2-Schicht, sporadische E-Schicht).
  The English follows the German in each place — "D region", "D layer",
  "sporadic E layer" — rather than evening them out. The earlier entry
  (*region*, not the RSGB's *layer*) concerns the questions, which only say
  *Region*. (Unit nea_wellenausbreitung_1.)
- **Spoken call signs in examples use English voice procedure too.** The
  table of spoken call sign suffixes (rufzeichenzusaetze, section and
  slides) gives German national usage — *Delta Lima Eins Foxtrott Lima
  Oskar (Stroke) Mobil*. In English it is "Delta Lima One Foxtrot Lima
  Oscar (Stroke) Mobile": digits in English, the ITU spellings of the code
  words where the German uses its own (*Foxtrott*, *Oskar*), and the
  suffixes spoken as English operators say them — "Stroke Portable",
  "Mobile", "Maritime Mobile", "Aeronautical Mobile"; "Stroke", "Remote"
  and "Trainee" are English already. This extends the `<qso>` entry above
  to quoted call signs. German digits (*Vier*) stay only where the text
  itself says it is showing German national usage (buchstabiertafel).
  Spellings the German shares with English usage (*Alpha*, *X-Ray*) are
  kept as written. (Unit nea_amateurfunkstationen.)
- **German mnemonics keep their German words, with the English meaning
  in brackets.** The country-prefix tables (internationale_landeskenner,
  section and slides) give German *Eselsbrücken* — *Keiner Will Nach
  Amerika* (K, W, N), *Viele Elche* (VE), *Schwedische Möbel* (SM). They
  work through the letters of the German words, and a made-up English
  mnemonic would be an addition, not a translation; so the German stays
  and the English reader gets its meaning: "Keiner Will Nach Amerika
  (nobody wants to go to America)". Where the mnemonic is only the
  country's name and the English name spells the same letters, the English
  name is used (*Frankreich* → France, *Großbritannien* → Great Britain,
  *mEXiko* → mEXico); mnemonics already in another language (*CosTa*,
  *EspaniA*, *JApan*, *Zea-Land*) stay, and German glosses inside them are
  translated (*CosTa (Küste)* → "CosTa (coast)"). (Unit
  nea_internationaler_funkbetrieb.)
- **Formula-sheet keywords: English, with the German keyword in
  brackets.** The course text points to entries of the formula sheet
  ("siehe Formelsammlung – Stichwort: Induktivität einer Ringkernspule").
  The formula sheet used in the examination is the German one, so the
  reader has to find the German entry: "see the formula sheet – keyword:
  inductance of a toroidal coil (*Induktivität einer Ringkernspule*)". The
  English says what the entry is about, the bracket is what to look for.
  A bare "(vgl. Formelsammlung)" stays "(see the formula sheet)". (Unit
  nea_bauelemente_1.)
- **German memory rhymes are kept, with the English meaning in
  brackets**, as the country-prefix mnemonics above: *Beim
  Kondensatooor eilt der Strom vooor!* → the same, followed by "(in the
  capacitor, the current leads)"; *Bei der Induktivitääät kommt der
  Strom zu spääät!* → "(in the inductance, the current comes too late)".
  The rhyme is the point of the mnemonic and cannot be translated; an
  established English mnemonic (such as *CIVIL*) would be an addition,
  not a translation. (Unit nea_bauelemente_1.)
- ***Akku* is a *rechargeable battery* where the German sets it against
  *Batterie*, and a plain *battery* where only rechargeable batteries are
  meant.** German has two everyday words — *Batterie* (single use) and
  *Akku* (rechargeable) — and English one. Where the text contrasts them
  (batterien_und_akkus: "Batterien … sind nur einmal verwendbar", "Akkus,
  manchmal aber auch Batterien"), *Akku* → "rechargeable battery" and
  *Batterie* → "battery", or "non-rechargeable battery" where the contrast
  would otherwise be lost, as ND110 ("rechargeable and non-rechargeable
  batteries") and NK306 do. Where the text is about rechargeable batteries
  throughout (akku: LiFePO4, 4S1P, balancer), *Akku* → "battery", by the
  glossary's house-style rule *Akku → battery* and as AB209 ("battery") and
  AB210 ("battery pack") have it, once the first mention has said
  "rechargeable"; *Akkumulatoren, kurz Akkus genannt* → "accumulators, or rechargeable
  batteries as they are usually called". (Unit
  nea_strom_spannungsversorgung_1.)
- **A remark that only a German reader needs is kept as information about
  German usage, not dropped.** The SSB section warns that *USB* does not
  stand for *unteres Seitenband* (the lower sideband) but, after the
  English name, for the upper sideband; for an English reader the
  abbreviation is self-evident. Since the course is the German one in
  English, the remark stays and says what it is about: "In German, the
  common abbreviation *USB* is easily taken for the lower sideband
  (*unteres Seitenband*); it stands, as the English name says, for the
  *upper sideband*!" (section and slides of ssb), as the glossary's
  *Relais oder Repeater* row keeps "In German, repeaters … are also
  called *Relais* or *Repeater*". Where the German only glosses the English
  term ("Im Englischen wird von "lower sideband" (LSB) … gesprochen",
  "gebräuchlicher ist die englische Bezeichnung single-sideband
  modulation"), the bracket rule applies and the gloss is dropped. (Unit
  nea_modulation.)
- ***Oberwelle* against *Harmonische* in the course text: *overtone*.**
  The section on non-sinusoidal signals (nicht_sinus_signale, section and
  slides) sets the two German words against each other — the 1st
  *Oberwelle* is the 2nd *Harmonische* — and counts them differently. English
  needs two words for that, so *Oberwelle* becomes *overtone* there, and the
  German words are named once ("*overtones* (in German *Oberwellen* or
  *Oberschwingungen*)") so that the reader can match the trap in AB402, whose
  stem already says "third overtone (Oberwelle)". Where *Oberwellen* only
  means unwanted multiples of a frequency (filters, harmonic content on a
  spectrum analyser, AI614 "harmonics"), it stays *harmonics*, as the
  glossary says. The formula subscript $f_\mathrm{Oberwelle,N}$ stays. (Unit
  nea_sender_1.)
- **Column headings of Annex 1 to the AFuV: English, with the German heading
  in brackets.** The course tells the reader to read values from the columns
  *Frequenzbereiche*, *Maximale Leistung* and *Zusätzliche
  Nutzungsbestimmungen gemäß B* of Annex 1, which is the German examination
  aid. As with the formula-sheet keywords, the English says what the column
  is, the bracket what to look for: "the column "Maximum power" (*Maximale
  Leistung*)". (Unit nea_sender_1, ausgangsleistung.)
- ***Störung* against *störende Beeinflussung*: *interference* / *breakthrough*.**
  The course text sets the two apart (stoerungen_vermeiden): a *Störung* is
  present when the amateur station radiates unwanted frequency components
  beyond the limits; a *störende Beeinflussung* when the limits are kept and
  the affected equipment is still upset by the wanted signal, through
  radiated pick-up via its antenna, direct pick-up or conducted pick-up.
  English needs two words for that. *Breakthrough* is the RSGB's established
  term for exactly the second case (glossary §12), and *interference* stays
  for the first. The German words are named once where the distinction is
  introduced: "a distinction is made between interference (in German
  *Störung*) and breakthrough (*störende Beeinflussung*)"; the slide heading
  *Störende Beeinflussung* is "Breakthrough", and *Übersteuerung oder
  störende Beeinflussung* "*overloading* … or *breakthrough*"
  (stoerungen_elektronischer_geraete_1). Plain *Beeinflussung* /
  *beeinflussen*, without *störend*, is *effect* / *affect*. The exam
  questions stand alone and never set the two against each other, so the
  bank's *interference* for *störende Beeinflussung* (EJ103 "overloading or
  interference", EJ110, EJ112, AJ108, AJ111) stays. (Unit nea_sender_2.)
- **Tables of operating abbreviations: the meaning in English; a
  "(vom Englischen …)" that only gives the meaning back is dropped, an
  origin that is not the meaning stays.** The German tables explain each
  abbreviation in German and add its English source: *PSE – Bitte (vom
  Englischen "Please")*, *TNX – Danke (vom Englischen "Thanks")*, *VY – sehr
  (vom Englischen "very")*, *RPRT – Rapport (vom Englischen "Report")*. In
  English the meaning *is* that word, so the cell reads "Please", "Thanks",
  "Very", "Report" — the bracket rule above, applied to table cells. Where
  the bracket says something the meaning does not, it stays: CQ "General
  call (from "seek you")", SK "End of contact (from "Silent Key")", UR "You
  are (in the sense of "your signal is")". Plain-language renderings of a
  telegraphy QSO (slide fragments) use English voice procedure as the
  `<qso>` entry above: *DL2AB von DL1PZ - Kommen!* → "DL2AB, this is DL1PZ –
  over!". The same tables recur in the operating chapters and follow this.
  (Unit nea_digitale_uebertragungsverfahren_1, funkfernschreiben.)
- **Labels in the applets: English, with the German label in brackets.**
  The interactive applets (`contents/html/applet_*.html`) are still German,
  and the course text and slide notes name their controls ("Mit „Erneut
  übertragen" wird derselbe Bitstrom nochmals … übertragen", psk slides). As
  with the formula-sheet keywords and the columns of Annex 1 to the AFuV, the
  English says what the control does and the bracket is what the reader has to
  find on the screen: 'The button "Transmit again" (*Erneut übertragen*)
  transmits the same bit stream once more'. When the applets are translated,
  the bracket goes. A control described without its label ("the slider on the
  right-hand side", modulatoren) is simply translated. (Unit
  nea_digitale_uebertragungsverfahren_2, psk.)
- ***Verkürzungsfaktor* in the course text: *shortening factor* for
  antennas, *velocity factor* for lines and cables**, as in the exam
  questions (AG101–AG105, EG202 against EG201, AG313, AG315, AG316). German
  has one word, and the course treats it as one quantity: verkuerzungsfaktor_1
  introduces it for "Leitungen, einschließlich Antennendrähten", defines it
  as a ratio of velocities (EG201 "velocity factor") and then applies it to
  wire antennas (EG202 "shortening factor"). There the English names it once
  with both terms and the German word: "the *velocity factor* $k_\mathrm{v}$
  (for antennas usually called the *shortening factor*; German has one word
  for both, *Verkürzungsfaktor*)", on the slide "(for antennas: *shortening
  factor*)". Everywhere else each place takes the term for what it is about:
  antenna lengths, the cause of the factor (wires not infinitely thin), the
  dipole slide note and the loop's counterpart → *shortening factor*;
  open-wire lines and coaxial cables → *velocity factor*. The loop
  antenna's *Verlängerungsfaktor* is the *lengthening factor* (glossary §14).
  (Unit nea_antennen_uebertragungsleitungen_1.)
- **Words written as a quantity in a worked formula are translated; letter
  symbols derived from them stay.** The front-to-back slides
  (vor_rueck_verhaeltnis) write the ratio itself as words,
  $\frac{Vor}{Rück}$; in English it is $\frac{Front}{Back}$, as the
  abbreviated word $\textrm{Abw.}$ became "Dev." (glossary §14). The
  single-letter symbols taken from the same words — $P_V$, $P_R$, $U_V$,
  $U_R$ — stay, because the exam questions (AG213, AG214) and the drawings
  use them, like every other German subscript. (Unit
  nea_antennen_uebertragungsleitungen_2.)
- **Coaxial connectors: *Stecker* → plug, *Kupplung* → socket, *Buchse* →
  panel socket, *Einbaustecker* → panel plug.** German has three words for
  the parts of a connector and the course defines them (koaxsteckverbinder):
  the *Stecker* is male, the *Kupplung* female, and a *Buchse* or
  *Einbaustecker* is a *Kupplung* or *Stecker* built into equipment. The
  glossary's *Buchse* → socket therefore becomes *panel socket* where the
  course sets it against the *Kupplung* (PL-Einbaubuchse,
  N-Einbaubuchse), and *Kupplung* takes plain *socket*; a bare *Buchse*
  with no contrast stays *socket* ("N-Buchse" → "N socket"; the reverse SMA
  slide's "Reverse-SMA-Stecker ist eine Buchse", which only means
  "female", → "a reverse SMA plug is a socket"). *Jack*, the RF industry's
  word for the female part, is not used: in British English a *jack* is also
  the male audio plug. Where *Stecker* names the connector type rather than
  the male part (*N-Stecker: für … hohe Leistung*), it is *connector*, as in
  EG303. The connector chapters that follow (e.g. swl_steckverbinder) keep
  this. (Unit nea_antennen_uebertragungsleitungen_3.)

## Open questions for DARC

- Suspected slips in the German original noticed while translating are listed
  in each batch's notes; they are translated faithfully, not corrected, and
  collected for DARC separately.
