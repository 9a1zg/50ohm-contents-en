# nea_wellenausbreitung_1 — translation report

Chapter "Wellenausbreitung (1/2)" (Propagation, part 1): 21 sections, each
with its slides, no solutions. 42 files:

- `contents/sections/` and `contents/slides/`: `wellenausbreitung.md`,
  `funkhorizont.md`, `troposphaere.md`, `troposphaere_2.md`,
  `troposphaere_3.md`, `mehrwegeausbreitung.md`, `aurora_1.md`,
  `aurora_2.md`, `sporadic_e_1.md`, `sporadic_e_2.md`, `sporadic_e_3.md`,
  `ionosphaere.md`, `ionosphaere_2.md`, `ionosphaere_3.md`,
  `tote_zone_1.md`, `tote_zone_2.md`, `fading.md`, `sprungdistanz_1.md`,
  `sprungdistanz_2.md`, `muf_luf_1.md`, `muf_luf_2.md`.

`revizija-guard.py --brojevi`: 42 files checked, *struktura netaknuta*.
German-word grep: no hits outside the two `%` comments (`%TODO` in
mehrwegeausbreitung, `%Simulation mit:` in tote_zone_2).

Embedded questions looked up in English and the prose aligned with them:
NH101–NH102, NH201, NH301–NH306, BE106, EH101–EH107, EH201–EH210, EH218,
EH219, EH301–EH305, AH101–AH108, AH201–AH215, AH219–AH222, AH301–AH309.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

31 rows: *Überreichweiten* (course text), *Wetterschicht*,
*Inversionswetterlage / troposphärische Inversionsbildung /
Inversionsschicht*, *Überhorizontverbindungen*, the *Ducting* gloss,
*Beugung / Streuung / Reflexion / Brechung oder Refraktion*, *gleichgerichtete
Streuung*, *Hochatmosphäre / Atmosphärenschichten*, *Atomrümpfe*, *gemäßigte
Breiten*, *Schicht / Region*, *sporadische E-Schicht / Sporadic-E-Bedingungen*,
*Sonnenzyklus*, *Aktivitätsmaximum / -minimum*, *Polarlichter /
Polarlichterscheinung*, *flatternd / verbrummt*, *Doppler-Spread /
Signalrapport*, *Interferenz / Summensignal / Laufzeit*, *Multipath-Effekte /
Faraday-Rotation*, *Abstrahlwinkel / flach / steil abstrahlen*, *Sprung
(Hop)*, *Short Skip* gloss, *Fading (Schwund)*, *Ionosphärenmessstation /
Ionosonde*, *Formelzeichen*, *FOT*, *kommerzielle Frequenzplanung*,
*Rauschflur*, *Magnetstürme*, *Raumstation ISS*,
*Notfunk-Ausbildungswochenende*.

## Added to `DECISIONS.md` ("Course text")

