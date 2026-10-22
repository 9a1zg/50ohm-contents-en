# nea_digitale_uebertragungsverfahren_1 — translation report

Chapter "Digitale Übertragungsverfahren (1/3)" (Digital transmission methods,
part 1): 11 sections, each with its slides, no solutions. 22 files:

- `contents/sections/` and `contents/slides/`: `analog_vs_digital.md`,
  `binaer.md`, `morsetelegrafie.md`, `computersteuerung.md`,
  `funkfernschreiben.md`, `digimode_ssb.md`, `9600_port.md`,
  `digimod_uebersteuerung.md`, `automatische_empfangsberichte.md`,
  `digital_voice.md`, `paketvermittelte_netzwerke.md`.

`revizija-guard.py --brojevi`: 22 files checked, *struktura netaknuta*.
German-word grep: no hits outside the `%` comments (the commented-out in-depth
box of analog_vs_digital, the seven commented-out photos of funkfernschreiben,
the `% TODO` table of digital_voice, all unchanged), the letters Ä, Ö, Ü, ẞ in
the Morse tables (characters of the code, unchanged) and the German words
named on purpose (*Dualsystem*, *Dualzahl*, *Binärzahl*). Line counts, blank
and whitespace-only lines (funkfernschreiben line 50, 9600_port line 24, the
indented example lines of slides/paketvermittelte_netzwerke), trailing spaces
(binaer, the Morse tables, 9600_port, automatische_empfangsberichte,
digital_voice, the HAMCloud margin) and the final-newline state are as in the
German in every file.

