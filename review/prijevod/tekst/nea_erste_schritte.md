# nea_erste_schritte — translation report

Chapter "Erste Schritte" (First steps): 9 sections, each with its slides, no
solutions. 18 files:

- `contents/sections/` and `contents/slides/`: `erste_schritte.md`,
  `rufzeichen.md`, `buchstabiertafel.md`, `betriebsabwicklung.md`, `rst.md`,
  `ausbildungsfunk.md`, `offene_sprache.md`, `nur_mit_afu_stellen.md`,
  `gewerblich.md`.

`revizija-guard.py --brojevi`: 18 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (*Vier*, "Allgemeiner
Anruf", the `%TODO` comment).

## Added to `TRANSLATION_GLOSSARY.md` (§14)

*Grundrechenarten / Dreisatz*, *Kofferwort*, *PTT-Taste / Handmikrofon*,
*Abbildung / Bild / Tabelle [ref:]*, *Aussprache (Buchstabiertafel)*, voice
procedure in `<qso>` (*hier ist*, *von*, *bitte kommen*, *und hört*), *Ist
diese Frequenz frei?*, *Wer zuerst kommt, mahlt zuerst*, *Lesbarkeit /
Verständlichkeit*, the RST R scale, *einwandfrei / unverständlich*,
*Empfangspegelanzeige*, *über Stufe 9*, *Flugfunk / Seefunk*, *Flug- und
Seefunkstellen*, *zugelassenes CB-Funk-Gerät*, *Verschleierungsverfahren*,
*digitale Kodierungen*, *Taxi-Funk / Absprachen in einem Unternehmen*,
*Zusatz "/T"*.

## Added to `DECISIONS.md` (new section "Course text")

- Numbered references: *Abbildung / Bild* → "Figure", *Tabelle* → "Table",
  capitalised.
- Pronunciation column of the phonetic alphabet: the ITU's English
  respelling (RR Appendix 14), not a respelling of the German column.
- `<qso>` and quoted calls in English voice procedure as in BE102, BE103,
  BE105; German phrases quoted as German usage stay; German glosses of
  English words are dropped.

## Judgement calls

- buchstabiertafel (section and slides): pronunciation column replaced by the ITU English respelling (KEH-BECK, not a transliteration of KWE-BECK); the `&#8209;` non-breaking hyphens of the November row kept.
- buchstabiertafel: first example keeps *Delta Mike Vier …* (spoken German digit on a national contact, explained two paragraphs later), rather than "Four".
- betriebsabwicklung: *Ist diese Frequenz frei?* → "Is this frequency in use?", prose "ask … whether the frequency is in use", to match BE105.
- betriebsabwicklung: *von* in a directed call and the slides' *für* both → "this is"; *bitte kommen* → "over"; *und hört* → "listening"; *krschkrsch* → "crackle-crackle".
- betriebsabwicklung: CQ respelling *si-kju* → "see-kyoo"; the second respelling *(etwa "sik-ju")* and the gloss *also "suche dich"* dropped (they only re-explain English to a German reader); "Allgemeiner Anruf" kept in German with "(general call)".
- betriebsabwicklung (indepth): QSO meaning written in the ITU Q code wording, "I can communicate with station X direct", instead of the literal "I have direct contact with station X".
- erste_schritte: *push to talk, also "drücken, um zu senden"* → "push to talk" (German gloss dropped); wordorigin rewritten as "formed from the two English words *transmitter* and *receiver*".
- erste_schritte: *Dreisatz* → "rule of three" (UK schools say "unitary method"; "rule of three" is the general term).
- rst: table n_rst keeps the "English" column; "Meaning" is given in lower case (readability, signal strength, tone quality), so the two columns partly repeat each other in English.
- rst: *Rapport* → "signal report" (index "Signal report"); *über Stufe 9* → "above S9"; *Telefonie (Sprechfunk)* → "telephony (voice communication)".
- Index terms translated, two-level where natural (`Call:General`, `RST system:Readability`); *Sprache:Offene* → one-level `Plain language`.
- ausbildungsfunk: *Klasse E oder A* → "Class E or Class A"; German „…“ quotes in the slides → plain double quotes, as in the sections.

## Suspected errors in the German original

- sections/buchstabiertafel.md — "Delta Mike *Vier* Echo Alpha X-ray" — *Alpha* is not the ITU spelling (*Alfa*, as in the table and the next sentence); also *X-Ray* / *X-ray* written both ways. Kept as written.
- slides/betriebsabwicklung.md — directed-call and unclear-call examples have "DL9MJ für DL1PZ" / "D…MJ für DK5WP" where the section has "von"; *für* reads as the reverse direction. Both rendered "this is".
- slides/rst.md vs sections/rst.md — the slides say the T value is used in Morse telegraphy *and digital transmissions*, the section says *only* in Morse telegraphy.
- slides/rst.md — "Subjektive Bewertung des Lesbarkeit": *des* should be *der* (typo, no effect on the English).
- slides/erste_schritte.md — speaker note "noch ein Bulletpoint" is a leftover placeholder (translated as "another bullet point").
- slides/erste_schritte.md vs sections/erste_schritte.md — slide "Der Lehrgang … kann aber nicht alles notwendige Wissen vermitteln" against section "dieser Kurs vermittelt alles nötige Wissen" (the slide probably means mathematics only).

## Provjera

18 files compared paragraph by paragraph with `ccb71af~1` (German); all
embedded questions (BA101–BA110, BB102, BD209, BE101–BE108, BE201–BE209,
NA101–NA103, NF103, NF108, NF301, VC111–VC115, VD102, VD103, VD205–VD207,
VD303, VD306, VD703) looked up in English. 5 changes in 3 files: 0 omission,
0 meaning, 0 technical, 5 style, 0 glossary. `revizija-guard.py --rev
ccb71af~1 --brojevi`: 18 files, *struktura netaknuta*.

- betriebsabwicklung (section and slides), `<qso>`: "this is DL1PZ with a general call" → "making a general call" (idiomatic; keeps the link to *general call*, BB102).
- betriebsabwicklung (section), indepth: *Daran angelehnt* "Following on from this" → "By extension".
- rst (section): *Unter der Lesbarkeit wird die Verständlichkeit verstanden* → "Readability is taken to mean intelligibility." (the translator's version added an explanation the German does not have).
- rst (section): *Besonderheit* "peculiarity" → "feature".

Judgement calls confirmed:

- Pronunciation column: the German column teaches German readers how to say the English code words ("Korrekte Aussprache vermitteln"); the ITU's own respelling (checked against RR Appendix 14, all 26 rows) teaches the same to an English reader. Kept, with the DECISIONS.md entry. The one audible difference, Quebec (German KWE-BECK, ITU KEH-BECK), follows the ITU.
- *Delta Mike Vier …* kept: in a national contact the digit is spoken in German, which is what the section teaches two paragraphs later.
- "Is this frequency in use?": matches BE105 a (*besetzt* → "in use") and the usual English phrase; no answer means a free frequency either way, so the procedure is unchanged.
- *von* / slides' *für* → "this is": standard English voice procedure, matches BE102/BE103.
- *Dreisatz* → "rule of three": the established English name, understood by a British reader; NA101–NA103 show what is meant.
- Dropped glosses (*suche dich*, *drücken, um zu senden*, the second CQ respelling, German words in brackets in the wordorigin and slide note): they translate English back into German; nothing a reader of the English needs is lost.
- QSO meaning in ITU wording ("I can communicate with station X direct"): follows the Q code decision.
- The three new DECISIONS.md entries and the §14 glossary rows: kept as written.
