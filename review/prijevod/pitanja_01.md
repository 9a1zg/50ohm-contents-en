# pitanja_01 — translation report

175 questions (NA1, AA1, EA1, NA2, EA2, AB1, NB1, AB2, NB2, EB1–EB5, NB3–NB6,
AB3–AB5), 855 fields. `qbank-prevedi.py`: 0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §3: metals and insulating materials (*Wolfram* → tungsten), boron /
  phosphorus / bismuth / tellurium; *Amperesekunde* → ampere-second;
  *Teile einer Frequenz / Unterschwingungen* → submultiples / subharmonics.
- §4: *Verarmungszone* → depletion region; *Dotierungsatome* → dopant atoms;
  *N-/P-leitend* → N-type / P-type; *Elektronenlöcher* → holes;
  *Metallbeläge* → metal foils; *Belastungsnennwert* → power rating.
- §5: *Durchlassdämpfung* → passband loss (insertion loss).
- §9: *rechts-/linksdrehend, rechts-/linkszirkular* → right-/left-hand circular.
- §11: *Schirmbild* → screen display; *Messsender* → signal generator.
- §13: *Leistungsaufnahme / Stromaufnahme / Stromentnahme* → power
  consumption / current drawn; *häusliche Spannungsversorgung* → domestic
  mains supply.

## Judgement calls

- Unit names as answers are lower case (*ohm*, *hertz (Hz)*, *baud (Bd)*),
  following the glossary's "lower case as unit names", even where the answer
  stands alone (AA101–AA104, EA101–EA106, NA201–NA206).
- *Ohm* written as a word after a number became *ohm/ohms* (AB101, AB205–AB208,
  NB505, EB5xx); *kOhm*/*MOhm* became *kΩ*/*MΩ* (EA112, EB510, EB511), as the
  German uses them as unit symbols. AB208 keeps the German mix of *mΩ* and
  *ohms* across its answers.
- AA116: the display reading *14,200.000 MHz* is kept as *14.200.000 MHz*
  (transceiver-display style); the number guard needs the grouping as is.
- NB401, AB404–AB407: picture answers have empty text; only the question was
  translated (the tool refuses empty fields).
- AB402: *Oberwelle* rendered "the third overtone (Oberwelle)", as the
  glossary prescribes, so that "fourth harmonic" stays the correct answer.
- AB108: *N-Teil / N-Seite* both rendered "N-type side"; *Grenzschicht* →
  junction, *Grenzfläche* → boundary.
- AB211: the German stem's word order ("bis dieser … entladen ist und einen
  Strom von 0,8 A aufnimmt") was rearranged so that the 0.8 A clearly belongs
  to the receiver.
- EB501/EB502: definitions worded after RR 1.157 / 1.158 (*average power
  supplied to the antenna feed line … at the crest of the modulation envelope*)
  while following the German sentence by sentence.
- NA213: *Perioden pro Sekunde* → "cycles per second"; the distractor unit
  "pps" kept as in the German.
- Suspected slips in the German, translated normally: NA203 "den elektrische
  Widerstand" (grammar); AB210 stem ends with "." instead of "?"; AB408
  answer c lacks a final full stop (added in English for parallelism).
