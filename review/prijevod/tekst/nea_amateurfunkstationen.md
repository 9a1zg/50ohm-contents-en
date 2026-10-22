# nea_amateurfunkstationen — translation report

Chapter "Amateurfunkstationen" (Amateur stations): 14 sections, each with
its slides, no solutions. 28 files:

- `contents/sections/` and `contents/slides/`: `rufzeichenaufbau.md`,
  `persoenliche_rufzeichen.md`, `klubstationen.md`,
  `ausbildungsrufzeichen.md`, `remote_stationen.md`,
  `rufzeichenzusaetze.md`, `besondere_anlaesse.md`,
  `fernbediente_automatische_stationen.md`, `relaisfunkstellen.md`,
  `baken.md`, `linkstrecken.md`, `satelliten.md`,
  `exterritoriale_stationen.md`, `experimentelle_studien.md`.

`revizija-guard.py --brojevi`: 28 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (*personengebundene
Rufzeichen*, *Relaisfunkstellen*, *Relais*, *Repeater*, *Reinheitsgebot*,
*Amateurfunkzentrum*, *Türen auf mit der Maus!*, the `%` comments).

Embedded questions looked up in English and the prose aligned with them:
VC107, VC116, VC117, VA303, VA406, VD104, VD115–VD119, VD201–VD204,
VD208, VD301, VD302, VD304–VD306, VD401–VD408, VD501–VD504, VD601–VD609,
VE705, VE706, BD101–BD108, BD201–BD211, BE401–BE416, NE308–NE310, NE405,
NF113, NF118.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

27 rows: *personengebundene Rufzeichen (Amtssprache)*, the class labels
*Entry Level License / Novice / Advanced*, *Wunschrufzeichen*,
*Webabfrage*, *Notfunkklubstation*, *Sonderstation / Sonderrufzeichen*,
*Aktivierer / Sammler*, *Heimatstandort*, *Halteleinen*, *12-Meilen-Zone*,
the spoken suffixes (*Mobil*, *Portabel*, *Maritim Mobil*, *Aeronautisch
Mobil*), *besetzt / unbesetzt*, *ununterbrochene, mittelbare und
vollständige Kontrolle*, *Netzabschaltung*, *§ 16 Absatz 2 Satz 2 AFuV*,
*Frequenzablage / Ablage*, *Relaissteuerung*, *Wide-FM / Narrow-FM*,
*Subton mit CTCSS*, *Repeaterverzeichnis / relaisverantwortliche Person*,
*Relais oder Repeater*, *Linkstrecke / HAMNET-Knoten*, *Hoheitsgebiet*,
*Forschungsschiff / Polarforschungsstation*, the orbit names, *Nutzlast*,
*Bodenstationen* (RR 25.2A), *Reinheitsgebot / Amateurfunkzentrum*.

## Added to `DECISIONS.md` (Course text)

- Spoken call signs in examples use English voice procedure: digits in
  English, ITU code-word spellings (*Foxtrott* → Foxtrot, *Oskar* → Oscar),
  "Stroke Portable", "Mobile", "Maritime Mobile", "Aeronautical Mobile";
  German digits only where the text says it shows German national usage.

## Judgement calls

