# pitanja_06 — translation report

175 questions (AG101–AG115, EG1, NG1, AG2, EG2, AG3, EG3, NG2, AG4, EG4,
NG304, NG305), 871 fields (EG214 has picture answers, so only its stem is
text). `qbank-prevedi.py`: 0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §9, notes on existing rows: *Verkürzungsfaktor (Antenne)* → shortening
  factor in exam questions; *Umwegleitung* → "(λ/2 / half-wave) delay line"
  where λ/2 is given or *Balun* stands beside it; *Mantelwellen* → "sheath
  currents" in AG425; *stromkompensierte Drossel* → "current-compensated
  choke" in AG426; *Strom-/Spannungsbauch* → antinode / node where paired
  with *Knoten*; *Zweidrahtleitung / Hühnerleiter / Paralleldrahtleitung* →
  twin feeder / ladder line / open-wire line as used here; *Halbwertsbreite
  (Öffnungswinkel)* → half-power beamwidth (beam angle).
- §9, new rows: *Mantelstrom* → sheath current; *Spannungs-Balun* → voltage
  balun; *Eingangswiderstand (Antenne)* → input impedance; *Stege / Spreizer*
  → spacers; *Flachbandkabel* → ribbon feeder; *Transformationsleitung* →
  transformer section; *Leitungsstück (Stub)* → length of line (stub);
  *Voll-PE / PE-Schaum / Massivschirm / Abschirmgeflecht*; *Cubical-Quad*;
  *magnetische Ringantenne* → magnetic loop antenna; *Ferrit(stab)antenne*;
  *Patch- / Schlitzantenne*; *Sperrtopfantenne* → sleeve dipole;
  *Winkeldipol* → inverted-V dipole; *Schleifendipol* → loop dipole;
  *Ringdipol*; *Saugkreis-Dipol* → acceptor-circuit dipole;
  *Gleichwellenfilter* → common-wave filter; *Dreiband-Dipol*;
  *Kurzwellenbeam* → HF beam; *Horizontaldiagramm* → horizontal radiation
  pattern; *Strahlungsdichte* → power density.
- §13: *Erdoberfläche mittlerer Leitfähigkeit / Erdboden* → ground of
  average conductivity / the ground; *Dämpfungsmaß* → attenuation;
  *Kabelkanal* → cable duct; *Spannungsüberschlag* → flashover; *Dachboden*
  → loft; *Cinch* → RCA (phono); *Pertinax*; *HF-Übertrager (Balun)* → RF
  transformer (balun).

## Added to `DECISIONS.md`

Antenna *Verkürzungsfaktor* → shortening factor in questions; the "no echo
the German does not have" rule (AG425, AG426, EG201); *Mantelstrom* →
sheath current; antenna *Eingangs-/Fußpunktwiderstand* → impedance;
*Cinch* → RCA (phono).

## Judgement calls

- EG201: the stem says "shortening factor" although answer a defines the
  cable's velocity factor; "velocity factor" in the stem would echo "velocity
  of propagation" in a, which the German *Verkürzungsfaktor* does not.
