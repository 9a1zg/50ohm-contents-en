# slike_10 — translation report

103 files, all in `contents/photos/` (3, 4, 58–99, 245–351 as listed in
`serije.json`).

## Files translated (84)

- With a description (75): 3, 4, 58–76, 79–84, 86, 88–92, 95, 99, 245–248,
  257, 259–262, 264–271, 277, 286–288, 291–296, 298–303, 306–308, 316,
  318–320. 40 carry DARC's marker, translated; the 35 without it (3, 4,
  58–76, 79–84, 86, 88–92, 95, 99) are the older descriptions with
  `1) Kurzbeschreibung` / `2) Ausführliche Beschreibung`.
- Marker only (9): 322–329 (marker and an empty line, kept so) and 330
  (marker, no newline); only the marker is translated.

## Files left as they are (19)

- `TODO` only: 332–347, 349, 350, 351 (no newline, as in German).

`alttext-check.py`: 103 files, 3 with findings, all checker artefacts:
259 ("ist"), 319 ("einen für ist und"), 79 ("das der"). In each the German
words are inside a quoted German label in brackets; the checker's
quote/bracket regex loses track because the quoted text itself contains
brackets ("(sprich: tangens delta)", "(BEMFV)", the footnote "1) …"). No
numbers missing. Line counts match the German. No file ends in a newline
except 322–329, which do in German too. The trailing space after the short
description of 59 and the double space after "Kurzbeschreibung:" in 99 are
dropped.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

10 rows: the texts overlaid on the oscilloscope photos (247, 257, 266–268);
the analyser screenshots' title and fields (248, 265); the tan δ slides
(259–261); the labels DARC set into photos 264, 299, 307; the ring-core
labels of 270, 271; the column headings of the Order 33/2007 table (319);
German printed on real objects (59, 61, 88, 89, 293, 298); coaxial-connector
parts (69, 72); a row of photo vocabulary (*DARC-Raute, OV-Stempel,
Massebolzen, Kühlblech, Tochterplatine, Lochrasterboard, Querträger,
Gleichstrom-Stromverteiler, Bundesadler* …).

## Judgement calls

- Section labels as §14: *Kurzbeschreibung* → "Short description",
  *Ausführliche / Detaillierte Beschreibung, Detailbeschreibung* → "Detailed
  description", *Kurzfassung* → "Brief summary", *Kurze Zusammenfassung,
  Kurzzusammenfassung, Kurz-Zusammenfassung* → "Short summary",
  *Zusammenfassung* → "Summary", *Details* → "Details". Numbering `1)`,
  `1.` or none kept as in each file, including the label on its own line
  (261, 262, 265, 267, 319).
- Text DARC overlaid on photos or slides (247, 257, 259–261, 264, 266–268,
  270, 271, 299, 307, 319) is treated like a drawing label: English, German
  in brackets, as photos 145 and 178 in slike_09. Value- or symbol-only
  labels ("A_L = 4.7 µH", "AL = 1180 nH", "tan δ = R / Xc", "R = 100 Ω",
  "X_C = 159 Ω", the frequency ranges and limits of 319) take a decimal point
  and no bracket. "Styroflex" (trade name) and "(Equivalent Series
  Resistance)" (printed in English) keep none. 295's "defekt" under the burnt
  fuse is treated the same way: "defective" ("defekt").
- 248, 265 (analyser screenshots): the title and "Phi / Grad" get English
  with the German in brackets; "|Z| / Ohm" reads the same and keeps none;
  the marker fields *Reell / Blind* → real / reactive. Quoted display
  readings keep the screen's commas ("900,000k", "5,000M", "12,22 V");
  unquoted readings take a decimal point ("1.0010 MHz", "fStart 500.000 k",
  "12.20 V"), as slike_09. 265's "10.000" (thousands) → "10,000".
- German printed on real objects stays as printed with the meaning in
  brackets, as slike_09: "EIN/AUS" (on/off) and "EMK max. 6 V" (EMF max.
  6 V) (293), "Ein" (on) / "Aus" (off) and "Kl. 2.0" (class 2.0) (298),
  "Sonder DOK: DVL" (special DOK: DVL) and the handwritten greeting (61),
  "Silber" (silver) on the award certificates (59; "Gold", "Bronze" read the
  same), the fuse packaging "Träge" / "Flink" / "Mittelträge" (time-lag /
  fast-acting / medium time-lag, §12) (88), the battery warnings (89). Type
  and maker markings ("Ueff 0,6V 6V", "0,1A 0,5A 2,5A", "CK 330 35V",
  "Pontavi Wheatstone", "Made in W.-Germany") unchanged.
- 79, 80: the BNetzA document headings → the §14 English titles, the German
  in brackets; 79 spells out the BEMFV's full English name, as the German
  does.
- 99: the German writes "(AfuV)"; the English uses the glossary form
  "Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)", and "Anlage 1" →
  "Annex 1 to the AFuV" (§1.2).
- 267, 268: "um 90 Grad" in the overlaid text → "by 90°" (unit symbol after
  a number); 266's caption as the §14 rhyme row ("current too late").
- 286: the switch scale "0,1 – 1 – 10 – 100 – 1000" is unquoted → "0.1 – 1
  – 10 – 100 – 1000".
- Connectors as §14 *Stecker / Kupplung / Einbaubuchse*: *N-Einbaustecker*
  → N panel plug (68), *PL-Einbaubuchse* → PL panel socket (70), *Kupplung*
  → socket (71), *N-Einbaubuchse* → N panel socket (73); *Reduzierhülse* →
  reducer sleeve (69).
- *Trimmpotentiometer* → preset (trimmer) (299, 308), §4; *Trimmelement* →
  trimmer (318); *Spule* → inductor, *Ringdrossel* → toroidal choke,
  *Speicherdrossel* → storage choke; *Masse-Schraube / Massebolzen* →
  chassis screw / chassis stud (81, 303); *Schutzkontakt* → earthing
  contact, *Schutzkontakt-Steckdose* → Schuko socket with earthing contacts
  (86), §12; *Dachständer* → roof-mounted support for an overhead mains line
  (82), §14; *Zulassungsbescheid* → notice of authorisation (91), §14;
  *Diplom / Diplomurkunde* → award / award certificate (59, 60), §2;
  *Sonderrufzeichen* → special event call sign (59).
- 83: both *für VHF* and *für UKW* become "for VHF".
- 84: *Amateurtext* → "amateur radio text".
- Slip translated as meant: 287 "eine graue, kuppelförmige Innenteile"
  (wrong article/number) → "a grey, dome-shaped inner part".
- All files were written in place in the repository; no drafts outside it.

## Suspected errors in the German descriptions

- 84 — the short description says the picture was sent "an F6BIB", but the
  detailed description, the picture's text and the course caption
  (`digimode_ssb.md`) all have F1BIB. Translated as written ("to F6BIB").
- 270 — not an error of the description: the picture itself prints
  "A_L = 4,7 µH", which as an A_L value would be nH (per turn²) or µH per
  100 turns (47); the description quotes it correctly and the English keeps
  it as printed.
