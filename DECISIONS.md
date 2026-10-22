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

## Open questions for DARC

- Suspected slips in the German original noticed while translating are listed
  in each batch's notes; they are translated faithfully, not corrected, and
  collected for DARC separately.