- AG425: *Mantelwellen* → "sheath currents" so that a ("common-mode
  components") is not echoed; AG426: *stromkompensierte Drossel* →
  "current-compensated choke" for the same reason.
- EG404 a / AG428: *Mantelstrom* → "Sheath current"; the distractors
  *Rückwärts-/Potential-/Phantomstrom* → "Reverse/Potential/Phantom current".
- AG420 a: *Umwegleitung oder Balun* → "a half-wave delay line or a balun",
  to avoid "a … balun or a balun"; AG423, AG424: "$\lambda$/2 delay line".
- AG423 b/d: *Schleifendipol* (a synonym of *Faltdipol*) → "loop dipole",
  kept apart from "folded dipole" in a, as the German changes the word.
- AG109 c: *Gleichwellenfilter* (made-up, beside *Oberwellenfilter*) →
  "common-wave filter"; d *Saugkreis-Dipol* → "Acceptor-circuit dipole",
  beside a "Trap dipole".
- AG108: *zweimal 15 m langen Dipol* → "with two legs of 15 m each";
  AG421: *aus zweimal acht Windungen* → "with two windings of eight turns".
- AG106, AG108: *Spule* in an antenna → "coil" (a loading coil).
- AG203–AG206, AG111–AG113: *erregt / Erregung* → "fed" (glossary);
  *Erregerfrequenz* → "feed frequency".
- AG209: *zeigt sich … als* → "appears … as"; *Wirkwiderstand* → "a
  resistance".
- AG207, AG208, AG413–AG415: *niederohmig / hochohmig* of an impedance →
  "of low/high impedance", "low/high"; AG409/AG410 "Very high"; AG411 d
  "almost infinitely high".
- AG223, AG224: *Erdoberfläche / Erdboden* (soil) → "ground"; *earth* kept
  for earthing (AG301 d, AG312, AG424, AG428 d).
- AG219 c: *Strahlungsdichte* → "power density".
- AG202 b: *Idealform des Kugelstrahlers* → "the ideal shape of the
  spherical (isotropic) radiator", so the link to "ideal spherical shape" in
  the next sentence survives.
- EG112: *HF-Richtantenne* → "directional antenna" (German HF = RF; "RF
  directional antenna" adds nothing in English).
- EG113: *Erregerantenne (Feed)* → "feed antenna" (the bracket only gives the
  English word); stem ends "consists of ..." with the article in each answer.
- EG212: *Energieeinspeisung* → "is the power fed"; answers keep the
  German's lack of full stops.
- EG213 d: German starts lower case (*mittengespeister*); capitalised.
- NG110: *2 m-QSO-Runde* → "2 m net" (glossary *Funkrunde*).
- NG111 d: *Dachboden* → "loft".
- NG206: *Cinch* → "RCA (phono)"; b "UHF and BNetzA" kept as the joke
  distractor it is.
- AG318 d: "Dunning–Kruger effect" kept, a joke distractor in the German.
- AG302 b: *Pertinax* kept (trade name).
- NG208 b/c: *verstärkt* of the reflected signal → "increases".
- Suspected slips in the German, translated normally: AG209 *Fusspunkt-*
  (Swiss spelling of *Fußpunkt-*); AG303 d *Rückflußdämpfung* (old
  spelling); NG208 c lacks a full stop (added); EG223 b *Ausstrahlungen
  unterworfen* is odd German, rendered "subject to radiation". Whitespace in
  the German, all dropped: trailing spaces in AG109, EG107, EG104,
  NG203–NG205, AG408, AG401 (questions); final newlines in AG309 c, AG424 a;
  double spaces in EG102 d, AG406 c.

## Provjera

175 questions checked (871 text fields; EG214's answers are pictures), German
from `upstream/main` beside the English. 17 fields in 15 questions changed via
`pitanja_06.provjera.json`, applied with `--retranslate`: 0 refused,
0 warnings. By kind: answer correctness 3 (AG423 b/d, EG201), terminology /
glossary 9, meaning 1 (AG427 c), style 4; glossary 7 rows fixed,
DECISIONS.md 2 entries reworked.

- AG423 b, d: *Schleifendipol* → "folded dipole", not "loop dipole". It is a
  plain German synonym of *Faltdipol*, and "loop dipole" is not an English
  term; b/d must be wrong for the German reasons (a folded dipole is not
  60 Ω; d's arrangement is not a filter), not because of an invented word.
- AG423 d: *koaxialer Leitungskreis, der als Sperrfilter* → "coaxial line
  resonator used as a band-stop filter" (was "line circuit … stop filter").
- EG201 question: "shortening factor" → "velocity factor". The answer defines
  the cable/line factor, whose only English name is velocity factor; in
  English "shortening factor" is the antenna end effect, which makes
  distractor b (diameter to length) look right. The echo with "velocity of
  propagation" in a is inherent in the English term, not added.
- AG426 question: *Mantelwellen* → "sheath currents" (was "common-mode
  currents"), as in AG425: the stem still echoed "common-mode components" in
  a, which the translator's no-echo rule was meant to prevent.
- AG111 b, AG112 a, AG113 b, AG203–AG206 questions: *Erregerfrequenz* →
  "operating frequency"; "feed frequency" is not English usage.
- AG109 c: *Gleichwellenfilter* → "common-frequency filter"; *Gleichwelle* is
  "common frequency" in English, "common-wave" exists nowhere. Still a
  made-up filter, as in German.
- AG424 a, c: "2 times 120 Ω to earth" → "2 × 120 Ω to earth".
- AG427 c: *geflochtenem Mantel* → "braided screen"; "braided sheath" reads as
  the outer jacket.
- AG304 question: "is operated matched when" → "is matched when".
- EG113 question: *scharf bündelnde Antenne* → "highly directional antenna"
  (was "sharply focusing").

Flagged points: AG423 and EG201 corrected as above. DECISIONS.md: the antenna
"shortening factor" entry kept for AG101–AG105/EG202 (clear, and what the
German says), but now states that a cable or line factor is always the
velocity factor, EG201 included; the "no echo" entry narrowed — the
alternative must itself be established English for the same thing, and the
established term wins where it is the only accurate one (EG201 removed,
AG426 stem added). The other three new entries (*Mantelstrom*, antenna input
impedance, *Cinch*) are sound. Glossary: *Schleifendipol* → folded dipole;
*Gleichwellenfilter* → common-frequency filter; *Erregerfrequenz* →
operating frequency; antenna *Verkürzungsfaktor* note no longer sends EG201
to "shortening factor"; *Mantelwellen* note adds AG426; *Sperrtopfantenne* →
sleeve dipole confirmed (coaxial sleeve antenna, note expanded);
*Saugkreis-Dipol* → acceptor-circuit dipole confirmed (RSGB *acceptor*,
series-resonant, beside *trap dipole*); *Strahlungsdichte* → power density
confirmed (W/m², RSGB exposure usage). Left as is: "radiator" for the Yagi
*Strahler* (EG111, EG212 — "driven element" would echo "fed" in EG212),
"delay line" for *Umwegleitung* where λ/2 or *Balun* is given.
