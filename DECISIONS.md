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
  (Batch 07.)
- **The German generic *er* for a radio amateur** ("Er muss die Antenne
  drehen …", "erkennt er, dass …") is recast without a pronoun — "The
  antenna must be turned to …", "that "PY" has been worked" — or, where a
  pronoun is unavoidable, singular *they* (AH305). (Batch 07.)

## Open questions for DARC

- Suspected slips in the German original noticed while translating are listed
  in each batch's notes; they are translated faithfully, not corrected, and
  collected for DARC separately.