- All files: *BNetzA* and *AFuV* written out at first mention in each file, slides included — "Federal Network Agency (Bundesnetzagentur, BNetzA)", "Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)" — as the earlier units do, also where the German has only the abbreviation; *Anlage 1 der AFuV* → "Annex 1 to the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)".
- rufzeichenaufbau: *Die persönlichen Rufzeichen. In der Amtssprache nennen sich diese "personengebundene Rufzeichen"* → "personal call signs. In German official language they are called "personengebundene Rufzeichen" (call signs tied to the person)" — English has one term for both, so the official German one is quoted with a literal gloss; *(International Telecommunication Union, ITU)* → "(ITU)" (bracket only repeats the English).
- rufzeichenaufbau (slides): *Amateurfunkweltmeisterschaft WRTC 2018* → "the WRTC 2018 amateur radio world championship"; *früher DDR* → "formerly the GDR".
- persoenliche_rufzeichen: *Klasse N (Entry Level License)* → "Class N (Entry Level Licence)" — the German's English label kept, British spelling; *Wunschrufzeichen* → "preferred call sign"; *Webabfrage der BNetzA* → "BNetzA online search"; slides *Wortwitz* → "Wordplay", *Einfache Morsetelegrafie* → "Easy Morse telegraphy".
- klubstationen: *Stationsverantwortlicher* → "responsible radio amateur", as VD401; *Zeugnisklasse* → "certificate class"; *Leistungen und Bänder* → "powers and bands"; *freigegeben* → "open to Class E"; caption *des DARC-Ortsverbands Amberg* → "of the Amberg DARC local club"; slides *Wird in der Regel unbefristet zugeteilt* (no subject in the German, below a bullet about the responsible person) → "The call sign is usually assigned without a time limit".
- remote_stationen: AFuV definition translated faithfully, with the questions' terms (*mittelbare* → "indirect", VD605); *§2 Nr. 6a* → "Section 2 no. 6a"; *Störungen* here are faults, not interference ("in the event of faults, such as loss of connection"); *Netzabschaltung* → "switching off the mains supply".
- rufzeichenzusaetze: spoken examples in English voice procedure (DECISIONS.md); *Alpha* and *X-Ray* kept as the German writes them; *Zeppelin* → "zeppelin"; *Zuteilungsurkunde* → "assignment document", *Zulassungsurkunde* → "licence document" (glossary), each as the German has it.
- besondere_anlaesse: *Sonderstation* → "special event station" (RSGB); table: *Deutsches Reinheitsgebot* → "German Beer Purity Law (Reinheitsgebot)", *Amateurfunkzentrum* → "Amateur Radio Centre (Amateurfunkzentrum)" (the call sign DB50AFZ spells the German), *Amateurfunkgesetz* → "Amateur Radio Act (Amateurfunkgesetz, AFuG)" (DL73AFUG); *Türen auf mit der Maus!* kept as the event's German name, with "(Door Opener Day)" as the glossary names the same event.
- fernbediente_automatische_stationen: *besetzt / unbesetzt* → "attended / unattended".
- relaisfunkstellen: *Relaisfunkstellen werden auch kurz als Relais oder als Repeater bezeichnet* → "In German, repeaters (*Relaisfunkstellen*) are also called *Relais* or *Repeater* for short" — English has only *repeater*, and the German short forms are what a reader of the German exam will hear; slides likewise. The quoted definition uses VD118 b's English wording where the two coincide.
- relaisfunkstellen: *Frequenzablage oder auch einfach nur Ablage* → "repeater shift, or simply the shift"; table caption "Repeater shift"; *Schmalband-FM (Narrow-FM)* → "narrowband FM" (bracket dropped, §2); *Wide-FM* → "wide FM"; *Subton mit CTCSS* → "CTCSS subtone"; *im Empfangsbereich* → "within its coverage area"; slides *Es wird darauf verzichtet* → "It is not given".
- baken: *an polaren Nordlichtern* → "from the polar aurora (northern lights)"; German „…“ quotes → plain double quotes.
- linkstrecken: *Afu-$\qty{2,4}{\giga\hertz}$* → "the amateur 2.4 GHz … bands"; *WLAN-Router* → "Wi-Fi routers".
- satelliten: the gloss *("Umkreisender Satellit, der Amateurfunk mitführt")* and the slide note giving the same German expansion are dropped — they only translate the English name back into German (bracket rule); *mehrere 100 Satelliten* → "number in the 100s" (keeps the figure); orbit headings in the English names the German gives in brackets, *Hohe Umlaufbahnen (Geostationary Orbit - GEO)* → "High orbits (Geostationary Orbit, GEO)"; *2.000*, *35.786* → "2,000", "35,786".
- satelliten: *Steuersignale zwischen Bodenstationen und Amateurfunksatelliten … zum Zwecke der Verschleierung zu verschlüsseln* → "Control signals between earth command stations and amateur satellites may be encoded for the purpose of obscuring their meaning", the RR 25.2A wording of VA303 (the German paraphrases the RR); the next sentence's *Verschlüsselungsverfahren* (cryptography) → "encryption methods" (glossary *verschlüsseln*).
- exterritoriale_stationen, experimentelle_studien: *BRD* → "the Federal Republic of Germany"; *§ 16 Absatz 2 Satz 2 AFuV* → "Section 16(2) sentence 2 of the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)" (BD101, BD102 write "Section 16(2) AFuV").

## Suspected errors in the German original

