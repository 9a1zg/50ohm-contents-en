# 50ohm.de content — English translation (work in progress)

This is a fork of DARC's [`50ohm-contents-dl`](https://github.com/DARC-e-V/50ohm-contents-dl),
the content of the German amateur-radio training platform [50ohm.de](https://50ohm.de),
being translated into **British English** by 9A1ZG. It is a faithful
translation for DARC — the licence classes N, E and A, the Bundesnetzagentur
and German law stay as they are — not an adaptation for another country.

**Status (2026-10-23):**

- **Exam questions** (`contents/questions/fragenkatalog3b.json`): all 1750
  questions and the catalogue section titles translated, each batch checked by
  a second pass, plus a consistency pass over the whole bank. Not yet reviewed
  by DARC.
- **SWL questions** (`contents/questions/fragenkatalog_swl.json`, DARC's
  question set for the DE examination): all 11 questions and the section
  titles translated and checked.
- **Course text** (sections, slides, worked solutions): all 41 units and the
  foreword translated, each checked by a second pass.
- **Static pages** (tables of contents, static pages, snippets, the applets'
  visible text): translated and checked.
- **Picture descriptions** (`contents/drawings/*.txt`, `contents/photos/*.txt`)
  **and the drawings' own labels:** not yet done; drawings still carry German
  labels.

How it is done, and every decision taken, is documented in
[`TRANSLATION.md`](TRANSLATION.md), [`DECISIONS.md`](DECISIONS.md) and
[`TRANSLATION_GLOSSARY.md`](TRANSLATION_GLOSSARY.md); per-batch notes, including
suspected errors in the German original, are in `review/prijevod/`.

**Licences and attribution.** The content is licensed under
[CC BY 4.0](LICENSE) and the exam questions under the
[Datenlizenz Deutschland – Namensnennung – 2.0](https://www.govdata.de/dl-de/by-2-0),
exactly as in the original, whose notice follows unchanged below.
*Changes made:* translated from German into English. Attribution: the
50ohm.de author team, coordinated by the AJW-Referat of DARC e. V. (see the
contributor list below); exam questions: Bundesnetzagentur, Prüfungsfragen zum
Erwerb von Amateurfunkprüfungsbescheinigungen, 3rd edition, March 2024.
English translation: 9A1ZG.

---

*Original notice (German):*

# Inhalte 50ohm.de

Dieses Repository enthält die Inhalte der Plattform 50ohm.de. Der Plattform-Code findet sich in einem gesonderten [Repository](https://github.com/DARC-e-V/50ohm). Die Lernplattform ist ein Angebot des AJW-Referats des DARC (Deutscher Amateur-Radio-Club e. V.). Viele ehrenamtlichen Mitarbeiterinnen und Mitarbeiter sind daran beteiligt.

# Lizenz und Pull-Requests

Die Inhalte stehen unter der [CC BY 4.0 Lizenz](LICENSE). Um zu diesem Repository beizutragen, musst du die entsprechenden Hinweise in unserer Datei [CONTRIBUTING](CONTRIBUTING.md) beachten.

## Hinweis zur Namensnennung (CC BY)

Bei jeder Verwendung der Materialien dieses Repositorys müssen angemessene Urheber- und Rechteangaben gemacht werden. Zudem ist anzugeben, ob Änderungen an den Materialien vorgenommen wurden. Details finden sich in der [CC BY 4.0 Lizenz](LICENSE).

Diese Angaben dürfen in jeder angemessenen Art und Weise erfolgen, jedoch nicht so, dass der Eindruck entsteht, der Lizenzgeber unterstütze oder befürworte die jeweilige Nutzung in besonderer Weise.

Bitte nenne als Urheber (Mitwirkendenliste):

> 50ohm.de–Autorenteam, koordiniert durch das AJW-Referat des DARC e. V.
> 
> Matthias Amberg (DG4MA), Henrik Bartels (DL6OCH), Jan Behrens (DL9JBE), Helmut Berka (DL2MAJ), Mathias Dahlke (DJ9MD), Michael Danowski (DK6QW), Christian Dasch (DO1CMD), Sabrina Deharde (DO7XK), Lucas Ebersberger (DA1EE), Dennis Eisold (DN9KGB), Klaus Finkenzeller (DL5MCC), Christoph Fischer (DC6GF), Michael Funke (DL4EAX), Tim Grelka (DA2TG), Michael Groni (DB7YI), Prof. Dr. Michael Hartje (DK5HH), Christian Hillmer (DM7EE), Ronny Jerke (DG2RON), Prof. Dr. Matthias Jung (DL9MJ), Thomas Kamp (DF5JL), Erich Kless (DD4UQ), Karlheinz Krause (DL4DBY), Stephan Kregel (DG1HXJ), Dr. Andreas Krüger (DJ3EI), Michael Lowack (DK1KC), Rüdiger Maaß (DF7LYN), Ralf Mahler (DF1RM), Karsten Merker (DH1KM), Daniel Mittendorf (DK5WP), Michael Moller (DG9NDT), Felix Pfannkuch (DF3LX), Christian Reiber (DL8MDW), Harald Rode (DL4HR), Florian Schmid (DL1FLO), Prof. Dr. Herrmann Schumacher (DF2DR), Alexander Schumacher (DL1ASN), Marco Schwan (DC8WAN), Prof. Dr. Klaus Solbach (DK3BA), Caspar Heinrich Nicolas Spethmann, Björn Swierczek (DL1PZ), Aaron Thielmann (DB9TT), Carmen Weber (DM4EAX), Lars Weiler (DC4LW), Daniel Wendt-Fröhlich (DL2AB), Severin Wiedemann (DL9SW), Emile Hansmaennel

## Prüfungsfragen

Die Prüfungsfragen in `contents/questions/fragenkatalog3b.json` sind dem amtlichen Fragenkatalog entnommen: Prüfungsfragen zum Erwerb von Amateurfunkprüfungsbescheinigungen, Bundesnetzagentur, 3. Auflage, März 2024, (www.bundesnetzagentur.de/amateurfunk), [Datenlizenz Deutschland – Namensnennung – Version 2.0](https://www.govdata.de/dl-de/by-2-0)

`contents/questions/fragenkatalog_swl.json` enthält die zusätzlichen Fragen aus dem DARC-Fragenkatalog für die DE-Prüfung, die keine Entsprechung im amtlichen Fragenkatalog der Bundesnetzagentur haben.

Am Fragenkatalog, welcher in Kooperation mit der Bundesnetzagentur entstand, waren und sind folgende Personen von Seiten des DARC e. V. beteiligt:

> Fabian Amann (DC1SAF), Matthias Amberg (DG4MA), Henrik Bartels (DL6OCH), Jan Behrens (DL9JBE), Michael Berger (DF7SA), Helmut Berka (DL2MAJ), Dr.-Ing. Hartmut Büttig (DL1VDL), Mathias Dahlke (DJ9MD), Michael Danowski (DK6QW), Sabrina Deharde (DO7XK), Hendrik Dietrich (DG3HDA), Marcus Engelmann (DL2DCX), Klaus Finkenzeller (DL5MCC), Christian Frieß (DL2MDU), Michael Funke (DL4EAX), Michael Gebhardt (DM1CHL), Lukas Greiner (KN6PSU), Michael Groni (DB7YI), Prof. Dr.-Ing. Michael Hartje (DK5HH), Gerrit Herzig (DH8GHH), Thomas Hillen (DF2TH), Christian Hillmer (DM7EE), Martin Jerabek (DK1MJ), Ronny Jerke (DG2RON), Prof. Dr.-Ing. Matthias Jung (DL9MJ), Klaus Jung (DL5KJ), Thomas Kamp (DF5JL), Erich Kless (DD4UQ), Peter Kornherr (DK4KP), Karlheinz Krause (DL4DBY), Stephan Kregel (DG1HXJ), Dr. Andreas Krüger (DJ3EI), Martin Kuhn (DL3SFB), Stefan Lampprecht (DL1SL), Manfred Lauterborn (DK2PZ), Markus Lör (DO2MLS), Michael Lowack (DK1KC), Jürgen Lutz (DK3OL), Hannes Matuschek (DM3MAT), Günther Mildenberger (DL4BX), Daniel Mittendorf (DK5WP), Michael Moller (DG9NDT), Roy Muselick (DM4ET), Andreas Nützel (DG4MIC), Ralph Oppelt (DL2NDO), Dr.-Ing. Henning Paul (DC4HP), Marei Peischl, Peter Pfann (DL2NBU), Christian Reiber (DL8MDW), LL.B. Lukas Reinhardt (DO7VLR), Harald Rode (DL4HR), Uwe Rüdiger (DG2DBF), Paul Schimanski (DF4ZL), Florian Schmid (DL1FLO), Werner Schmidt (DL4YBZ), Malte Schmitz (DE7LMS), Stefan Scholl (DC9ST), Alexander Schumacher (DL1ASN), Marco Schwan (DC8WAN), Björn Swierczek (DL1PZ), Aaron Thielmann (DB9TT), Jann Traschewski (DG8NGN), Alexander Vidoni (DK6AV), Werner Vollmer (DF8XO), Carmen Weber (DM4EAX), Michael Weber (DL1XMW), Lars Weiler (DC4LW), Wolfgang Welter (DL2KBJ), Daniel Wendt-Fröhlich (DL2AB), Severin Wiedemann (DL9SW), Udo Witte (DJ4FV), Dipl.-Ing. Claus-Dieter Wittek (DF8QJ), Bernhard Zimmermann (DG3BZ)

# Kontakt

Verantwortlich für das Betreiben von 50ohm.de ist das AJW-Referat des DARC e. V. in Baunatal, Deutschland. Für Anfragen bitte die Email-Adresse [50ohm@darc.de](mailto:50ohm@darc.de) nutzen. Weiterhin findet man viele der Beitragenden im Matrix-Kanal [50ohm Contribution](https://matrix.to/#/#50ohm-contribution:darc.de).
