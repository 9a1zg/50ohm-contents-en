# nea_abkuerzungen — translation report

Chapter "Abkürzungen" (Abbreviations): 4 sections, each with its slides, no
solutions. 8 files:

- `contents/sections/` and `contents/slides/`: `betriebliche_abkuerzungen.md`,
  `q_schluessel.md`, `locator.md`, `N_Ende.md`.

`revizija-guard.py --brojevi`: 8 files checked, *struktura netaknuta*.
German-word grep: no hits outside the German cue words kept on purpose in
the mnemonics (*ich bin vorbereitet*, *ein zweites Mal*, *bergauf und
bergab*, *Kommen*, *große Leistung*), the German names of the locator levels
(*Feld*, *Quadrat*, *Unter-Quadrat*, *Größtfeld*, *Großfeld*, *Kleinfeld*),
*Sender* / *Empfänger*, *Ortsverband*, *Distriktsortskenner*, proper names
(DARC-Chat, DARC-Treff, Dienstags-Treff, Funk.Tag) and URLs. Line counts, the
trailing spaces in the betriebliche_abkuerzungen table (PSE, TX rows), the
whitespace-only lines (sections/q_schluessel.md line 24, slides line 10), the
two trailing spaces before the signature and the missing final newline of
sections/N_Ende.md are as in the German.