- Ionosphere: *Region* → region and *Schicht* → layer, each as the German
  writes it, since the text itself names both ("Regionen … manchmal auch
  Schichten"); the earlier *region* entry concerns the questions.

## Judgement calls

- troposphaere, wellenausbreitung (section and slides): *Überreichweiten* → "enhanced propagation" (index "Enhanced propagation"), *erheblich größere Reichweiten* → "considerably greater ranges"; *Besondere Überreichweiten durch Sporadic-E* → "Particularly enhanced propagation due to sporadic E".
- troposphaere: *Inversionswetterlage* → "temperature inversion"; slides *Troposphärische Inversionsbildung* → "Formation of tropospheric inversions", the wording of NH304 a.
- troposphaere_2 (slides): *Brechung oder Refraktion* → "Refraction" (one English word); *Gleichgerichtete Streuung* → "scattering in one uniform direction".
- troposphaere_3: the gloss *vom englischen duct, was so viel wie Röhre, Kanal oder Führung bedeutet* kept as "(from *duct*, meaning roughly a pipe, channel or guide)" — it explains the word rather than translating it back.
- sporadic_e_2: *Short Skip Bedingungen (engl. short skip = "kurzer Sprung")* → "*short skip* conditions", gloss dropped; sprungdistanz_1: *Sprung (oder englisch Hop)* → "*hop*"; fading: *Fading (Schwund)* → "*fading*"; mehrwegeausbreitung (slides): *Schwund, Fading oder QSB* → "fading or QSB" (bracket rule, DECISIONS.md).
- Throughout: *Abstrahlwinkel* → "angle of radiation" (EH208, AH208, AH209); *flach / flacher* → "low / lower angle", never "flat"; *steil* → "steep".
- Throughout: *Region* / *Schicht* kept apart as the German has them (new DECISIONS.md entry); *Sporadic-E* → "sporadic E", capitalised only at the start of a sentence.
- Throughout: *Kurzwelle* → "HF", *Kurzwellen* (the waves) → "HF waves", *Lang- und Mittelwelle* → "long and medium wave"; *Kilometern* after a number → "km".
- muf_luf_1 (section and slides): *maximal usable frequency* written "maximum usable frequency"; *LUF (Lowest Usable Frequency), also die niedrigste nutzbare Frequenz* → "LUF (*lowest usable frequency*), the lowest frequency that can be used" (avoids saying the same words twice).
- muf_luf_2 (section and slides): *FOT (frequency of optimal transmission, optimale Sendefrequenz)* → "*FOT* (*frequency of optimum transmission*, optimum working frequency)", the usual English expansion plus the name AH206 uses; headings *Höchste / Niedrigste brauchbare Frequenz* → "Maximum / Lowest usable frequency".
- muf_luf_2: *kleiner tiefgestellter Buchstabe "O"* → small subscript letter "o"; symbols $f_\text{k}$, $f_\text{krit}$ unchanged.
- muf_luf_1: *zwischen 6 und 12 Uhr* → "between 6 a.m. and 12 noon"; muf_luf_2: date "08.09.2025" kept numeric (as the earlier unit did); *Raumstation ISS* → "International Space Station (ISS)"; *im Kapitel Ionosphäre II* → "in the chapter Ionosphere II" (the table-of-contents titles are not translated yet).
- ionosphaere_2: *Atomrümpfe* → "positive ions"; *Dieser Prozess verleiht insbesondere der Kurzwelle ihre einzigartigen Fähigkeiten* → "It is this process above all that gives HF its unique capabilities".
- ionosphaere_2 (slides): *Namensgebene: E(lektrische)-Schicht* → "Origin of the name: *E*(lectric) *layer*".
- aurora_1, aurora_2: *Polarlichter* → "aurorae", slides *Aurora- oder Polarlichterscheinung* → "Aurora (polar lights)"; *flatternd* / *verbrummt* → "fluttering" / "buzzing" (AH308, glossary §10); *Digimodes* → "data modes"; link text *Youtube* → "YouTube".
- mehrwegeausbreitung: the indepth etymology of *Interferenz* kept (Latin *inter*, *ferire*, Old French *s'entreferir*), which is also the English word's origin; German „…“ quotes → plain double quotes.
- ionosphaere: "(Abbildung [ref:…].)" → "(Figure [ref:…])." (full stop moved outside the bracket).
- Index terms: Radio horizon, Line of sight, Enhanced propagation, Troposphere, Sporadic E, Ionosphere, Sky wave, Ground wave, Solar cycle, Solar cycle:Sunspots, Skip zone.

## Suspected errors in the German original

- sections/muf_luf_1.md and slides/muf_luf_1.md — "MUF (*maximal usable frequency*)", heading "Maximal Usable Frequency (MUF)" — the English term is *maximum* usable frequency (muf_luf_2 and the questions have it right).
- slides/muf_luf_2.md — "*Frequency of optimal transmition*" — typo *transmission*; the usual expansion of FOT is *frequency of optimum transmission* / *optimum working frequency* (AH206).
- slides/ionosphaere.md — caption of picture 741 "Die Tote Zone, die für die Bodenwelle zu nah und für die Raumwelle zu weit weg ist" — reversed; the section and tote_zone_1 say *zu weit* for the ground wave and *zu nah* for the sky wave. Translated as written.
- sections/sporadic_e_2.md — "Da die Brechung bei Sporadic E in Bedingungen in der in niedrigerer Höhe befindlichen E-Region erfolgt" — garbled (probably *bei Sporadic-E-Bedingungen in der …*); translated as meant.
- slides/ionosphaere_2.md — note "Die Schichten darüber und darüber wurden …" — should be *darunter und darüber*; translated "below and above".
- slides/ionosphaere_2.md vs sections/ionosphaere_2.md — F regions "200–400 km" in the slides, "130 bis 450 km" in the section (and EH102, AH105, AH106); E region "verschwindet etwa 1 Stunde nach Sonnenuntergang" in the slides, "binnen weniger Minuten" in the section.
- slides/troposphaere_2.md vs sections/troposphaere.md — troposphere "Bis ca. 10 km" in the speaker note, "rund 15 km" in the section and slides of troposphaere.
- slides/aurora_2.md — "Wird also hauptsächlich mit UHF und VHF verwendet", while the sections name only VHF (6 m and 2 m bands).
- Typos with no effect on the English: sections/ionosphaere_2.md "ionosierten", "Sonneneintrahlung", "überbrückt werde"; slides/ionosphaere_2.md "Namensgebene"; sections/aurora_1.md and sections/aurora_2.md "verauschten"; slides/mehrwegeausbreitung.md "Ionossphäre"; sections/tote_zone_1.md "Genau genommene"; sections/ionosphaere_3.md and slides "Mögliche höhen"; slides/ionosphaere_3.md "In der Klasse A, es ist wichtig, …" (word order); slides/ionosphaere.md "über den elfjährige Sonnenzyklus"; sections/ionosphaere.md "(Abbildung [ref:…].)".
