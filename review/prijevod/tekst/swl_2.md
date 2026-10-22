# swl_2 — translation report

Chapter "SWL-Kurs (2/2)": 17 sections, each with its slides, no solutions.
34 files:

- `contents/sections/` and `contents/slides/`: `swl_buchstabieralphabet.md`,
  `swl_abkuerzungen.md`, `swl_q_gruppen.md`, `swl_qso.md`, `swl_rst.md`,
  `swl_betriebsbeobachtung.md`, `swl_relais.md`, `swl_logbuch.md`,
  `swl_qsl.md`, `swl_rechtsgrundlagen.md`, `swl_abhoerverbot.md`,
  `swl_de_pruefung.md`, `swl_de_kennzeichen.md`, `swl_antrag.md`,
  `swl_dld.md`, `swl_dem.md`, `swl_abschluss.md`.

`revizija-guard.py --brojevi`: 34 files, *struktura netaknuta*. German-word
grep: no hits outside the words kept on purpose (*bergauf und bergab* in the
QSB memory aid, the award names *Deutschland-Diplom(-SWL)* and *Deutscher
Empfangsmeister*, *Distrikts-Ortsverbands-Kennziffer*, the German name of the
TDDDG). Line counts, the trailing spaces (sections: swl_qso lines 1, 7 and the
unterminated last line, swl_betriebsbeobachtung line 9, swl_qsl line 35,
swl_abhoerverbot line 1; slides: the two-space line break after
"**Matthias, DL9MJ**" in swl_abschluss), the missing final newlines
(sections: swl_buchstabieralphabet, swl_abkuerzungen, swl_qso, swl_rst,
swl_rechtsgrundlagen, swl_abhoerverbot, swl_de_kennzeichen) and the blank
lines at the ends of files are as in the German.

