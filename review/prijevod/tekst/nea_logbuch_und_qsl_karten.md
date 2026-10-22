# nea_logbuch_und_qsl_karten — translation report

Chapter "Logbuch und QSL-Karten" (Log and QSL cards): 2 sections, each with
its slides, no solutions. 4 files:

- `contents/sections/` and `contents/slides/`: `logbuch.md`, `qsl_karten.md`.

`revizija-guard.py --brojevi`: 4 files checked, *struktura netaknuta*.
German-word grep: one hit, the `%` comment in sections/qsl_karten.md
(`%[photo:12:…:Gemeinsame QSL-Karte … (Vorderseite)]`), unchanged. Line
counts, blank lines, the trailing space after "the following details:" in
sections/qsl_karten.md, the double space after "(Bundesnetzagentur, BNetzA)."
in the SWL box, the leading `---` of sections/logbuch.md and the trailing
blank line of slides/logbuch.md are as in the German.

Embedded questions looked up in English and the prose aligned with them:
BG101–BG111, VD108, VD109 (BG101 "station log … keeps voluntarily",
BG102/BG103 "When keeping a log has been ordered", "paper log", "computer
log", "logging software", "available for inspection for a certain period",
VD108 "to investigate causes of interference or to clarify questions of
frequency engineering", BG105 "date and time … in UTC, band, mode and signal
report", BG106 "Coordinated Universal Time (UTC)", BG107/BG108 CET / CEST,
BG109 "QSL via K8PYD", "QSL manager", BG110 "international amateur radio
call sign list (callbook)", BG111 "electronic QSL cards or log upload").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

8 rows: *Logbuchführung / verpflichtende Logbuchführung / Aufbewahrung des
Logbuchs*; *Logbuch-Software / Logdatei / Praxis-Tipp*; *Universal Time
Coordinated / Sommerzeit / Winterzeit*; *Amateurfunk-Diplom / Kurzzeitdiplom
/ Urkunde*; *Vermittlungsbüro / QSL-Vermittlung (international "Bureau") /
via-Feld*; *Bildmotiv / persönliches Motiv*; *DARC QSL-Service / DCL /
Wavelog / Drittanbieter*; *Datenträger*.

## Added to `DECISIONS.md`

None.

## Judgement calls

- logbuch: *Logbuch* → "log" throughout (glossary §1.3, §2, BG101), "logbook" only for the ship's and aircraft's logbook; *Stationstagebuch* → "station log" (BG101), in the section without italics as in the German, on the slide in italics as in the German.
- logbuch: *Übertragungsverfahren* in the lists → "Mode" (BG105); *Vergebener und erhaltener Rapport* → "Report given and received"; *Name des QSO-Partners oder eigene verwendete Station* → "the other operator's name or the station you used".
- logbuch: *Aufforderung der Bundesnetzagentur* → "request from the Federal Network Agency (Bundesnetzagentur, BNetzA)", full form at first mention in the section and on the slides (also in the qsl_karten SWL box and slide).
- logbuch: *UTC (von Universal Time Coordinated)* and the slide's *UTC (Universal Time Coordinated)* kept as written, although the English name is Coordinated Universal Time (see suspected errors); the sentence before it gives the correct English name from the glossary.
- logbuch: *Winterzeit / Sommerzeit* → "winter / summer time" (British *summer time*); *bei uns* → "here"; *wir erinnern uns* (qsl_karten) → "Remember:".
- logbuch: *Praxis-Tipp:* → "*Practical tip:*"; *Drittanbieter* → "third-party services"; *DCL* (DARC Community Logbook) kept as the name; link text *Video* → "video".
- logbuch slides: headings *Verpflichtende Logbuchführung* → "Mandatory log-keeping", *Aufbewahrung des Logbuchs* → "Keeping the log available" (the slide is about the log remaining available for inspection, not about storing it); *Wechsel Papier $\rightarrow$ elektronisch* → "Switching from paper $\rightarrow$ electronic"; *Hier DARC-Mitgliedschaft bewerben* → "Promote DARC membership here".
- qsl_karten: *Amateurfunkverband* → "national amateur radio society" where it means the national societies (bureau, callbooks, awards issued by societies such as the DARC, the ARRL), as the iaru_bandplan section has it; *Amateurfunkvereinigungen, denen der Funkamateur angehört* and the slide's *Amateurfunkvereinigungen* → "amateur radio societies" (glossary §13).
- qsl_karten: *die sogenannte QSL-Vermittlung* → "known as the *QSL bureau*" (glossary §2), *Vermittlungsbüro - international "Bureau" genannt -* → "the bureau": the gloss only gives the English word and is dropped by the bracket rule (DECISIONS.md), also on the slide (*via Vermittlungsbüro - international "Bureau"* → "Via the QSL bureau").
- qsl_karten: Q code QSL → "I am acknowledging receipt" (ITU wording, DECISIONS.md Q code meanings), section and slide.
- qsl_karten: generic *er* recast (DECISIONS.md): *wenn er eine bestimmte Anzahl an Funkverbindungen … erreicht hat* → "after making a certain number of contacts that meet certain requirements".
- qsl_karten: *Eine Unterschrift der Karte ist seit einigen Jahren nicht mehr notwendig* → "For some years now, the card no longer needs to be signed".
- qsl_karten: *DARC QSL-Service* kept as the service's name; *Bildmotiv* → "picture"; *deutlich vergünstigt* → "much cheaper".
- qsl_karten: *Hörerkennzeichen* → "short-wave listener identifiers" (glossary §2); *sogenannten SWLs (vom englischen "short wave listener")* → "short-wave listeners, known as SWLs" — the bracket only explains the English word; slide *Hörerkennzeichen (short wave listener)* → "*short-wave listener identifiers*" without the bracket; slide heading *Short Wave Listener (SWL)* → "Short-wave listeners (SWL)" in sentence case.
- qsl_karten: attention box *möglichst präzise Uhrzeit* → "as *precise a time* as possible", keeping the emphasis on the time.
- qsl_karten: captions *Gemeinsame QSL-Karte … (Vorderseite / Rückseite)* → "Joint QSL card of DL4EAX and DM4EAX (front / back)", *Urkunde des DX Century Clubs* → "DX Century Club certificate"; the `%` comment keeps its German caption.
- qsl_karten slides: *Angaben* → "Details"; *Vermittlung von QSL-Karten* → "Distributing QSL cards"; *Es gibt abenteuerliche Wege, wie die Karten zugestellt werden* → "Cards sometimes reach their recipients by adventurous routes"; *Im via-Feld der QSL-Karte eintragen* → "Enter them in the via field of the QSL card"; *Diplom als Zertifikat über gewisses Funkkönnen* → "An award as a certificate of a certain operating skill".

## Suspected errors in the German original

- sections/logbuch.md and slides/logbuch.md — "*UTC* (von Universal Time Coordinated)" / "UTC (Universal Time Coordinated)": the English name is *Coordinated Universal Time* (French *temps universel coordonné*); "UTC" is a language-neutral compromise abbreviation (ITU-R TF.460), not the initials of "Universal Time Coordinated". Kept.
- sections/logbuch.md (in-depth box) — "Im Jahre 1972 wurde die UTC als universelle und weltweit einheitliche Uhrzeit eingeführt": coordinated time signals under the name UTC were in use from the 1960s; what began on 1 January 1972 is UTC in its present form (SI second, leap seconds). Imprecise rather than wrong. Kept.
- Typos with no effect on the English: sections/logbuch.md "In Berlin ist es ist 9:00 MEZ" (doubled *ist*), "zu einem elektronisch per Computer geführtem Logbuch" (*geführten*); sections/qsl_karten.md "eine eingereichte QSL-Karten nicht anerkannt wird" (*QSL-Karte*).