- sections/relaisfunkstellen.md, slides/relaisfunkstellen.md — the "amtliche Definition" quoted ("eine fernbediente Amateurfunkstelle (auch in Satelliten), die … Signale fern ausgelöst aussendet und dabei zur Erhöhung der Erreichbarkeit von Amateurfunkstellen dient") is not the current AFuV wording, which VD118 a quotes ("fernbediente oder automatisch arbeitende Amateurfunkstelle … Inhalte fernausgelöst wieder aussendet oder weiterleitet"); it is distractor VD118 b without "ständig besetzt". The text then teaches how to eliminate b, but presents b's wording as the official definition.
- sections/rufzeichenaufbau.md — DN2JMU is given as an example of a personal call sign; DN1–DN8 are the (old) training call signs (slides/persoenliche_rufzeichen.md, slides/ausbildungsrufzeichen.md), and Class N personal call signs are DN9 only (table n_persoenliche_rufzeichen_praefixe, BD105).
- sections/persoenliche_rufzeichen.md vs slides — the section's table n_persoenliche_rufzeichen_praefixe lacks the DA6 row for Class E that the slides' table has.
- sections/remote_stationen.md — "Die Remotestation ist nach §2 Nr. 6a AFuV wie folgt definiert" introduces a definition of the remote *station*, but quotes the definition of remote *operation* (*Remote-Betrieb*).
- sections/linkstrecken.md — links "benötigen … immer eine Zulassung durch die BNetzA": what an automatically operating station needs is a call sign assignment (*Zuteilung*, VD501), not a *Zulassung*, which is the personal licence. Translated "authorisation".
- sections/satelliten.md (webindepth, GEO) — "da sie feste Signalempfangsstationen nutzen können": it is the ground stations that can use fixed antennas because the satellite stays put; as written the satellites use fixed receiving stations.
- Typos with no effect on the English: sections/rufzeichenaufbau.md "Personengebunde" and "Manchmal ist er" (*es*, das Präfix); "personengebunde" in the captions of both tables in sections/ and slides/persoenliche_rufzeichen.md; sections/klubstationen.md "den personengebundenem"; sections/ausbildungsrufzeichen.md "des Rufzeichenzusatz" (*-zusatzes*); slides/remote_stationen.md "die Stationen" (*Station*); sections/baken.md "ob … DX-Verbindungen … möglich ist" (*sind*); slides/besondere_anlaesse.md "73. Geburtstags", caption "200. Geburtstag" (the section has *Geburtstags*); sections/exterritoriale_stationen.md "International Raumstation", "Bundesrepublik Deutschlands", "Mit hilfe"; sections/satelliten.md ".:"; slides/relaisfunkstellen.md "Eingangsfrequenz" beside "Ausgabefrequenz" (the section has *Eingabefrequenz*); sections/rufzeichenzusaetze.md spoken table mixes *Oskar* (DL1FLO) and *Oscar* (DG2RON), and has *Alpha* for the ITU *Alfa*.

## Provjera

All 28 files compared paragraph by paragraph with `606c89b~1`; prose checked
against the English of every embedded question (VC107–VD609, BD101–BD211,
BE401–BE416, NE308–NE310, NE405, NF113, NF118, VA303, VA406, VE705, VE706).
`revizija-guard.py --rev 606c89b~1 --brojevi`: 28 files, *struktura
netaknuta*. The 27 glossary rows, the DECISIONS.md entry and every judgement
call above are kept.

Changes: omission 1, meaning 0, technical 1, style 5, glossary 0.

- slides/klubstationen: "Must be a licensed radio amateur" → "Must themselves be a licensed radio amateur" (*selbst* had been dropped).
- sections/baken: "from the polar aurora (northern lights)" → "from the aurora borealis" — *polare Nordlichter* is the aurora borealis; the added bracket only restated it.
- sections/rufzeichenaufbau: "In German official language" → "In official German usage".
- slides/ausbildungsrufzeichen: "Valid until now and until the end of 2028" → "Previously, and still valid until the end of 2028".
- sections/rufzeichenzusaetze: "you may use a call sign suffix voluntarily" → "you can choose to use a call sign suffix".
- sections/relaisfunkstellen: "Many repeaters do not like signals that are too wide at all" → "Many repeaters really do not like signals that are too wide" (the trailing "at all" read as part of "too wide").
- slides/satelliten: "satellites in orbit (now or in the past) number in the 100s" → "100s of satellites have been (or still are) in orbit".