Embedded questions looked up in English and the prose aligned with them:
VD206, BA101–BA110 ("international phonetic alphabet"), BB102, BB103, BB106,
BB107 ("General call", "Long distance", "Transmitter, receiver,
transceiver", "Continuous Wave"), BB201–BB204 (Q code wordings, as §2),
BE201–BE208 ("readability", "signal strength", "tone", "reception report",
"SSB telephony"), NF103 ("S meter"), BE308 ("split operation"), BE408 (only
the readability "R" with a repeater), BG105–BG108, BG110 ("mode", UTC, CET,
CEST, "callbook"), VC101, VC104, VC105, VC111 ("radio amateur within the
meaning of the Amateur Radio Act", "harmonised … examination certificate",
"Only with other amateur stations"). SWL001–SWL003 are in
`contents/questions/fragenkatalog_swl.json`, still German (outside this
unit); swl_abhoerverbot is written in the terms of the existing
fernmeldegeheimnis_abhoerverbot section and VE202/VE203 (*Fernmeldegeheimnis*,
"the general public, an unspecified group of people", "eavesdropping on
private (non-public) conversations", "emergencies and disasters"), so that it
fits them once they are translated.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

8 rows: *Deutschland-Diplom-SWL / Deutschland-Diplom / Sonder-DOK /
Diplomregeln*; *Deutscher Empfangsmeister / Grundstufe / Bronze, Silber, Gold
/ korporativer Verband / Ausschreibungsbedingungen*;
*Distrikts-Ortsverbands-Kennziffer*; *Ortsverbandsvorsitzende /
Distriktsvorsitzende / AJW-Distriktsreferent / DL-AJW-Referat / Vorstand /
DARC-Regularien*; *Wunschkennzeichen / Wunschsuffix / Suffixkombination /
Vergabeschlüssel / Vergabestelle / Urkunde / Kennzeichenbereich*; *geprüfte
Empfangsstation / geprüfter SWL / Ausbildungsempfangsstation / Höramateur,
Empfangsamateur*; *Prüfungskommission / Fragebogen, Prüfungsbogen /
Probeprüfung*; *Hörpause / Hörübung / wertbare Verbindungen /
Tabellenkalkulation*.

## Added to `DECISIONS.md`

One entry (Course text): the DARC's SWL award titles keep their German names
with an English gloss at first mention in a file — *Deutschland-Diplom-SWL*
(Germany Award for SWLs, DLD-SWL), *Deutscher Empfangsmeister* (German
Reception Master, DEM) — because the abbreviations spell the German words, as
*DE* spells *Deutsche Empfangsstation*.

## Judgement calls

- swl_buchstabieralphabet: *Delta Lima Eins …*, *Delta November Neun …* → "One", "Nine" (DECISIONS.md, spoken call signs: German digits stay only where the text says it shows German national usage, which this one does not); "Stroke portable" kept in the German's casing, as glossary §2; table header *Buchstabe / Wort* → "Letter / Word", as buchstabiertafel; *Nationale Buchstabiertafeln* → "National phonetic alphabets"; *nicht vorgesehen* → "not provided for this purpose".
- swl_abkuerzungen: *de bedeutet von* → '*de* means *this is*', as the abbreviation table (DE "This is") and swl_rufzeichen; table cells capitalised like betriebliche_abkuerzungen; *Transceiver, also Sendeempfänger* → "Transceiver, that is, a combined transmitter and receiver" (nea_abkuerzungen), slide *oder Sendeempfänger* → "or combined transmitter and receiver"; *Gerät arbeitet im RX-Betrieb* → "works in RX mode".
- swl_q_gruppen: Q code meanings in the ITU wording (DECISIONS.md, glossary §2): QRN *durch atmosphärische Störungen beeinträchtigt* → "I am troubled by static", QRT *Stellen Sie die Übermittlung ein* → "Stop sending", QSB? → "Are my signals fading?", both German wordings of QSL? → "Can you acknowledge receipt?", QSO? *mit einer bestimmten Station* → "Can you communicate with ... direct?" (as the looser German in q_schluessel); QRM keeps the German's addition: "I am being interfered with by other stations". Column *Gruppe* → "Code". Memory aid by the mnemonic decision: "*m*an-made", "*n*atural", "*s*ignal strength", "*b*ergauf und *b*ergab" kept German with its meaning.
- swl_qso: `<qso>` in English voice procedure (DECISIONS.md), following betriebsabwicklung: *hier ist … mit einem allgemeinen Anruf … und geht auf Empfang* → "this is … making a general call, … listening"; *DL9MJ von DL1FLO* → "DL9MJ this is DL1FLO"; *du bist bei mir 5 und 7* → "you are 5 and 7 here"; *die nebenstehende Abbildung* → "the example opposite" (it is a QSO block, not a figure); *angeschriebene Station* → "the station you write to / the station written to"; *ihre Gegenstation* → "the station it was in contact with" (§2 *Gegenstation*).
- swl_rst: *Lesbarkeit (Readability)*, *Signalstärke – Signal Strength*, *Tonqualität – Tone* → "Readability", "Signal strength", "Tone" (bracket rule); *Rapport* → report, *Empfangsrapport* → reception report (BE207); *S9 und weiteren 20 dB* → "S9 plus a further 20 dB".
- swl_betriebsbeobachtung: *wertbare Verbindungen* → "valid contacts"; *Split-Verkehr* → "split operation" (BE308); *gesuchte Station* → "the station being sought", *begehrte Station* → "sought-after station" (§2); *Durchgang* → over; *Hörübung* → "listening exercise"; slide *dokumentiert* → "logged".
- swl_relais: *Relaisfunkstelle / Relais* → repeater, *Funkrunde* → net, *Eingabe-/Ausgabefrequenz* → input / output frequency (§2); *Kennungen* → "Identifiers" (§1.3 *Kennung*); *sich melden* → "call in".
- swl_logbuch / swl_qsl: *Übertragungsverfahren* in the lists of log and card details → "mode", as BG105 and §1.3 *transmission method; mode* (swl_was_ist_swl's running text has "transmission method"); [index:Logbuch] → [index:Log]; *MEZ / MESZ* → CET / CEST (BG107, BG108); *Callbooks* → callbooks; *stabiler Karton* → "stiff card"; the tip's closing link "[Become a DARC member now!]" as swl_was_ist_swl; *Vermittlungsbüros* → "bureaus" (glossary §14).
- swl_rechtsgrundlagen: AFuG, AFuV and BNetzA in full at first mention in the section and on the slides, then abbreviations (*Das Amateurfunkgesetz unterscheidet* → "The AFuG distinguishes"); *Höramateur* set against *Funkamateur* → "listening amateur … not yet a radio amateur in the legal sense"; *Zulassung zum Amateurfunkdienst* → "authorisation to participate in the amateur service", as swl_1 and the slide's *Zulassung zur Teilnahme*; bare *Zulassung* → licence (§1.3); *vereinsinterne Prüfung des DARC* → "an internal examination of the DARC as an association".
- swl_abhoerverbot: TDDDG in full at first mention, as fernmeldegeheimnis_abhoerverbot; the slide's bare "§ 5 TDDDG" → "Section 5 TDDDG"; *abhören* → "listen to", *Abhören des nicht öffentlich gesprochenen Wortes* → "eavesdropping on private (non-public) conversations" (§1.2); *Schutz wichtiger Rechtsgüter* → "protection of important legal interests"; the prescriptive present (*werden weder aufgezeichnet noch weitererzählt*) → "should be neither recorded nor passed on", as the swl_1 checker.
- swl_de_pruefung: *Probeprüfungen* → "practice examinations"; *Fragebogen* / *Prüfungsbogen* → "question paper" / "examination paper"; *abnehmen* → "conduct"; *Ortsverbandsvorsitzende*, *Distriktsvorsitzende*, *AJW-Distriktsreferent*, *DL-AJW-Referat* → "local club chair", "district chair", "district AJW officer", "DL-AJW department" (AJW not expanded, as VFDB); *körperliche Einschränkungen* → "physical disabilities"; *Betriebstechnik* → "Operating practice".
- swl_de_kennzeichen / swl_antrag: *geprüfte Empfangsstation*, *geprüfte SWLs* → "qualified receiving station", "qualified SWLs"; *Urkunde* → certificate; *Wunschkennzeichen* → "preferred identifier" (as *Wunschrufzeichen*); *Zuteilung … erlischt* → "the assignment lapses"; *Amateurfunkgenehmigung* → amateur radio licence; *5 Euro* → "5 euros"; *Kontodaten* → "bank details"; *Lehrgänge* → courses.
- swl_dld / swl_dem: award names by the new DECISIONS.md entry; photo captions *Deutschland-Diplom-SWL* kept as the name, *Urkunde Deutscher Empfangsmeister (Kategorie Gold)* → "Deutscher Empfangsmeister certificate (Gold category)"; *DOK* expansion kept in brackets, since the text defines it; *korporativer Verband* → "affiliated association"; *Kurzwellenempfänger* → "HF receiver" (swl_1); the slide's *Der Deutsche Empfangsmeister (DEM) ist eine Auszeichnung* → "The Deutscher Empfangsmeister (DEM), the German Reception Master, is a DARC award"; *Empfangsmeister erhalten* → "Holders of the title receive".
- swl_abschluss: *vy 73 und 55! / Wünschen Matthias … und Florian …* → "vy 73 and 55! / With best wishes from Matthias DL9MJ and Florian DL1FLO" (the meanings were glossed in swl_vorwort); slide *Viel Erfolg und viel Freude beim Zuhören wünschen dir* → "Wishing you every success and lots of fun listening,"; *Lernweg* → "the right next thing to study for".

## Suspected errors in the German original

- sections/swl_dld.md and slides — "Der *DOK* ist die Distrikts-Ortsverbands-Kennziffer": elsewhere the course expands DOK as *Distriktsortskenner* (N_Ende, swl_was_ist_swl), and a DOK is a letter-and-digit code (B17), not a *Kennziffer*; the slide also narrows it to "einer DARC-Station" where the section says "eines DARC- oder VFDB-Ortsverbandes". Kept, the expansion in brackets.
- slides/swl_rechtsgrundlagen.md — "wer ein Amateurfunkzeugnis oder eine anerkannte ausländische Prüfungsbescheinigung besitzt": the section and the AFuG (VC105) say *harmonisierte* (harmonised) examination certificate; it is the harmonisation, not the foreign origin, that counts. Kept ("recognised foreign examination certificate").
- sections/swl_q_gruppen.md and slides — QRM "Ich werde durch andere Stationen gestört": QRM is man-made interference in general, not only from other stations (q_schluessel names a photovoltaic system as an example). A narrowing. Kept, with the ITU wording plus "by other stations".
- sections/swl_qso.md — "Die nebenstehende Abbildung zeigt ein Beispiel": the example is a `<qso>` dialogue block, not a figure. Rendered "The example opposite".
- Typos and style with no effect on the English: sections/swl_qso.md "Am Ende des QSO wird sich in der Regel verabschiedet" (impersonal reflexive), trailing space after "DL1FLO hier ist DL9MJ" (kept); sections/swl_abschluss.md "Wünschen Matthias …" (capital after a line break).
