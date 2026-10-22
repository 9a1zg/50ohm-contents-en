# nea_antennen_uebertragungsleitungen_1 — translation report

Chapter "Antennen und Übertragungsleitungen (1/4)" (Antennas and
transmission lines, part 1): 13 sections, each with its slides, and 8
solutions. 34 files:

- `contents/sections/` and `contents/slides/`: `antennen.md`, `dipol.md`,
  `yagi_uda_1.md`, `rundstrahler.md`, `endgespeiste_antennen.md`,
  `polarisation.md`, `polarisation_2.md`, `polarisation_3.md`,
  `antennenformen_2.md`, `antennenformen_3.md`, `antenne_laenge_resonanz.md`,
  `verkuerzungsfaktor_1.md`, `verkuerzungsfaktor_2.md`.
- `contents/solutions/`: `AG101.md`–`AG105.md`, `AG118.md`, `AG315.md`,
  `AG316.md`.

`revizija-guard.py --brojevi`: 34 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (the `%` comments and
the commented-out picture in antennen, *Mantelwellensperre*, *Verkürzungsfaktor*,
*Polyäthylen*, the symbol $ü$). Line counts, trailing spaces (endgespeiste_antennen,
polarisation_2, antennenformen_2, verkuerzungsfaktor_1, slides polarisation_3 and
verkuerzungsfaktor_2), the double spaces in endgespeiste_antennen, polarisation and
polarisation_2, the blank lines at the end of yagi_uda_1 and the missing final
newlines are as in the German.

