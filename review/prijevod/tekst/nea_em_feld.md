# nea_em_feld — translation report

Chapter "Elektromagnetisches Feld" (Electromagnetic field): 3 sections, each
with its slides, no solutions. 6 files:

- `contents/sections/` and `contents/slides/`: `e_feld.md`, `h_feld.md`,
  `em_feld.md`.

`revizija-guard.py --brojevi`: 6 files checked, *struktura netaknuta*.
German-word grep: no hits (the idents `e_kondensator_homogenes_feld`,
`e_vertikalantenne_magnetfeld` … stay German, as idents do).

Embedded questions looked up in English and the prose aligned with them:
EB101–EB105, EA103, EA104, EB201–EB203, EB206, EB301–EB304.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

11 rows: *in den Äther lauschen* (listen in to the ether), *zeitlich
veränderlich / konstant* (varies with time / constant with time, EB301),
*senkrecht aufeinander stehen* (at right angles to each other, EB304),
*Durchschlagsfeldstärke / Grenzfeldstärke*, *stromdurchflossener Leiter*,
*(Feldlinien) in sich geschlossen*, *mittlerer Durchmesser / Umfang /
Länge* (EB203), *Wicklungsanzahl*, *gleichgerichtetes Feld*,
*Naturforscher*, *Vektor*.

## Added to `DECISIONS.md`

Nothing: every choice here is a single term (glossary) or follows an
existing rule (*Figure* before a reference, units after a number, decimal
point, *earth*).

## Judgement calls

- e_feld margin: *Äther* → "aether" (glossary §14, the physics concept); the idiom *lauschen in den Äther* → "*listen in to the ether*", the spelling English uses for the radio idiom, joined by "the term has survived in everyday language as "the ether"" so the reader sees it is the same word.
- e_feld, h_feld: *homogen* → "uniform" throughout (glossary §3, EB101, EB202); *Plattenkondensator* → "parallel-plate capacitor", *Wickelkondensator* → "wound capacitor", *Zylinderspule* → "solenoid" (EB202), *Ringkernspule* → "toroidal inductor", slide heading *Ringkern* → "Toroidal core" (EB203).
- e_feld: *Durchschlagsfeldstärke* → "breakdown field strength", *Durchbruchspannung* → "breakdown voltage"; the slides' *Durchschlagsfestigkeit* → "dielectric strength", as EB104.
- e_feld: *Antennenanpassgeräte* → "antenna tuning units" (glossary §9); slides *vom "positiven Ende" zur Erde* → "to earth" (house style).
- e_feld slides note: *homogen Feld: gleichgerichtetes Feld* → "Uniform field: a field pointing in one direction" — not "rectified", the other sense of *gleichgerichtet*; solution slide *Gegeben / Gesucht / Lösung* → "Given / Required / Solution", heading "### Solution", as in earlier units.
- h_feld: *Oerstedt* → "Ørsted", the physicist's name as English (and Danish) writes it (see errors below); *Naturforscher* → "natural philosopher", the period term.
- h_feld: *Die so genannte magnetische Feldstärke* → "The *magnetic field strength*, as it is called"; *lineare Form der Feldlinien* → "the field lines inside are straight"; *in sich geschlossen* → "closed loops".
- h_feld slides: the placeholder *Grafik … kommt noch* → "Graphic … to follow"; the elliptic note *H-Feld von magnetische Feldstärke H ein paar Folien weiter* → "H-field from magnetic field strength H, a few slides further on", keeping its terseness.
- em_feld: *Primärwindung / Sekundärwindung* → "primary winding / secondary winding" (glossary §14: *usually primary / secondary winding*); *zeitlich veränderlich* → "that varies with time" / "time-varying", as EB301; *senkrecht aufeinander* → "at right angles to each other", as EB304; *uninteressant* → "of no interest".
- em_feld: the German's empty reference "in den Abbildungen  und [ref:e_emfeld_ausbreitung]" kept as "in Figures  and [ref:e_emfeld_ausbreitung]", gap included (see errors); no reference added.
- em_feld slides: *in einem 90°-Winkel zueinander* → "at an angle of $\qty{90}{\degree}$ to each other".

## Suspected errors in the German original

- sections/em_feld.md — "Wie in den Abbildungen  und [ref:e_emfeld_ausbreitung] gezeigt": the first reference is missing (two spaces before *und*); probably `[ref:e_vertikalantenne_em]`. Kept as a gap in English.
- slides/em_feld.md — the picture 885 ("Elektrisches und magnetisches Feld an einer Antenne") carries the ident `e_vertikalantenne_magnetfeld`, which in h_feld (section 883, slides 192) is the magnetic field alone; the section uses 885 with `e_vertikalantenne_em`. Ident left unchanged.
- sections/h_feld.md — "Hans Christian Oerstedt": the name is Ørsted (German usually *Oersted*). Written "Ørsted" in English.
- sections/h_feld.md — EB203: with $l_m$ rounded to 0.082 m the result is 182.9 ≈ 183 A/m; the exam's correct answer, 183.6 A/m, comes from the unrounded 0.0817 m. Not wrong, but the text's figure does not match the answer.
- Typos with no effect on the English: sections/e_feld.md "ein isolierende Schicht" (*eine*), "*lauschen  in den Äther*" (double space), "(Achtung auf die Einheiten aufpassen!)" (two constructions merged); sections/h_feld.md "am Besten" (*am besten*); sections/em_feld.md "die sie zwischen 1861 und 1864 … erarbeitet" (*erarbeitete*), "was man im Amateurfunk" (comma missing before *was*); slides/h_feld.md "im inneren" (*Inneren*), "von magnetische Feldstärke" (*magnetischer*); slides/e_feld.md "homogen Feld" (*homogenes*).

## Provjera

Checked all 6 files paragraph by paragraph against `d98c73b~1` (German):
complete, numbers and formulas intact, embedded questions EB101–EB105,
EA103, EA104, EB201–EB203, EB206, EB301–EB304 consistent with the prose.
`revizija-guard.py --rev d98c73b~1 --brojevi`: *struktura netaknuta*.

Changes: omission 0, meaning 0, technical 1, style 3, glossary 2.

- technical — slides/h_feld.md: *magnetisch leitender Ringkern* "magnetically conductive toroidal core" → "toroidal core of magnetic material", the English way of saying it.
- style — sections/h_feld.md: "Inside a solenoid, unlike a straight conductor, the picture is different" → "the picture is different from that of a straight conductor" (no double contrast).
- style — sections/em_feld.md: *Dabei treten zusätzliche Effekte auf* "This brings additional effects" → "Additional effects then come into play".
- style — sections/em_feld.md: *legen … fest* "fix the direction of propagation" → "determine".
- glossary — row *Vektor* → *vector* removed: no choice in it, nothing for later units to follow (10 rows remain).
- glossary — row *Naturforscher* narrowed to the historical sense (natural philosopher before about 1850; a modern *Naturforscher* is a *scientist*).

Judgement calls kept: *Ørsted* for the German's *Oerstedt* (a name written as English writes it, slip listed for DARC); *aether* / *ether*; the empty figure reference in em_feld kept as a gap; no new DECISIONS.md entry needed. Suspected German errors confirmed as listed.