Embedded questions looked up in English and the prose aligned with them:
EA201–EA208, VA304, BE112, BE117, BE118, BB101, BB108–BB110, NE307,
NE401–NE404, NF114–NF117, EE402–EE405, EE412–EE415, EF219, EF309,
EJ217–EJ219 (e.g. BE118 "no faster than I can receive myself", BB101
"information content transmitted per unit of time", BB108 "informal
handover", BB109 "Invitation to transmit", BB110 "Received", NE401 "by
radioteletype", "same transmission method", NF115 "analogue data port (e.g.
labelled DATA or called a 9600 port)", "tap off or feed in", NF116 "CAT
interface", NF117 "unexpectedly switch to transmit", EE403 "AF bandwidth" /
"RF bandwidth", EE405 "automatic reception reports", NE402 "repeater
network", "reflector, time slot or colour code", NE403 "voice contacts",
"time slots", EE412 "intermediate stations (packet forwarding)", EE413
"subnet mask", "router", EJ217–EJ219 "digital modes", "automatic level
control (ALC)", "intervenes", "AF level").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

20 rows: *Digimode / Digimodes / Digimode-Interface* (course text, beside
*digitale Übertragungsverfahren*); *Informationsübertragung /
-übermittlung*; *Zehnersystem / Dualsystem, Dualzahl*; *Stelle / Stellenzahl
/ Breite / Ziffernvorrat*; *Fernschreiber / Funkfernschreiber*; the Morse
special characters (*Unterbrechung (BK)* … *Korrektur*); the telegraphy
abbreviation table; *Startsound / Benachrichtigungstöne*; *Hardware-Modem /
TNC / Packet-Radio*; *DATA-Port / 9600-Anschluss*; *Audiopfad /
De-Emphasis-Prozess*; *Empfangsbericht / Skimmer-Stationen /
Internetplattformen*; *Repeaternetzwerk / Relaisverbund /
Richtfunkanbindung*; *Raum / Zeitslot / Zeitschlitz*; *TDMA … oder
Zeitmultiplexverfahren*; *Reaktions- und Haltezeit*; *Farbtiefe / zeilenweise
/ Bewegtbilder*; *Einstiegspunkt / Knoten mit Benutzerzugang /
WLAN-Transceiver*; *Teilnehmer / Netzwerkgerät / Heimnetz / Firmennetz*;
*Vorwahl / Ortsnetz / Schrägstrich / Netzmaske*.

## Added to `DECISIONS.md`

One entry (Course text):

- Tables of operating abbreviations: the meaning column in English; a
  *(vom Englischen "Please")* that only gives the meaning back is dropped
  (PSE "Please", TNX "Thanks", VY "Very", RPRT "Report"), an origin that is
  not the meaning stays (CQ "General call (from "seek you")", SK "End of
  contact (from "Silent Key")"); plain-language renderings of a telegraphy
  QSO use English voice procedure ("DL2AB, this is DL1PZ – over!"). The same
  tables recur in the operating chapters (betriebliche_abkuerzungen).

## Judgement calls

- Throughout: *Digimode(s)* → "data mode(s)", *digitale Übertragungsverfahren* → "digital transmission methods", or "digital modes" where operating is meant (digimod_uebersteuerung, automatische_empfangsberichte, as EJ217–EJ219 and the alc section), so the two German words stay apart (glossary row); *Übertragungsverfahren* → transmission method (NE401, NE404); *Funkgerät* → radio; *WLAN* → Wi-Fi, as in earlier units.
- analog_vs_digital: *Informationsübertragung* → "transmitting information"; *keine Werte dazwischen kennt* → "has no values in between"; the slide note's etymologies "Digitus (Latin): finger", "analogos (Ancient Greek): …"; the unbalanced bracket of the German kept (see errors).
- binaer: *Zehnersystem oder Dezimalsystem* → "base-ten system or decimal system"; *binäres Zahlensystem oder Dualsystem* → "binary number system (in German also called *Dualsystem*)", and the slide bullet *Neben Binärzahl wird auch Dualzahl gesagt* kept as information about German usage (DECISIONS.md *USB* remark), since English has one word; *Dual* in the table head → "Binary"; *"Transistor gesperrt" / "Transistor leitend"* → "transistor cut off" / "transistor conducting" (§14 *gesperrter Transistor*); `\qty{64}{\text{Bits}}` → `\qty{64}{\text{bits}}` (running word inside `\text{}`); *Stellenwert $\num{1}$* → "the place value $\num{1}$"; the numbered steps as imperatives ("Write …", "Add up …").
- morsetelegrafie: *Continuous Wave (CW)* → "continuous wave (CW)"; *bevor er auf der Kurzwelle funken durfte* → "before being allowed to operate on HF" (generic *er* recast, DECISIONS.md; KW → HF); *Gegenstelle* (section and slide) → "the other station", not the glossary's IP sense *remote end*; *aufnehmen* → receive (§2, BE118); *Durchgang* → over (§2) in the special-character table; *Unterbrechung (BK)* → "Interruption (BK)", as BB109 b; " - " → en dash.
- computersteuerung: *Funkfernschreiber* (the device) → "radio teleprinter", *Funkfernschreiben* (the mode, funkfernschreiben) → radioteletype (§2, NE401); *Die Abkürzung RTTY des englischen Begriffes radio teletype* → "The abbreviation RTTY, for radio teletype" (the expansion stated plainly, as §14 *NTC / PTC*); *sogenannte CAT-Schnittstelle* → "what is known as the CAT interface"; *Rückwirkungen des Funkgeräts auf den PC* → "the radio having an effect on the PC"; *Aufzeichnen des Funkverkehrs* → "recording radio communication"; *Startsound des Betriebssystems* → "the start-up sound of their operating system"; slide note *Windows-Startsound über Funk* → "Windows start-up sound over the air".
- funkfernschreiben: *Seitlich ist … dargestellt* → "Shown alongside is …"; *im Kapitel Q-Gruppen und Locator* → "in the chapter on Q codes and the locator" (chapter titles not yet translated, descriptive as in earlier units); abbreviation tables per the new DECISIONS.md entry, *Abkz. / Bedeutung* → "Abbr. / Meaning", QSL → "I am acknowledging receipt" (ITU wording, as qsl_karten), DE → "This is" (§14 *hier ist / von*), 73 → "Best regards", *Formlose Übergabe* → informal handover (BB108); the slide fragments in English voice procedure ("this is", "over", *Zurück zu dir!* → "Back to you!", *Hier bin ich wieder* → "I am back", *Verstanden* → "Understood"); *widrige Funkbedingungen* → "poor propagation conditions" (§2 *Funkwetter*); *Grundrauschen* → noise floor (§14); the `<qso>` blocks unchanged.
- digimode_ssb: *HF-/NF-Bandbreite* → "RF / AF bandwidth" (EE403); *Rein rechnerisch* → "Purely by calculation"; caption 718's plain "2,4 kHz" → "2.4 kHz"; *Amateur Television (ATV)* → "amateur television (ATV)", *Slow-Scan Television* → "Slow-scan television" (§7); *$\qty{70}{\centi\meter}$-Band* → "$\qty{70}{\centi\meter}$ band"; photo 84 caption *Bestätigung eines SSTV Verbindung an F1BIB von ON1GA* → "Confirmation of an SSTV contact, sent to F1BIB by ON1GA".
- 9600_port: *sogenannten DATA-Anschluss* → "what is known as a DATA port"; *De-Emphasis-Prozess* → de-emphasis; *Warum eigentlich 9600 Baud?* → "So why 9600 Bd?"; the slide caption's doubled unit *$\qty{9600}{\baud}$-Baud-Datensignals* → "the $\qty{9600}{\baud}$ data signal" (see errors); *Abgreifen* → "tapped off" (NF115); caption 185 *Module M17 ein TNC* → "Module M17, a TNC"; *TNC (Terminal Node Controller)* kept as written (the expansion adds information).
- digimod_uebersteuerung: *Oberschwingungen* → harmonics (no contrast with *Harmonische* here; DECISIONS.md *Oberwelle*); *automatische Pegelregelung (englisch: Automatic Level Control, ALC)* → "automatic level control (ALC)" (bracket rule, §6); the sentences and the in-depth box shared with the alc section rendered as there (nea_sender_1), the in-depth box word for word; *Nutzsignal* → "wanted signal" (set against the unwanted components); *Nebenaussendungen* → spurious emissions (§6); *Reaktions- und Haltezeit* → "response and hold times"; *Merke:* (not italic in the German) → "Remember:".
- automatische_empfangsberichte: *Reverse-Beacon-Network* / link text *PSK-Reporter* → the services' own names "Reverse Beacon Network", "PSK Reporter" (§2 *Skimmer / Reverse Beacon Network*); „Skimmer-Stationen" → "skimmer stations" in English quotes; *Modulationsarten* → modes (§7 *Modulationsart*); *2-Wege-QSO* (slide) → "2-way QSO", keeping the digit; the slide's misspelt *Progagation* written "Propagation" (see errors); *QRP-Digimode* → "QRP data mode".
- digital_voice: *Relaisfunkstelle* → repeater (§1.3); *Richtfunkanbindung* → radio link; *sogenannten Hotspot* → "what is known as a hotspot"; *besetzte Station* → attended station, *fernbediente Station* → remotely controlled station (§14, §1.3); *TDMA (Time Division Multiple Access) oder Zeitmultiplexverfahren* → "TDMA (time-division multiple access)", slide *Time Division Multiple Access – Zeitmultiplexverfahren* → "Time-division multiple access" (bracket rule, §8); *Sprechgruppe (Talkgroup)* (slide) → "Talkgroup"; *Color-Code* → "colour code" in prose and on the slide (§8); *Teilnehmer* → another station; *M17 Open-Source Übertragungsverfahren* → "Open-source transmission method"; caption 542 ":" in the section and " - " on the slide kept apart (slide en dash).
- paketvermittelte_netzwerke: *HAMNET* / *Hamnet* each as the German writes it; *Highspeed Amateurradio Multimedia Network* kept as the network's own name; *Teilnehmer* → users; *Ortsnetze* → "local exchanges"; *Klasse A/B/C* → "Class A/B/C" (network classes, capitalised as English writes them); *keine festen Leitungen geschaltet* → "no fixed lines are switched through"; *beim Partner* → "those of the other device"; slide *Man erkennt sie daran* → "They recognise this by the fact that", as in the section; link text *Jetzt Mitglied im DARC werden!* → "Become a DARC member now!" (§14).

## Suspected errors in the German original

- sections/analog_vs_digital.md — "also auch beliebige Zwischenwerte annehmen kann [ref:n_digital_einleitung_analoges_signal])": the opening "(Abbildung" before the reference is missing, as the parallel sentence before it shows. Kept (the stray closing bracket stays).
- sections/morsetelegrafie.md and slides — "Erst in den 1990er Jahren wurde diese Regel aufgehoben" / "Seit Mitte der 1990er legen Länder fest, ob Morseprüfung notwendig ist": the RR requirement of Morse proficiency for frequencies below 30 MHz (RR 25.5) was made a national decision by WRC-03 in 2003, which is also why Germany dropped the test in 2003. Kept.
- sections/funkfernschreiben.md and slides — "SK | Ende der Verbindung (vom Englischen "Silent Key")": SK is the procedural signal for the end of work; "silent key" is the later use of the same letters for a deceased radio amateur, not the origin of SK. Kept.
- sections/digimode_ssb.md and slides — SSTV as "Übertragung von Standbildern mithilfe digitalisierte[r] Bilddaten" / "mittels Digimodes": the common SSTV modes (Martin, Scottie, Robot) send the picture as an analogue audio signal whose frequency follows the brightness; only digital SSTV (e.g. DRM-based) transmits digitised picture data. Kept.
- sections/automatische_empfangsberichte.md and slides — "WSPR steht für *Weak Signal Propagation Reporter Network*": WSPR is the Weak Signal Propagation Reporter; WSPRnet is the network. Kept.
- slides/9600_port.md — caption "FM-Sender mit Zuführung des $\qty{9600}{\baud}$-Baud-Datensignals": the unit is given twice; the English writes it once.
- Typos with no effect on the English: slides/automatische_empfangsberichte.md "Progagation"; sections/digimode_ssb.md "mithilfe digitalisierte Bilddaten", "zeigt ein Typisches SSTV-Bild", caption "eines SSTV Verbindung"; sections/9600_port.md "mit seinen begrenzten Frequenzgang", "In den Folgenden Fragen", "sollten der DATA-Port … angeschlossen werden"; slides/digimod_uebersteuerung.md "kann die ALC jedoch Problemen führen"; slides/funkfernschreiben.md note "nach Erklärungen Abkürzungen" (translated as meant: after the abbreviations have been explained); sections/paketvermittelte_netzwerke.md "über die sogenannten HAMCloud", "Die Nummern der Teilnehmern"; slides/paketvermittelte_netzwerke.md "Es zwei Möglichkeiten"; the idents `binar_stellenwert_dual` beside `binaer_…` (idents never change).