Embedded questions looked up in English and the prose aligned with them:
NG101–NG111, NG304, NG305, NB304, EB305–EB310, EG101–EG110, EG201, EG202,
EG213–EG217, EG219, EG222, AG101–AG105, AG117–AG124, AG201, AG202, AG223,
AG313, AG315, AG316, AG419 (NG104 "a λ/4 vertical antenna fed against earth";
NG106 "radials"; NG110/NG111 "omnidirectional antenna", "magnetic-mount
antenna", "on the roof of the house"; NG304/NG305 "shorten / lengthen both
ends equally"; EG213 "balanced antenna", "centre-fed"; EG219 "a low angle of
radiation"; EG222 "is stated according to the orientation of the electric
field component"; EG201 "the ratio of the velocity of propagation along a
line to the velocity of propagation in a vacuum"; EG202 "shortening factor
(correction factor)"; AG101–AG105 "shortening factor", AG104 "radiating
element"; AG118 "full-wave delta loop", "correction factor"; AG120 "Zepp
antenna"; AG123 "MWS = common-mode choke"; AG124 "end-fed resonant multiband
antenna"; AG313–AG316 "velocity factor", "open-wire line", "solid
polyethylene"; EG107 "sleeve dipole", "crossed Yagi-Uda", "parabolic dish").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

21 rows: *Up- and Outer-Antenne*; *Dipolschenkel / Schenkel / Teilstück*;
*gegen Erde erregt*; *Ortsverbindungen*; *End-Fed / EFHW*;
*Stummel-Stabantenne*; *Poynting-Vektor*; *magnetische Ringantennen
(Magnetic-Loops) / Magnetantennen / Magloop*; *elektrische Schleifenantenne*;
*Keule / hertzscher Dipol / Richtwirkung*; *Sperrtopf / Kreuz-Yagi-Uda*;
*Zeppelinantenne (Kurstext)*; *Mantelwellensperre (Abkürzung MWS)*; *Un-Un /
Pigtail / Symbolbild*; *Erde als Gegenpol / Erdpotential*; *Verkürzungsfaktor
(Kurstext)*; *Vakuumlichtgeschwindigkeit / Überlichtgeschwindigkeit /
Phasen- / Gruppengeschwindigkeit*; *Polyäthylen (Formelsammlung)*;
*Anpassgerät bzw. Tuner*; *plattgedrückte Ganzwellenschleife*; *Anpassung
(Folienüberschrift)*.

Changed: the §14 row *Fuchskreis* (Fuchs matching circuit) got a note —
*Fuchs circuit* after the first mention in a file, *Fuchsantenne* → Fuchs
antenna. The English term itself is unchanged.

## Added to `DECISIONS.md`

1 entry (Course text): *Verkürzungsfaktor* — *shortening factor* for
antennas, *velocity factor* for lines and cables; named once with both
terms and the German word where verkuerzungsfaktor_1 introduces it for lines
including antenna wires.

## Judgement calls

- verkuerzungsfaktor_1: "the *velocity factor* $k_\mathrm{v}$ (for antennas usually called the *shortening factor*; German has one word for both, *Verkürzungsfaktor*)" — the German defines one quantity that EG201 calls *velocity factor* and EG202 *shortening factor*; without both names the two embedded questions would seem to be about different things (DECISIONS.md). The section's long sentence is split in two ("… cannot be used. Instead, a correction factor is needed: …").
- verkuerzungsfaktor_2 and solutions: antenna sense → "shortening factor" (also the dipol slide note "The shortening factor only comes in Class E" and antennenformen_3 "Unlike the shortening factor of dipoles"); open-wire line and coaxial cable → "velocity factor" (section, slide headings, AG315, AG316); *Verlängerungsfaktor* → "lengthening factor" (glossary).
- verkuerzungsfaktor_2: *Polyäthylen* (the formula sheet's spelling, which the `%` TODO contrasts with the questions' *Polyethylen*) → "polyethylene (*Polyäthylen*)", as a formula-sheet keyword (DECISIONS.md); the slide only "polyethylene".
- verkuerzungsfaktor_2: *elektrische Schleifenantennen* → "electric loop antennas" (the full-wave loop as against the magnetic loop), kept rather than interpreted as "full-wave loops".
- rundstrahler: *"Up- and Outer"-Antenne* → '"up-and-outer" antenna', in quotation marks at first mention as in the German, lower case afterwards and in captions; *Erdboden* → "the ground", *Erde* → "earth" (glossary); *Erdnagel* → "earth spike"; *Rundstrahler* → "omnidirectional antennas" (NG110, NG111); *Relaisfunkstellen* → "repeaters"; *rundherum frei* → "clear all round"; *im Kapitel Einbau Kfz* → "in the chapter on installation in vehicles" (chapter titles not yet translated).
- rundstrahler slides: *Im UKW-Bereich … für Ortsverbindungen und Relaisfunk* → "On VHF, … for local contacts and repeater operation".
- dipol: *in Resonanz* → "at *resonance*"; *Teilstück* → "section"; *asymmetrisch gespeister Dipol* → "off-centre-fed dipole" (glossary §9 *Windom*), as *asymmetrisch angeregte Windomantenne* → "off-centre-fed Windom antenna" in antennenformen_3; *Töne* → "notes".
- dipol slides: heading *Anpassung* → "Adjustment", not "Matching": the slide is about bringing the dipole to the wanted frequency by changing its length, and *matching* (glossary) is impedance matching, which the chapter treats separately.
- yagi_uda_1 slide caption: *mit Einspeisung am Dipol am vorletzten Element* → "fed at the dipole, the second-to-last element"; *Taschenlampe* → "torch".
- endgespeiste_antennen: *oder auch kurz End-Fed* → "or an *end-fed* for short"; *Anpassglied* → "matching network", *Speisewiderstand* → "feed-point impedance" (glossary).
- antennenformen_2: *(englisch: end fed half wave, EFHW)* → "end-fed half-wave dipoles (EFHW)" — the English gloss is the term itself (bracket rule), the abbreviation stays because the text uses it; *magnetischen Ringantennen (Magnetic-Loops)* → "*magnetic loop antennas*", bracket dropped likewise; *Symmetrierglied (Balun)* → "what is known as a balun".
- antennenformen_2: *symmetrische Antenne / Kabel* → "balanced", *unsymmetrisch / asymmetrisch* → "unbalanced" (glossary, EG213); *Symmetrie* (slide heading) → "Balance"; *Pole* of a dipole → "poles" (keeps the link to the wordorigin "two poles").
- antennenformen_2: *Fuchskreis* → "Fuchs matching circuit" at first mention, "Fuchs circuit" afterwards; *Dr. Josef Fuchs* → "Dr Josef Fuchs" (British style); *Amateurfunkrufzeichen* → "amateur call signs".
- antennenformen_2: *flache Abstrahlung* → "a low angle of radiation" (EG219, glossary: never "flat"); *Keule* → "lobe"; *hertzscher Dipol* → "Hertzian dipole"; *bei idealer Erde* (caption) → "over perfect earth"; *2,5-mal* → "2.5 times".
- antennenformen_2: *Sperrtopfantenne … aus einem λ/4-langen Topf* → "sleeve dipole … of a λ/4 long sleeve"; *sowohl ein Sperrtopf als auch eine Kreuz-Yagi-Uda … ebenso wie Parabolspiegel* → "a sleeve dipole and a crossed Yagi-Uda, just like a parabolic dish" (EG107).
- antennenformen_2 slides: *Richtwirkung* → "Directional properties"; *Weniger Störungen bei … Gegenständen im Nahfeld* → "Less affected by … objects in the near field" (the section's *stören sich weniger an*); note *für den Ausschluss geeignet* → "useful for eliminating answers".
- antennenformen_3: *Zeppelinantenne* → "Zepp antenna" (AG120, glossary), at the paragraph that introduces it "*Zepp antenna*, short for Zeppelin antenna", so that the next paragraph's airship explanation makes sense in English.
- antennenformen_3: *Mantelwellensperre (Abkürzung MWS)* → "A common-mode choke (in German *Mantelwellensperre*, abbreviated MWS)" — MWS is a German abbreviation that the drawings and AG123/AG124 use.
- antennenformen_3: *Übersetzungsverhältnis* $ü$ → "transformation ratio", *Windungsverhältnis* → "turns ratio" (glossary §4); *Es besteht also die Möglichkeit der Verwechselung* → "so the two can be confused" (joined to the sentence before); *1 zu 49 Un-Un* → "1 to 49 unun"; *Symbolbild* → "illustrative photo".
- antennenformen_3: *Schenkel* of a delta loop → "sides"; *Tages-, Jahres- und Sonnenzykluszeiten* → "times of day, seasons and phases of the solar cycle"; *Zweidrahtleitung* → "twin feeder" (glossary); *Erde als Gegenpol* → "earth as the other pole"; *Antennen für den KFZ-Bereich* → "vehicle antennas"; *Abstrahlcharakteristik* → "radiation pattern".
- antenne_laenge_resonanz: *Anpassgerät bzw. Tuner* → "an antenna tuning unit or tuner"; *plattgedrückte Ganzwellenschleife* → "flattened full-wave loop".
- polarisation: *linkszirkular / rechtszirkular* → "left-hand / right-hand circular(ly)" (NB304); slide note *mit Stummel-Stabantenne in vertikal schlechter Empfang; Grund war die Weiterverwendung der vorhandenen Yagi-Uda-Antennen* → "with a stubby rod antenna, vertical gives poor reception; the reason was that the existing Yagi-Uda antennas could go on being used".
- polarisation_2: *Sie entsprechen der elektrischen Feldkomponente* → "They are in line with the electric field component"; *Merkregel* → "rule"; *senkrecht auf / aufeinander* → "at right angles to (each other)" (glossary); slides *Breitet sich das E-Feld horizontal / vertikal / zirkular aus* → "If the E field extends horizontally / vertically / circularly", kept parallel and as vague as the German (see below); *Magloop* → "mag loop".
- polarisation_3: *Satelliten- bzw. Weltraumkommunikation* → "satellite and space communication" (glossary §13).
- Solutions and solution slides: *Gesucht ist* → "We are looking for", *Lösungsweg* → "Solution", *gegeben / gesucht* → "given / required", as earlier units; the symbols $l_E$, $l_G$, $k_v$, $v_\mathrm{k}$, $\lambda_\mathrm{Leitung}$ unchanged.

## Suspected errors in the German original

- sections/antennenformen_3.md — `[ref:a_zeppelinantenn]` names an ident that does not exist (the picture is `a_zeppelinantenne`), so the reference is broken; also "Abbildung[ref" without a space. Markup kept; the English has a space before the ref.
- sections/polarisation_2.md — the three margin pictures 886, 936 and 935 all carry the ident `e_funkhorizont` ("radio horizon"), which is duplicated and unrelated to polarisation (copied from another figure?). Kept.
- slides/antenne_laenge_resonanz.md — "Jedoch ist dann deren Wellenwiderstand anders … Dieser Wellenwiderstand muss an die Speiseleitung angepasst werden": an antenna has a feed-point impedance (*Fußpunktimpedanz*), not a characteristic impedance (*Wellenwiderstand*), which is a property of a line. Translated as written ("characteristic impedance").
- sections/antenne_laenge_resonanz.md — the worked result is written "$\lambda = … \cdot \frac{5}{8} = 6,58$ m": the result is the length $l = \frac{5}{8}\lambda$, not $\lambda$ (the slides write $l$). Kept.
- slides/verkuerzungsfaktor_2.md (AG118) — $l_E \approx 42,23$ m, while the solution AG118 and the other slides have 42,25 m ($300/7,1 = 42,25$); and $1,02 \cdot 42,23 = 43,07$, not 43,10 — the result follows from 42,25. Kept.
- sections/verkuerzungsfaktor_2.md, slides — the factor is written $v_\mathrm{k}$ in the coaxial formula but $k_\mathrm{v}$ / $k_v$ everywhere else in the chapter. Kept.
- slides/polarisation_2.md — "Breitet sich das E-Feld horizontal aus, wird von horizontaler Polarisation gesprochen" (and vertical, circular): what counts is the *orientation* of the E-field vector, as the section and EG222 say, not the direction in which the field spreads. Translated as written ("extends").
- sections/antennenformen_3.md — the attention box on the 5/4 λ optimum for centre-fed dipoles carries the German's own `% TODO: Frage ist falsch` about AG223. Kept as it is.
- Typos with no effect on the English: sections/rundstrahler.md "von Gesamtgebilde" (*vom*), "wird abgestrahlte Welle" (*die abgestrahlte*), "auf einem hohem Mast" (*hohen*); sections/endgespeiste_antennen.md "machmal" (*manchmal*); slides/endgespeiste_antennen.md "Anpassglieder ist Teil" (*sind*); sections/polarisation_2.md "zirkuar" (*zirkular*), "die in derselben Ebene befinden" (*sich … befinden*); sections/antennenformen_2.md "aben" (*haben*), "verscheidenen" (*verschiedenen*), "Nicht zu Verwechseln" (*verwechseln*); sections/antennenformen_3.md "mindests" (*mindestens*), "notig" (*nötig*); sections/antenne_laenge_resonanz.md and sections/verkuerzungsfaktor_2.md "in dem man" (*indem*); slides/antenne_laenge_resonanz.md "Die Drähte einer Antennen" (*Antenne*); slides/antennenformen_2.md "bei dem starken magnetische Feld" (*magnetischen*).
