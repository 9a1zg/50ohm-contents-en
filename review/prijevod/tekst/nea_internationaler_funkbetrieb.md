# nea_internationaler_funkbetrieb — translation report

Chapter "Internationaler Funkbetrieb" (International operating): 4 sections,
each with its slides, no solutions. 8 files:

- `contents/sections/` and `contents/slides/`:
  `internationale_landeskenner.md`, `itu_regionen.md`, `dx.md`,
  `funken_im_ausland.md`.

`revizija-guard.py --brojevi`: 8 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (the mnemonics
*Links Außen*, *Schwedische Möbel*, *Schönes Polen*, *Viele Kängurus* …,
*DARC-Auslandsreferat*, *ECC-Empfehlung*, the CEPT's French name).

Embedded questions looked up in English and the prose aligned with them:
BD212–BD214, BD301–BD318, VA401–VA405, BB103–BB105, BE104, BE109, BE110,
BE113, BE114, BE312, VB101–VB114.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

11 rows: *Fragenkatalog* (question catalogue), the mnemonics of the
country-prefix tables, the remaining country names (*Vereintes Königreich*,
*Vatikan*, *Norwegen* …), the ITU region names (*Naher Osten*, *Ozeanien*,
*Antarktis* …), *gezielter CQ-Ruf*, *Diplomprogramme*,
*DARC-Auslandsreferat / CEPT-Länderliste*, *Reports (Berichte) und
Recommendations (Empfehlungen)*, *Entry Level License / Novice License*,
*Lehrplan*, *Umzug ins Ausland*.

## Added to `DECISIONS.md` (Course text)

- German mnemonics (*Eselsbrücken*) keep their German words, with the
  English meaning in brackets; a mnemonic that is only the country's name
  takes the English name where it spells the same letters (France, Great
  Britain, mEXico).

## Judgement calls

- internationale_landeskenner (section and slides): mnemonics per the new decision — "Keiner Will Nach Amerika (nobody wants to go to America)", "Viele Elche (lots of moose)" (*Elch* in North America is the moose), "OEsterreich (Austria)", "Hohe Berge (high mountains), small / large" for *(klein) / (groß)*, *LAchse (Links Außen)* → "LAchse (salmon), Links Außen (far left)" (two mnemonics in one cell, each glossed); "Pyranhas" kept with its spelling (it plays on PY) and glossed "(piranhas)".
- internationale_landeskenner: *Funkpartner* → "the other station" (glossary §2); *Kapitel Amateurfunkstationen* → "the chapter on amateur stations"; *Fragenkatalog* → "question catalogue"; table cells without the article ("Netherlands", "Czech Republic", "Philippines"), as a list of names; *Vatikan* → "Vatican" (the ITU entity); trailing spaces after two table rows kept as in the German.
- itu_regionen: *Funkdienste* → "radiocommunication services" and the purpose sentence in VA401's wording ("different allocations of frequency bands to the radiocommunication services"); *Naher Osten* → "the Middle East"; the two Antarctica sentences joined with a colon.
- dx: *Kurzwelle / UKW* → HF / VHF (TRANSLATION.md), although the text then speaks of VHF and UHF; *erkennbar einige hundert Kilometer* → "evidently a few hundred kilometres away" (BE109); *sogenannten* → "what is known as"; *Diplomprogramme* → "award programmes"; *DX-Pedition* → "DXpedition" (BE312).
- dx slides: *DX Kurzwelle* → "DX on HF"; *Gezielter CQ-Ruf* → "Directed CQ call"; *Englische Sprache* → "The English language"; *80m Band* → "80 m band"; *Rufe Stationen …* → "Calling stations …".
- funken_im_ausland: *Reports (Berichte) und Recommendations (Empfehlungen)* → "Reports and Recommendations" (the brackets only translate the English back); *In den Prüfungsfragen wird die deutsche Übersetzung ECC-Empfehlung verwendet oder auch schlicht weg gelassen* → "In the German examination questions, the German translation *ECC-Empfehlung* is used, or the word is simply left out" — "German" added, because the English questions say "ECC Recommendation" and the sentence would otherwise be false for the English reader.
- funken_im_ausland: table kept as the German labels it (also "ECC Recommendation T/R 61-01/-02", see below); *Bezeichnung* → "Title"; *Harmonized* → "Harmonised" and *License* → "Licence" (glossary §1.1, §14); *Lehrplan* → "syllabus".
- funken_im_ausland: *CEPT-Regelungen* → "CEPT arrangements" (glossary, VB109); *Regelungen* otherwise "provisions" / "rules"; *DARC-Auslandsreferat* → "DARC foreign affairs department (DARC-Auslandsreferat)" at first mention, then without the bracket; *Jetzt Mitglied im DARC werden!* → "Become a DARC member now!"; slides *Werbung für DARC machen* → "Promote DARC".
- funken_im_ausland: the generic *er* after *Ausländische Funkamateure* → "they" (DECISIONS.md, generic *er*); „stroke“ → "stroke" with plain quotes.
- funken_im_ausland slides: *Zulassung zum Amateurfunkdienst* → "authorisation for the amateur service" (glossary §1.3); *ob man bereits eine Prüfung nach HAREC besitzt* → "if you have already passed an examination under HAREC".

## Suspected errors in the German original

- sections/funken_im_ausland.md (table n_funken_im_ausland_cept_empfehlungen) — T/R 61-01 and T/R 61-02 are labelled "ECC Recommendation"; they are CEPT Recommendations (originally of the CEPT T/R committee), as the questions call them (VB104, VB107, VB110, VB114 "CEPT Recommendation T/R 61-01"); only (05)06 is an ECC Recommendation.
- slides/funken_im_ausland.md (note on BD213) — "Deutsches Klasse-E-Rufzeichen erhält Schweizer Entry Level Präfix … Entry Level wird ein paar Folien später erklärt": Class E corresponds to the CEPT Novice licence (ECC (05)06; BD213 itself says "CEPT Novice Radio Amateur Licence"), while the section's table and the later slide make *Entry Level* Class N, which may not be used abroad at all.
- slides/funken_im_ausland.md ("Nationale Regelungen") — "das in Deutschland freigegebene 6 m-Band [ist] im Ausland beschränkt" states as a fact what the section only says may be the case ("bedeutet das nicht automatisch, dass man … darf").
- Typos with no effect on the English: sections/itu_regionen.md "Koordinerung"; sections/funken_im_ausland.md "HAREC-Bescheinung", "des DARC-Auslandsreferat" (*-s*), "für bis zu 3 Monaten" (*Monate*), "schlicht weg" (*schlichtweg*), "Ausländischen Funkamateure" (*Ausländische*) followed by singular "muss er", "das Prefix" (*Präfix*); slides/funken_im_ausland.md "der *Europäische Konferenz*" (*Europäischen*), "oder Länder mit geringer Funkaktivität" in slides/dx.md (*Ländern*); slides/dx.md "Länderkenner" (*Landeskenner*); sections and slides/internationale_landeskenner.md "Vereintes Königreich" (*Vereinigtes*).

## Provjera

Checked all 8 files paragraph by paragraph against `cc6b3e3~1` (German), with
the embedded questions (BD212–BD214, BD301–BD318, VA401–VA405, BB103–BB105,
BE104, BE109, BE110, BE113, BE114, BE312, VB101–VB114) read in English.
Nothing dropped or added; numbers, tags and idents intact
(`revizija-guard.py --rev cc6b3e3~1 --brojevi`: 8 files, *struktura
netaknuta*).

Changes: omission 0, meaning 0, technical 0, style 4, glossary 0.

- sections/internationale_landeskenner.md: *im Funkbetrieb* → "when operating" (was "in operation", which reads as "in service").
- sections and slides/internationale_landeskenner.md: *Oben Hinten* glossed "(up at the back)" (was "(top, at the back)").
- slides/dx.md (note on recognising distance): "The distance can be told from the country prefix, the locator, or call sign databases that give the QTH" (was "recognised from … or call sign databases with the QTH").
- slides/funken_im_ausland.md: *Ggf. je nach Amateurfunkklasse* → "Where applicable, depending on the licence class" (was "Possibly depending on the amateur radio class").

Judgement calls kept: all of them, including "German" added before
"examination questions" in funken_im_ausland (the English questions say "ECC
Recommendation", so without it the sentence would be false for the English
reader), *Kurzwelle / UKW* → HF / VHF, and the table's "ECC Recommendation
T/R 61-01/-02" labels kept as the German has them (slip reported). The 11
glossary rows and the DECISIONS.md entry on German mnemonics are kept
unchanged: the mnemonics only work through the German letters, and the
rows match the English questions (BD301 "the ITU's list of country
prefixes", VB109 "CEPT arrangement", VB113/VB114 "guest licence"). The
translator's suspected errors in the German stand as listed.
