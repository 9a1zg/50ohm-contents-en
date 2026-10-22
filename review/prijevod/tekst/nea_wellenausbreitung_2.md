# nea_wellenausbreitung_2 — translation report

Chapter "Wellenausbreitung (2/2)" (Propagation, part 2): 6 sections, each
with its slides, no solutions. 12 files:

- `contents/sections/` and `contents/slides/`: `bodenwelle.md`,
  `greyline.md`, `moegel_dellinger_effekt.md`, `langer_kurzer_weg_1.md`,
  `langer_kurzer_weg_2.md`, `scatter.md`.

`revizija-guard.py --brojevi`: 12 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (*Türöffnertag* and
*Die Sendung mit der Maus*, the `%TODO` comment in scatter).

Embedded questions looked up in English and the prose aligned with them:
EH211–EH217, AH216–AH218, AH223, AH310, AH311.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

17 rows: *Lang- und Mittelwelle* (ground wave), *Bodenbeschaffenheit /
leitfähiger Boden*, *Stadtbereich*, *Tag-/Nachtgrenze / Tag- und
Nacht-Gleiche*, *Greyline-DX / Twilight-DX*, *Skip-Distanz*,
*Strahlungsausbrüche / Plasma-Flares*, *Radio Blackouts*, *Sonneneruption der
Klasse X9.0 / aktive Sonnenfleckenregion*, *Türöffnertag der Sendung mit der
Maus / Maus-Stationen*, *Drehwinkel (Richtantenne)*, *Richtantennen (engl.
Beams)*, *Regenscatter (Rainscatter)*, *Flatterfading (flutter fading)*,
*Verbindungslinie zwischen Sender und Empfänger*, *Dämmerung*,
*Besserwisser*.

## Added to `DECISIONS.md`

Nothing; the unit follows the existing entries (bracket rule, *Region* /
*Schicht*, numbered *Figure*).

## Judgement calls

