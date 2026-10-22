# pitanja_05 — translation report

175 questions (AF2 AF201–AF223, EF2, NF3, AF3, EF3, NF4, AF4, EF4, AF5, EF5,
AF6, EF6, AF7, AG116–AG127), 811 fields (16 questions have picture answers,
so only their stem is text). `qbank-prevedi.py`: 0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §5: *Unterbrechungsfreie Spannungsversorgung* → uninterruptible power
  supply; *Arbeitswiderstand* → load resistance; *Schwingungseinsatz* → start
  of oscillation; *Verachtfacher / Vervielfachungskombination* → eight-times
  multiplier / sequence of multipliers.
- §6: *Grenzempfindlichkeit* → minimum discernible signal; *Interception
  Point* → intercept point; *Noise-Blanker / Störaustaster* → noise blanker;
  *Rauschunterdrückung (Noise Reduction)* → noise reduction (NR);
  *Clarifier*; *Gleichlauf(steuerung)* → ganging (control); *digitaler
  Direktempfänger* → digital direct-sampling receiver; *Empfangszweig /
  Sendezweig* → receive / transmit path; *Durchlasskurve* → passband curve;
  *Antennenvorverstärker*; *Eintakt-Transistormischer / Dualtransistormischer*;
  *Hilfsträger* → auxiliary carrier; *Endstufenröhre / Endstufentransistor*;
  *Ausgangsanpassschaltung*; *Stromzufuhr* → power feed; *Wärmeleistung* →
  power dissipated as heat; *Bedienteil* → control unit; *Remote-Tuner*;
  *Kontrollseite / Remoteseite* → control site / remote site; *IP-Steckdose*
  → IP-controlled mains socket.
- §7: *Ein- oder Zweitonaussteuerung* → single-tone or two-tone drive.
- §8: *Alias-Effekt / Anti-Alias-Filter*; *Abtastratengenerator* → sampling
  clock generator; *Abtastergebnis* → sampled result; *Taktzittern (Jitter)*
  → clock jitter; *Schrittweite* → step size; *Amplitudengang / Frequenzgang*;
  *Raummultiplexing* → space-division multiplexing; *digitaler Sprechfunk /
  DATV*.
- §9: *rotationssymmetrischer Parabolspiegel*; *Verzögerungsleitung /
  Transformationsstück* → delay line / transformer section;
  *Zweibandantenne* → dual-band antenna (as *Zweiband-Dipol*); *Abspannung*
  → guying.
- §10: *NVIS*. §13: *Draufsicht* → plan view; *Korrekturfaktor*.

## Added to `DECISIONS.md`

"What does the abbreviation X stand for?" — a faithful distractor that also
fits the letters is preferred (EF212); *symmetrisch* on a circuit block is
*balanced*, only the attenuator is *symmetrical* (AF306).

## Judgement calls

- AF223, EF216, EF307, AF601–AF604, AF612–AF614, AF623, AF625–AF629:
  picture answers have empty text; only the question was translated.
- EF212: German answers are German terms, none spelling AGC; in English
  "Automatic gain control" spells it. *Automatische Gleichlaufsteuerung* →
  "Automatic ganging control" (faithful: *Gleichlauf* of tuned circuits is
  ganging/tracking) also spells AGC, so the correct answer does not stand out
  alone. b "Automatic antenna tuner", d "Automatic frequency correction".
- AF306 b: *symmetrisches Filter* → "Balanced filter", as tempting beside
  "Balanced mixer" as *symmetrisch* beside *Balance-* is in German.
- AF221: *Interception Point IP$_3$* → "intercept point IP$_3$";
  *Grenzempfindlichkeit* → "Minimum discernible signal" (the recognised
  English receiver spec, so the distractor stays as plausible).
- AF305: stem ends "is ..." and each answer carries its own article
  ("a crystal filter …", "an RC high-pass filter …"); the German quote macro
  `\glqq?"` has to stay (the tool keeps LaTeX commands), so the "?" label
  renders with German quotation marks.
- AF412, AG124: articles moved into the answers for the same reason (an
  oscillator / an end-fed …).
- AF201: *HF-Nutzfrequenz* → "wanted radio frequency" (not "RF frequency").
- AF204 a: *Vorselektion* → "The preselection" (glossary *preselector*;
  the German names the function, not the unit, as c names the IF selectivity).
- EF401: the German stem breaks inside the phrase (*die unmittelbar nach …*);
  English stem "is the ..." with "immediately after …" moved into each
  answer.
- AF631: "Digital filters ..." with "can be …" / "cannot be …" in the answers,
  so each answer reads as a full statement.
- AF616 b–d: identical German to AE416 b–d; English copied word for word, a
  made parallel ("… required to reconstruct a signal without errors").
- AF415 d: German *weil er sonst …* — "er" read as the electrolytic capacitor
  and written out ("the electrolytic capacitor would be destroyed").
- AF706: *durch ihre eigene Aussendung* read as the remote station's own
  transmission ("Its own transmission causes …"), not a slip for *Ihre*.
- AF707: *Kontrollseite / Remoteseite* → "control site / remote site", kept
  apart from *remote end* (*Gegenstelle*).
- AF301 d: *Verachtfacher* → "eight-times multiplier" (no digit in the German,
  so none in the English); *Frequenzteiler durch 3* → "divide-by-3 frequency
  divider".
- AF314: *Vervielfachungskombination* → "sequence of multipliers" (the order
  of the factors is what distinguishes the answers).
- AG125: German *Near Vertical Incident Skywave* → "near vertical incidence
  skywave", the established English expansion.
- AG126 d: *in der Draufsicht ein liegendes Kreuz* → "a diagonal cross (X) in
  plan view".
- AG116: *Zweibandantenne* → "dual-band antenna", as the glossary's
  *Zweiband-Dipol*.
- AG120–AG122: *Zeppelin-Antenne* → "Zepp antenna" (glossary).
- EF306, AF306: *Dynamic Compressor* / *Dynamikkompressor* → "Compressor"
  (glossary).
- EF505: *Abweichung* → "frequency error", so it is not read as FM deviation.
- AF313 c: *unbedingt* → "should always", parallel with the other three
  "should" answers.
- Suspected slips in the German, translated normally: AF311 a–d *die
  gewünschte Oberschwingungen* (should be *gewünschten*); EF306 *eines
  Sprachsignale* (should be *Sprachsignals*); AF427 *Wärmeleistung … in Wärme
  umgesetzt* (redundant); AF313 c lacks a full stop (added); AF502 b contains
  a line break (dropped). Whitespace in the German, all dropped: trailing
  spaces in AF222 (q, a), AF217 d, AF215 d, AF212, AF202 c, EF208 d, EF207 d,
  EF206 d, AF314, AF309, EF310 a–d, EF304 b/d, AF410 a, AF407 a/b,
  AF406 b–d, AF404 d, AF403 b, EF405 d, EF403, EF505 a–d, AG120–AG122;
  final newlines in NF403 b/d, EF404 a/c; double spaces in AF222, AF314,
  AF309, AF406, AF401 d, EF403, AG127 d, AG120–AG122 and NF403; non-breaking
  spaces in AF631, AF618, AF707 d, AF706, AF705 (q, b), AF703, AF702. NF403
  keeps its line breaks between the six positions, normalised to "; \n".
