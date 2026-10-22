# toc_static — translation report

Not a chapter: the tables of contents, the static pages, the site snippets
and the applets. 61 files:

- `toc/`: `N.json`, `E.json`, `A.json`, `NE.json`, `EA.json`, `NEA.json`,
  `swl.json` — the `title` and `abstract` strings only (492 distinct German
  strings, 1520 occurrences), by exact string replacement; every other byte
  unchanged (checked: same structure, same line count, every value the
  intended English), and each file passes `python3 -m json.tool`.
- `contents/static/`: `infos.html`, `pruefung.html`, `pruefung_sidebar.html`,
  `suche.html`, `hamspirit.html`, `ausbilder.html` — visible text and
  `title`/`aria-label`/`placeholder` text only; the tag sequence was checked
  identical to the German. The other 25 files are empty or hold only a
  placeholder (`{{ index }}`, `%CONTENT%`).
- `contents/snippets/`: all 20 files; line structure and trailing blank
  lines/spaces as in the German; no placeholders occur.
- `contents/html/`: 28 applets — text, labels, buttons, `alt`, `title`,
  `aria-label`, chart labels and messages. Unchanged: `applet_aurora`,
  `applet_chirp_1`, `applet_chirp_2` (already English: Play/Pause/Stop; the
  rest is Morse and audio data), `applet_schwingkreis`,
  `applet_schwingkreis_antenne`, `test` (no text). Never touched: code,
  identifiers, comments (still German), URLs including CircuitJS's `lang=de`,
  the compressed CircuitJS circuits.

`revizija-guard.py --brojevi`: 54 files (snippets, static pages, applets),
*struktura netaknuta*. German-word grep: no hits in the English outside
names kept on purpose (*Deutscher Empfangsmeister*, *Deutschland-Diplom-SWL*,
*Mögel–Dellinger*, Frankfurt an der Oder, the catalogue's German title, the
data licence's name, contributor names) and code comments. Numbers in the
toc strings checked one by one against the German.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

19 rows: course names (*Gesamtkurs*, *Aufbaukurs*, *SWL-Kurs*); site buttons;
*Vorwort / Kursabschluss*; *Präsenzkurs / Patenkarte / Lehrgangskarte …*;
examination terms of the pruefung page (*Erstprüfung, Zusatzprüfung,
Lösungsbogen, Entwurfspapier …*); *mündliche Nachprüfung*;
*Nachteilsausgleich …*; examination parts; *Jedermann-Funk*; the seven Ham
Spirit virtues; section titles *Störende Beeinflussung elektronischer Geräte*,
*Verkürzungsfaktor I / II*, *Aufbau eines Empfängers / Senders,
Antennenformen*; five rows of applet labels (phasor applet, signal labels,
sampling labels, QPSK buttons, traps applet, attenuator applet).

## Added to `DECISIONS.md`

One entry (Course text): toc titles in sentence case, taking the slide
heading where one exists, and matching the titles the course text already
quotes; applets translated in their visible strings only, with the `de-DE`
number formatting in code left alone; the German bracket the course text
gives for applet controls is now obsolete (follow-up below).

## Judgement calls

- toc: *Gesamtkurs N/E/A* → "Full course N/E/A", *Aufbaukurs N -> E* → "Upgrade course N -> E" (glossary *Aufstockungskurs*), arrow kept.
- toc: same German, same English across editions; abstracts that differ only by German slips (see below) get one English text.
- toc: titles quoted in course text kept identical: "Rectifiers I" (gleichrichter_2 "Class E chapter "Rectifiers I""), "Rearranging formulas I", "Dangers of electric current", "Components and circuits".
- toc: *Verkürzungsfaktor I* → "Velocity and shortening factor I" (the section introduces both terms), *Verkürzungsfaktor II* → "Shortening factor II" (antennas only), per DECISIONS.md.
- toc: *Störende Beeinflussung elektronischer Geräte* → "Breakthrough into electronic equipment" (DECISIONS.md *Störung* vs *störende Beeinflussung*).
- toc: *Betriebsabwicklung* → "Operating procedure"; *Amateurfunkstationen* → "Amateur stations" (RR term); *Antennen und Leitungen* → "Antennas and feeders"; *Transceiver* (chapter) → "Transceivers"; *Sender / Empfänger* (chapters) → "Transmitters / Receivers".
- toc: *Fuchsjagd (ARDF)* → "Direction finding (ARDF)" (glossary: *foxhunt* only where the text quotes the colloquial word); *Physikalische Stromrichtung* → "Physical direction of current" (title, before the text introduces *electron flow*).
- toc: *Endgespeiste Antennen (End-Fed)*, *Doppelüberlagerungsempfänger (Doppelsuper)* → bracket dropped (it only repeats the term); *Überlagerungsempfänger (Einfachsuper)* keeps "(single-conversion superhet)", which adds information.
- toc: *Spannungsteiler* → "Potential divider", *Übertrager* → "Transformer", *Dynamikkompressor* → "Compressor", *Low Noise Block (LNB)* → "Low-noise block converter (LNB)", *SNR und Rauschzahl* → "SNR and noise factor" (as the slide heading), *GPS-synchronisierter Oszillator* → "GPS-synchronised oscillator" (glossary, no abbreviation in the German).
- toc swl: *Q-Gruppen* → "Q codes"; *QSL-Vermittlung* → "QSL forwarding"; award names kept German, with the English gloss in the chapter abstract (DECISIONS.md, swl_2); *Kurzwelle* → "short wave" as the swl_ionosphaere slide heading.
- toc abstracts: *Antennenanlage* → "antenna installation" (§1.3); *Bundesnetzagentur* → "Federal Network Agency (Bundesnetzagentur)"; *Amateurfunk-Peilsport* → "amateur radio direction finding"; *Sende-Empfänger (wenig gebräuchlich)* → "transmitter-receiver (rarely used)".
- snippets: *Ausbildungspaten* → "Mentors" (§14); *Selbst-Studium* → "Self-study"; *Kurse vor Ort und Online* → "Local and online courses"; *AJW-Referat* → "AJW department".
- pruefung: *Bundesnetzagentur* in full at first mention; *Anlage 1 der AFuV* → "Annex 1 to the Amateur Radio Ordinance"; *Rufzeichenplan* → "Call Sign Plan"; *Verfügung 29/2024* → "Order 29/2024"; the German-only abbreviation *(WTR)* after "scientific calculator" dropped; *&bdquo;…&ldquo;* → *&ldquo;…&rdquo;*.
- pruefung_sidebar: *Prüfungsordnung* → "Examination regulations"; *Externe Trainingsmethoden* → "External ways to practise".
- suche: *Lösungsweg* → "Solution" (§13); *Sektion* → "section"; *Treffer* → "results".
- hamspirit: the DARC's seven virtues translated faithfully in its *we* form, not replaced by Segal's English Radio Amateur's Code (which has six and different wording).
- infos: *2,8 Millionen* → "2.8 million"; *20€* → "€20"; *2,2 km* → "2.2 km"; *Jedermann-Funk* → "licence-free personal radio services"; *Relais, auch Repeater genannt* → "repeaters" (bracket rule); the generic *er* → singular *they* (DECISIONS.md); *8. und 9. Klassen* → "years 8 and 9 of German schools" (German numbering kept); *Datenlizenz Deutschland – Namensnennung – Version 2.0* and the catalogue's German title kept as names, the title with an English gloss; *MIT-Lizenz* → "MIT License" (the licence's own name).
- applets: *Zeiger* → "phasor" (iq_verfahren); *I-/Q-Anteil* → "I/Q component"; *Brummton* → "hum" (§14); *Anregung / Anregungsfrequenz* → "Not fed" / "operating frequency" (§9, §14); *Normreihe / Normwerte* → "Preferred-value series / preferred values" (§4); *Erneut übertragen* → "Transmit again", as the psk slides quote it; *Zeit-Sampling / Wert-Quantisierung* → "Time sampling / Value quantisation"; *Überlagerung* (dataset label) → "Superimposed signal"; static initial values *0,75* → "0.75", *3,5 MHz* → "3.5 MHz".

