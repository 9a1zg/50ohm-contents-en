# nea_elektrische_schwingungen_funkwellen — translation report

Chapter "Elektrische Schwingungen und Funkwellen" (Electrical oscillations
and radio waves): 17 sections, each with its slides, no solutions. 34 files:

- `contents/sections/` and `contents/slides/`: `gleich_und_wechselspannung.md`,
  `frequenz.md`, `sinusschwingung.md`, `amplitude_periode.md`,
  `zehnerpotenzen.md`, `funkwellen.md`, `wellenlaenge.md`,
  `formeln_umstellen.md`, `wellenlaenge_2.md`, `wasserfall.md`,
  `frequenzspektrum.md`, `frequenzzuteilung.md`, `amateurfunkbaender.md`,
  `primaerer_sekundaerer_funkdienst.md`, `iaru_bandplan.md`,
  `iaru_bandplan_2m.md`, `iaru_bandplan_70cm.md`.

`revizija-guard.py --brojevi`: 34 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (the German titles in
brackets after Telecommunications Act, Amateur Radio Ordinance and Federal
Network Agency, the `% TODO` comment).

## Added to `TRANSLATION_GLOSSARY.md` (§14)

*Windkraftwerk*, *Einheitenvorzeichen / Einheitenpräfix*, *Periode oder auch
Periodendauer*, *Ort* (snapshot axis label), *Hochzahl / Exponent*,
*technisch-wissenschaftlicher Taschenrechner*, *Exponentialschreibweise*,
*zugeschnittene Größengleichung*, *Grundeinheiten*, *umstellen /
herauskürzen*, *über das Band drehen*, *Amplitudenspektrum* (display),
*Langwelle / Mittelwelle* in the frequency-range table, *Verordnung über den
Amateurfunk (AFuV)*, *Nutzungsbestimmungen*, *Nutzungsrechte*, *Verfügungen
und Mitteilungen*, *Küstenfunk*, the ISM devices (*Garagentoröffner …
Reifendrucksensor*), *Interessenvertretung*, *geordnetes Nebeneinander der
Betriebsarten*, *Selbstregulierung*, *Funkpartner finden*,
*Telefonie-Direktverbindung*, band plan labels in brackets, *center of
activity*.

## Added to `DECISIONS.md` ("Course text")

- English names that the German glosses are not glossed back: in the
  frequency-range table the rows *(Kurzwelle) (KW)*, *(Ultrakurzwelle)
  (UKW)*, *(Dezimeterwelle)* are dropped (as BC101–BC106), LW/MW become the
  English everyday names; in the IARU band plan sections a bracketed band
  plan label is dropped where it is the English term itself, kept where it
  differs.

## Judgement calls

- frequenzspektrum (section and slides): three German-name rows of table n_frequenzspektrum_bereiche dropped (DECISIONS.md); "Short Wave | SW" kept capitalised as the German table has it, although BC104 writes "short wave (SW)".
- iaru_bandplan_2m (section and slides): *Baken ("beacons")*, *Weltraumkommunikation ("space communication")* etc. → "Beacons", "Space communication"; "FM voice ("FM calling")", "Digital telephony ("digital voice calling")", "Morse telegraphy ("CW")" keep the label.
- iaru_bandplan_2m: *Aktivitätszentrum … als* center of activity *markiert* → "centre of activity" in prose, "marked *center of activity* in the band plan" (label quoted as printed).
- iaru_bandplan_2m: *FM-Sprechfunk* → "FM voice" (glossary), while BC205/BC209 say "FM telephony"; *Digitale Telefonie* → "digital telephony" (BC207).
- iaru_bandplan_2m: *Um schnell einen Funkpartner zu finden* → "To find someone to talk to quickly" rather than the glossary's "the other station", which does not fit before a contact exists.
- amplitude_periode: *Periode oder auch Periodendauer* → "period … or periodic time" (both names kept, British *periodic time*).
- formeln_umstellen, wellenlaenge_2: *zugeschnittene Größengleichung* → "tailored quantity equation" (DIN 1313 term without a settled English name; the course defines it).
- wasserfall: *Amplitudenspektrum* → "amplitude spectrum" throughout (NI401), glossed once "(spectrum display)" to tie it to NF104's answer.
- funkwellen: snapshot axis label *Ort* → "position"; the drawing still says "Ort" until the drawings are translated.
- frequenzzuteilung: *Verordnung über den Amateurfunk (AFuV)* → "Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)", the glossary form VD101/VD702 use; BNetzA, which the German gives as an abbreviation only, written out at first mention as the brief asks.
- frequenzzuteilung (slides, note): "6,1W ERP" quoted as "6.1W ERP"; "auf 2m und 70cm" kept as "on 2m and 70cm" (a quotation from the speaker note, not running band names).
- primaerer_sekundaerer_funkdienst (slides, note): date "31.12.1998" kept in numeric form (the number check, and readable as is).
- zehnerpotenzen: *sechs Exemplare der Zahl 10* → "six copies of the number 10" (keeps the number); *Komma* → "decimal point"; calculator key sequence "3,5 → EXP → 6" in the slides → "3.5".
- gleich_und_wechselspannung (slides, note): *Außer, man bekommt "einen gewischt"* → "Unless you get a static shock."
- frequenz: *Amateurfunk-Einsteigerklasse N* → "the entry-level amateur radio Class N"; *Klasse E bzw. A* → "Class E and Class A".
- Index terms translated, two-level where the German has two levels (`Oscillation:Sine wave`, `Frequency assignment:Individual assignment`, `Voltage:AC voltage`).

## Suspected errors in the German original

- sections/wellenlaenge_2.md and slides/wellenlaenge_2.md — "Das 10 m-Band erstreckt sich von 28 bis 29,5 MHz" — the band is 28–29.7 MHz (VD717, frequenz, wellenlaenge table); the argument still works.
- sections/formeln_umstellen.md — indepth box "$c_o \approx …$" — letter o instead of the subscript zero used everywhere else ($c_0$).
- sections/wellenlaenge_2.md — "$\qty{1}{\giga\hertz} = 1000 {\mega\hertz}$" — the second value lacks `\qty`, so `\mega` stands bare in math mode (may not render).
- slides/frequenzspektrum.md — "Extemely High Frequency" — typo, written correctly in the English.
- slides/wasserfall.md — heading "Wassefalldiagramm" — typo.
- sections/iaru_bandplan_2m.md — "Dies Frequenzbereiche" — should be *Diese*.
- sections/wasserfall.md — "Anteile … am Gesamtsignals" — should be *Gesamtsignal*.
- slides/amateurfunkbaender.md — "Anlage 1 AfuV" — *AFuV*.
- sections/frequenzzuteilung.md and slides — "Verordnung über den Amateurfunk (AFuV)" — not the AFuV's formal title (*Verordnung zum Gesetz über den Amateurfunk*).
- slides/wellenlaenge.md vs sections/wellenlaenge.md — table n_funkwellen_baender gives the 70 cm wavelengths as 68–70 cm in the slides, 70–68 cm (descending, like the other rows) in the section.
- sections vs slides of frequenzspektrum (picture 847 / 471) and amateurfunkbaender (749, 750 / 829, 830) — the same ident with different picture ids; probably separate slide versions of the drawings, worth a check.