- bodenwelle: *in höheren Frequenzbereichen stärker gedämpft als in niedrigeren* → "attenuated more in higher frequency ranges than in lower frequency ranges", next to EH212 a ("at higher frequencies than at lower frequencies"); *geografischen Horizont* → "geographical horizon" as EH212.
- bodenwelle (slides): *Radio hat früher stark die Bodenwelle genutzt* → "Broadcasting used to rely heavily on the ground wave" (*Radio* is the broadcast medium); *"schlecht nutzbaren"* → "hardly usable"; *im Stadtbereich* → "within a city".
- greyline: *Greyline* → "grey line" (§10); slides *Greyline-DX oder Twilight-DX* → "*Grey-line DX* or *twilight DX*"; *Hohe Skip-Distanz* → "Long skip distance"; *flach gebrochen / reflektiert* → "refracted / reflected at a low angle" (as the earlier unit's *flach*).
- moegel_dellinger_effekt: *Im englischen Sprachraum spricht man meist vom Shortwave Fade-Out …* → "In English it is usually called a *short-wave fade-out* or a *sudden ionospheric disturbance* (*SID*)" — glossary spelling, without the glossary's "(SWF)", which the German does not give.
- moegel_dellinger_effekt: *Türöffnertag der Sendung mit der Maus* → "the Door Opener Day (*Türöffnertag*) of the children's television programme *Die Sendung mit der Maus*" — the programme's name stays German, three words added so an English reader knows what it is; *Maus-Stationen* → "the Maus stations".
- moegel_dellinger_effekt: *D-Schicht* in the 2024 paragraph → "D layer", *D-Region* elsewhere → "D region" (DECISIONS.md); *HF-Verbindungen* → "HF contacts" (the German HF here means short wave, as the sentence before says *Kurzwellen-Funksignalen*).
- moegel_dellinger_effekt: *Abbildung … zeigt das Zentrum der Sonneneruption auf der Erdoberfläche* → "shows where on the earth's surface the solar flare was centred" (the flare is on the sun; the map shows where its effect is centred); captions *am 03.10.2024 um 12 Uhr und 19 Minuten* → "on 03.10.2024 at 12:19" (numeric date kept, as earlier units), *Quelle NOAA* → "Source: NOAA"; the line break between the two figure sentences kept.
- langer_kurzer_weg_1: *Die Funkverbindung läuft also nicht über den direkten Weg …* → worded as EH216 a ("does not run via the direct path to the other station, but in the direction opposite to the shortest path"); the speaker note quotes the same English wording.
- langer_kurzer_weg_2: *Beam-Karten* → "great-circle maps (beam heading maps)" at first mention (glossary), "great-circle map" afterwards and in captions and slides; *Richtantennen (engl. Beams)* → "directional antennas (beams)", bracket kept because *beam* is a different English word and explains the map's name; *Rotorsteuerungen* → "rotator controllers".
- langer_kurzer_weg_2 (slides): *Drehwinkel* → "heading" / "beam heading" (AH217, AH218), *Drehwinkel der Hauptstrahlrichtung* → "heading of the direction of maximum radiation" (glossary *Hauptstrahlrichtung*), *über zwei Drehrichtungen* → "with two different headings"; the minus in "beam heading - 180°" kept as the German writes it.
- langer_kurzer_weg_2: *Der Funkamateur nutzt …* → "Radio amateurs use …" (no generic pronoun, DECISIONS.md).
- scatter: *Regenscatter (Rainscatter)* → "*rain scatter*", bracket dropped; slides: the bullet *Englisch Rainscatter* dropped (it only gives the English name of the heading, which is now English); *(Flatterfading, flutter fading)* → "(*flutter fading*)" — bracket rule.
- scatter: *Aircraft-Scatter* → "aircraft scatter" (§10, AH310); heading "Aircraft scatter"; *Spitzfindigkeit* → "A fine point"; *Besserwisser* (langer_kurzer_weg_2 note) → "know-alls".

## Suspected errors in the German original

- slides/moegel_dellinger_effekt.md — "Hohe Dämpfung der Raumwelle bis 300 MHz" — the section and EH214/EH215 speak of HF sky-wave propagation; 300 MHz looks like a slip (30 MHz?). Translated as written.
- slides/moegel_dellinger_effekt.md — "Sonneneruptionen mit Plasma-Flares ionisieren die D-Region" — the section (and EH214) attributes the D-region ionisation to the UV and X-ray radiation of the flare; the plasma (particles) arrives much later and is not what causes the fade-out.
- slides/scatter.md — Backscatter "Brechung der Raumwelle zurück zum Empfänger" — the section says the signal is *scattered* back *towards the transmitter* ("zurück Richtung Sender"). Translated as written ("Refraction … back to the receiver").
- sections/langer_kurzer_weg_1.md — "Die Funkverbindung läuft also nicht über den direkten Weg …" — introduced with *also* as if it followed from the two-paths paragraph, but it is EH216's definition of the *long* path, which the text names only in the next paragraph; read on its own it says every contact avoids the direct path. Translated faithfully ("therefore").
- sections/langer_kurzer_weg_2.md — "den langen Weg, der einmal vollständig um den Globus herumführt" — the long path runs the other way round the great circle (here about 24000 km), not once completely round the globe.
- sections/bodenwelle.md — "jeden Sender, denn man dort tagsüber hört" — *denn* should be *den*.
- Typos with no effect on the English: sections/bodenwelle.md "Lang und Mittelwelle" (*Lang- und*); sections/moegel_dellinger_effekt.md missing full stop after "überhaupt möglich ist", "in diese Fall" (*diesem*); slides/moegel_dellinger_effekt.md note "beschreiben" (*beschrieben*); slides/langer_kurzer_weg_1.md note "Anhand" (*anhand*); sections/langer_kurzer_weg_2.md "Die Richtung … unterscheiden sich in der Richtung" (number and repetition); sections/scatter.md "üblichweise" (*üblicherweise*), indepth "als "Scatter" bezeichnet" (missing *wird*).

## Provjera

Checked all 12 files against `2c62b05~1`, paragraph by paragraph, and the
embedded questions (EH211–EH217, AH216–AH218, AH223, AH310, AH311) in
English. Complete and faithful; the prose matches the questions' wording.
`revizija-guard.py --rev 2c62b05~1 --brojevi`: 12 files, *struktura
netaknuta*.

Changes: omission 0, meaning 0, technical 0, style 5, glossary 3.

- moegel_dellinger_effekt: "Basically a fine thing" → "In principle that is a good thing" (*Grundsätzlich eine feine Sache*).
- moegel_dellinger_effekt: "unlike usual" (not idiomatic) → "unusually".
- moegel_dellinger_effekt caption e_dellinger: "affected by an absorption of 1 dB" → "affected by 1 dB of absorption", as NOAA's D-RAP labels it.
- scatter: "The scattering goes in all directions" → "Scattering takes place in all directions".
- greyline: "the area of the boundary between day and night" → "the zone along the boundary …" (cf. EH213 "twilight zone").
- Glossary: *Besserwisser* row removed (a one-off colloquialism in a speaker note, not a term).
- Glossary: *Richtantennen (engl. Beams)* note said "explains *beam map*"; corrected to *beam heading map*, the bracket actually used for *Beam-Karte*.
- Glossary: *Strahlungsausbrüche / Plasma-Flares* note records why the slides' *Sonneneruptionen* are "solar eruptions" there, not the glossary's *solar flare* (it would sit beside "plasma flares").

Judgement calls kept: all of them, including the dropped slide bullet
*Englisch Rainscatter* (bracket rule for list items, DECISIONS.md), "(beams)"
kept beside *directional antennas*, and the interpretive "where on the
earth's surface the solar flare was centred". Suspected German errors
confirmed as listed; no DECISIONS.md entry needed.