## Follow-ups outside this unit (not changed here)

- `contents/sections/sampling_quantisierung.md` ("(*Zeit-Sampling*)", "(*Wert-Quantisierung*)") and `contents/slides/psk.md` ('"Transmit again" (*Erneut übertragen*)'): by DECISIONS.md *Labels in the applets*, the German bracket goes now that the applets are English.
- `contents/sections/vorwort.md` and `contents/slides/vorwort.md` are still German and belong to no unit in `jedinice.json` (the only toc section not covered).
- Code, not translated by the brief's rule: `applet_iq_zeiger` and `applet_daempfungsglied` format numbers with `toLocaleString('de-DE')` (decimal comma in computed output); `applet_daempfungsglied` writes the symbol $a_\mathrm{erreicht}$ in its result (German subscript, like the course's formulas); the CircuitJS iframes load with `lang=de`; code comments are German.

## Suspected errors in the German original

- toc N/E/A.json, abstract of n_/e_/a_modulation — "Dabei lernen die grundlegenden Modulationsarten … kennen": *wir* missing (the NE/NEA version has it); also a double space and a stray comma before "auf eine Funkwelle".
- toc N/E.json, abstract of n_antennen_und_leitungen / e_antennen_uebertragungsleitungen — "Dabei behandeln wird": *wir*.
- toc N.json, abstract of n_bauteile_und_schaltkreise — "von jedem Funkamateure" (*Funkamateur*), "die wird in diesem Kapitel einführen werden" (*wir*).
- toc NE.json, abstract of ne_amateurfunkstationen — "unterschiedlichesten", and two commas missing compared with the N/NEA text.
- toc NE/NEA.json, abstract of ne_/nea_gesetze_und_vorschriften — "alle für Funkamateure wichtige rechtlichen Grundlagen" (*wichtigen*).
- toc N/NE/NEA.json, abstract of *_logbuch_und_qsl_karten — "senden … sogenannte QSO-Karten": they are *QSL* cards (the chapter title says so). Translated "QSO cards".
- toc swl.json — section title "CQ, DX, Contest und Split", while the section's slide heading says "CQ, DX, Contest und Pile-up". Kept as each says.
- toc — inconsistent forms of one series: "Yagi-Uda Antenne II" without the hyphen of "Yagi-Uda-Antenne" (I, III); "Gleich- und  Wechselspannung" with a double space. No effect on the English.
- static/pruefung.html — "muss ein (fach-) ärztliches Attest oder einen vergleichbaren Nachweis vorlegt werden" (*ein*, *vorgelegt*).
- static/infos.html — "entsprechendenHinweise" (space missing); "kannst Du hier … hier" (doubled *hier*); "Freude am Verstehen naturwissenschaftlich-physikalischen Zusammenhängen" (case); Class E "in einigen anderen europäischen Ländern" followed by a list that includes Australia, Canada, Israel and the USA.
- html/applet_lambda_und_f.html — the slider is labelled "Periode:" although it sets the wavelength λ, as the text above it says (copied from the sine applet). Translated "Period:".
- html/applet_rectangle.html — "Die Schalter erlauben Werte von 1 bis 500": the controls go from 1 to 499 in odd steps.
- html/maidenhead.html — "interkativen", "Reinzoomst"; html/fourier.html — "Applett". No effect on the English.