Embedded questions looked up in English and the prose aligned with them:
BB106, BB107, VA407, BB201–BB206, BE107, BE115, BE111 (BB106 "transmitter,
receiver, transceiver"; BB107 "Continuous Wave"; BB204 "I am ready", "Are
you being interfered with?", "My location is ..."; BB203 "Stop sending.",
"Who is calling me?", "Can you acknowledge receipt?"; BB202 "Shall I
increase transmitter power?", "Can you communicate with ... direct?", "When
will you call me again?"; BB201 "I am being interfered with."; BB205/BB206
"transmit power", "change frequency"; BE115 "inviting further stations to
call", "pile-ups"; BE111 "QTH locator or grid locator", "fields and
squares"). Table rows for the operating abbreviations follow the
funkfernschreiben table (BK "Interruption of the transmission; informal
handover", K "Invitation to transmit", R "Received", BB108–BB110).

## Added to `TRANSLATION_GLOSSARY.md` (§14)

12 rows: the Q code mnemonics; *Atmosphärische / menschengemachte Störungen,
schwankende Zeichen, Frequenzwechsel*; *QRP-Betrieb / -Geräte /
-Verbindungen*; *Locator-System / QTH-Locator / Kästchen*; *Feld / Quadrat /
Unter-Quadrat* with *Größtfeld / Großfeld / Kleinfeld*; *DARC-Geschäftsstelle*;
the OpenStreetMap / OpenTopoMap attributions; *Distriktsortskenner (DOK) /
Distrikt*; *Lern-App / Prüfungstrainer / Trainingsapp*; *Nachwuchsförderung*;
*Nach der Prüfung ist vor der Prüfung*; the names of DARC services and events.

## Added to `DECISIONS.md`

One entry (Course text): letter mnemonics that mark one letter — English
where a faithful rendering of the cue keeps the letter (*m*an-made,
*n*atural, *l*ogged, *o*n top, at time *X*), otherwise the German cue with
its English meaning (*v*orbereitet, *z*weites Mal, gr*o*ße Leistung,
*b*ergauf und *b*ergab, *K*ommen); a German gloss of an English cue
(*H*eimat, *Beenden*) dropped.

## Judgement calls

- betriebliche_abkuerzungen: table cells by the funkfernschreiben convention (DECISIONS.md): *Bitte, Please* → "*P*lea*se*", *Receiver (Empfänger)* → "Receiver", *Transmitter (Sender)*, *Transceiver (Sendeempfänger)* likewise; the slide's *Allgemeiner Anruf (vom Englischen "Seek You")* → 'General call (from "seek you")'; K → 'Invitation to transmit ("*K*ommen", German for "over")'.
- betriebliche_abkuerzungen: *viele unserer Fachbegriffe aus dem amerikanischen Englisch, beispielsweise Transmitter statt Sender* kept as information about German usage (DECISIONS.md, USB remark): "*transmitter* instead of the German *Sender*"; *der Transceiver, also der Sendeempfänger* → "the transceiver, that is, the combined transmitter and receiver".
- betriebliche_abkuerzungen: *als die Bedeutung "Allgemeiner Anruf"* → 'than its meaning, "general call"' — the point (the abbreviation is shorter) holds in English, so it is not quoted as German usage; *Zeichen* (R, K) → "sign"; *Durchgang* → over (§2).
- q_schluessel: Q code meanings in the ITU wording where the German gives a German wording (DECISIONS.md): QRT "Stop sending", QRZ? "Who is calling me?" (also for the table's *Wer hat mich gerufen?*), QSO? "Can you communicate with ... direct?" (also for the table's looser *Erreichen Sie Station ...?*), QSL "I am acknowledging receipt", QRO "Increase transmitter power!", QRP "Decrease transmitter power!"; descriptive cells (*Atmosphärische Störungen*, *Fading, Schwankungen*, *Frequenzwechsel*) translated plainly.
- q_schluessel: *QRV bedeutet, dass man empfangsbereit ist* → "you are ready to receive"; *ich mache QRT* → "I am going QRT"; *QSO … freizügige, aber übliche Interpretation* → "a loose but common interpretation"; *"abgearbeitet"* → '"worked through"'; *Pile Up* → "pile-up" (glossary, BE115).
- q_schluessel: QRM *Werden Sie durch "Menschengemachte" Störungen gestört?* → 'Are you being disturbed by "*m*an-made" interference?', to avoid "interfered with by … interference"; QRO's two cues: "high power (in German "gr*o*ße Leistung")" and "Shall I put a few more watts *o*n top?"; slide *gr*o*ße Leistung* likewise kept German.
- q_schluessel slides: *Wann werden Sie mich zum Zeitpunkt X wieder rufen?* → "When will you call me again (at time *X*)?" (the section's two questions merged in the German; see errors); note *Wo ist Dein Standort?* → "What is your location?" (BB203 c).
- q_schluessel: margin *Telegrafie mittels CW oder digitalen Übertragungsverfahren* → "telegraphy using CW or digital modes" (operating sense, nea_digitale_uebertragungsverfahren_1).
- q_schluessel: table headings *Bedeutung / Merkhilfe* → "Meaning / Memory aid" (§14 *Merkhilfe*); *P*ssst! kept as written.
- locator: *Felder (englisch fields)*, *"squares" (Quadrate)* → "*fields*", '"squares"' (bracket rule); the level table keeps its German columns as information about German usage, headed "German" and "Alternative German name" (*Übersetzung* would be meaningless in English, and *Größtfeld / Großfeld / Kleinfeld* are the names German operators also use); *Bezeichnung* → Name, *z.B.* → "e.g.".
- locator: *Standortkenner oder QTH-Locator* → "grid locator or QTH locator" (BE111); *Kästchen* → box; *Ortsbezeichnungen* → "naming a place"; *Entfernungsmessungen* (slide) → "working out distances"; *Noch kleinere Felder sind möglich* → "Even smaller boxes are possible" (not *fields*, which is the top level); *DARC-Geschäftsstelle* → "DARC head office"; *Hessen* → Hesse; *180. Längengrad* → "180th meridian".
- locator: captions *Kartendaten © OpenStreetMap-Mitwirkende … Kartendarstellung © OpenTopoMap* → "Map data © OpenStreetMap contributors … Map style © OpenTopoMap", the services' own English attribution.
- N_Ende: *der DARC* → "the DARC", as in earlier units; *Bundesnetzagentur* written out at first mention, "Federal Network Agency (Bundesnetzagentur, BNetzA)", the slide keeps "BNetzA"; *DARC-Ortsverband (OV)* → "DARC local club (Ortsverband, OV)" (§14), *OV* kept afterwards as the German does; *Distriktsortskenner (DOK)* → "*district local club identifier* (Distriktsortskenner, DOK)".
- N_Ende: menu item *[Prüfung]* → "[Examination]" (the static pages are translated later in this project, so the menu will be English; not bracketed like the applet labels); link text *[Mitarbeiterinnen und Mitarbeitern erarbeitet]* → "[developed by many volunteer contributors]"; *Funkamateurinnen und Funkamateure*, *frisch gebackene Funkamateurin oder Funkamateur*, *Besucherinnen und Besuchern* → plain "radio amateurs", "a newly licensed radio amateur", "visitors" (English has no gendered pair).
- N_Ende: *Nach der Prüfung ist vor der Prüfung* → "*after the exam is before the exam*", literal (glossary row; the *denn* clause explains it); *Dienstags-Treff* kept as the name with "(Tuesday meeting)"; *10.000* → "10,000" (English thousands separator, as earlier units); *Bodensee* → Lake Constance; *Selbstbau* → home construction (§14).
- N_Ende: closing line *Viel Spaß … wünschen stellvertretend für das 50ohm.de-Team / Lars DC4LW und Matthias DL9MJ* → "On behalf of the *50ohm.de team*, we wish you lots of fun with your new hobby! / Lars DC4LW and Matthias DL9MJ" (the signers as "we"); slide *Geschafft!* → "You did it!".

## Suspected errors in the German original

- sections/betriebliche_abkuerzungen.md — 'Das "R" (received, bzw. roger) … ist eines der wenigen Zeichen, das ausschließlich in der Telegrafie genutzt wird': the letter R as a sign is telegraphy-only, but its spoken form "Roger" (which the same sentence names) is common in telephony. Imprecise. Kept.
- sections/betriebliche_abkuerzungen.md — "Der Ursprung des Amateurfunks ist in den USA": amateur radio grew up at the same time in several countries (the UK's first amateur licences and societies date from the same years as the ARRL); the US influence on the vocabulary is real, the single origin is a simplification. Kept.
- sections/locator.md — "in 18 mal 18 gleich große Bereiche": the fields are equal in angular extent (20° × 10°), not in area; near the poles they are much smaller. The in-depth box on the squares hints at this. Kept.
- slides/q_schluessel.md — "Wann werden Sie mich zum Zeitpunkt *X* wieder rufen?": merges the section's two questions (*Wann werden Sie mich wieder rufen?* / *Werden Sie mich zum Zeitpunkt X wieder rufen?*) into one that asks "when" and gives the time. Rendered with the time in brackets.
- Typos with no effect on the English: sections/betriebliche_abkuerzungen.md "Die Anwendung dieser Abkürzung" (*Abkürzungen*), "Morsetelegraphie" in the tables beside "Morsetelegrafie" in the prose; sections/locator.md "ähnlich der Felder" (*wie bei den Feldern*); slides/locator.md "Stufen des Maidenhead Locators" (hyphen), "DARC Geschäftsstelle"; slides/q_schluessel.md "angehangen" (*angehängt*).

## Provjera

Checked all 8 files paragraph by paragraph against `839ca81~1`, the embedded
questions (BB106, BB107, VA407, BB201–BB206, BE107, BE111, BE115) in English,
the glossary and DECISIONS.md. Nothing dropped or added apart from the
closing line below; the Q code wordings follow §2 and the ITU entry; the
table cells follow the funkfernschreiben convention. Kept as they are: all
judgement calls, the 12 glossary rows, the DECISIONS.md entry on letter
mnemonics, and the suspected errors in the German (all four are fair).
`revizija-guard.py --rev 839ca81~1 --brojevi`: 8 files, *struktura netaknuta*.

Changes: omission 0, meaning 1, technical 0, style 8, glossary 0.

- N_Ende section, closing line: "On behalf of the *50ohm.de team*, we wish
  you lots of fun with your new hobby!" → "With best wishes for lots of fun
  with your new hobby, on behalf of the *50ohm.de team*" — the German has
  no exclamation mark and no "we"; the signers below are its subject.
- q_schluessel section: QRM 'Are you being disturbed by "*m*an-made"
  interference?' → 'Are you suffering from …' (natural English, still
  avoids "interfered with by … interference").
- q_schluessel section and slide: *"abgearbeitet"* → '"worked" a caller'
  instead of '"worked through"': *work* a station is the operating term.
- q_schluessel margin: "bridge the greatest possible distances" → "cover"
  (Germanism).
- betriebliche_abkuerzungen section: "a firm part of everyday language
  among radio amateurs" → "an established part of the everyday language of
  radio amateurs".
- N_Ende section: "prepare … in a focused way" → "prepare specifically";
  "The members on the spot" → "The local members".
- N_Ende slide: "Works for frequencies, training and young people" →
  "Stands up for …" (*setzt sich ein*; "works for" reads as employment).
