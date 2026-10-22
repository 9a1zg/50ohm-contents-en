# nea_betriebsabwicklung — translation report

Chapter "Betriebsabwicklung" (Operating procedures): 6 sections, each with
its slides, no solutions. 12 files:

- `contents/sections/` and `contents/slides/`: `pileup.md`,
  `split_betrieb.md`, `contest.md`, `ardf.md`, `sstv.md`, `notfunk.md`.

`revizija-guard.py --brojevi`: 12 files checked, *struktura netaknuta*.
German-word grep: no hits outside the intended German (the `% TODO`
comments in notfunk, *Fuchsjagd*, *Notfunkreferat*, *Strafgesetzbuch*,
*Amateurfunkverordnung*, "Notfall", "CQ Ruhrgebietscontest"). Line counts,
the trailing space after the sprint-contest paragraph (sections/contest.md),
the whitespace-only lines in sections/ardf.md and sections/notfunk.md, the
double space after "SOS"*. in sections/notfunk.md, the indented `</note>`
and `###  ` in slides/notfunk.md, and the missing final newline of
slides/split_betrieb.md, contest.md and ardf.md are as in the German.

Embedded questions looked up in English and the prose aligned with them:
BE305–BE311, BE301–BE304, BE116, BE313, BD109, BE210, BF101–BF109, VD105
(BE305 "pile-up", "sought-after station"; BE306 "only number 3", "the digit
3 between prefix and suffix"; BE307 "list operation"; BE308 "split
operation"; BE309 "on varying frequencies within the range given"; BE310
"listening 5 kHz above its own transmit frequency"; BE301 "for competing";
BE302 "as many contacts as possible in the given time"; BE303 "contest
rules", "so that the contact counts"; BE304 "sprint contest", "leaves the
frequency to the other station"; BE116 "Field Day contest"; BE313
"foxhunt", "direction-finding receivers"; BF104 "listen carefully and note
down all important information"; BF105 "do not disrupt the radio traffic";
BF106 "the police or the emergency control centre"; BF107 "remain reachable
and pass on information until help has arrived"; BF108 CEST; BF101
"distress signals outside amateur radio"; VD105 "distress, urgency and
safety signals", "expressly prohibited"; BF109 "kept clear").

## Added to `TRANSLATION_GLOSSARY.md` (§14)

9 rows: *Aufruf nach Ziffern / nach Ländern oder Kontinenten /
Kontaktwünsche*; *fortlaufende Nummer / Alter / Rangliste / Punktabzug*;
*Fuchsjagdsender / Zielpunkt / Wimpel / Zeitnehmer*; the RSV V-scale
values; *Leitstation (Notfunk)*; *Notfunkreferat des DARC*;
*Notfunkfrequenzen*; *"Notfall" oder "Emergency"*; *Amateurfunkmedien*.

Changed: the §14 row *5 W-Fragen* "the five Ws (who, what, where, when,
why)" → "the 5 Ws", with a note that the course's five are *Where / Who /
What / How many / Wait* (the journalists' list it gave did not match the
text, and the digit is kept as the German writes it). No translated text
used the old row.

## Added to `DECISIONS.md`

None.

## Judgement calls

- pileup: *"only number 5" (nur Ziffer 5)* → '"*only number* 5" (the digit 5 only)': the German bracket only translates the English, but in English it still says what BE306 says — that *number* means the digit between prefix and suffix — and it keeps the number.
- pileup: wordorigin *"sich aufstapeln" oder "sich türmen"* → "to stack up or to heap up" (the German glosses rendered as English meanings, not dropped, since they explain the verb); *was sich hier aufstapelt oder türmt* → "What piles up or heaps up here".
- pileup: *Kurzwelle* → HF; *sogenannte* → "what is known as"; *Aufruf nach Ziffern / Ländern oder Kontinenten* → "Calling by digit / by country or continent"; *Kontaktwünsche* → "requests for contacts".
- split_betrieb: *Split-Verkehr* and *Split-Betrieb* both → "split operation" (glossary, BE308); *Abstand zur Sendefrequenz* → "offset from the transmit frequency"; *Die Angaben erfolgen immer in kHz* → "The figures are always given in kHz"; *auf gut Glück* → "at random".
- contest: *Betriebsabwicklung* → "operating procedures" (glossary; BE301 says "operating technique" for its own German wording); *Ausschreibung* → "contest rules" (glossary, BE303), which makes *Regeln, die der Veranstalter in einer Ausschreibung festlegt* "rules, which the organiser lays down in the *contest rules*"; *kommt man nur mit einer Portabelstation in die Wertung* → "you are only scored if you operate a portable station"; generic *sein Ruf* → "the call" (DECISIONS.md, generic *er*); *Versuch* → "trial"; *das Alter* → "the operator's age".
- contest slides: "CQ Ruhrgebietscontest" kept — it is a call as transmitted (call strings are not translated); *In Telegrafie dann CQ TEST* → "In telegraphy, accordingly, CQ TEST".
- ardf: *im deutschsprachigen Raum meist als Fuchsjagd bezeichnet* → 'in German-speaking countries are mostly called *Fuchsjagd* ("foxhunt")' — the sentence is about the German name (DECISIONS.md, remarks about German usage kept), and BE313 gives the English "foxhunt"; elsewhere *Fuchsjagd* → "foxhunt" (informal course text, glossary), *Mobilfuchsjagd* → "mobile direction finding" (glossary); *Bundesnetzagentur* written out at first mention, "Federal Network Agency (Bundesnetzagentur, BNetzA)"; generic *er* recast ("The winner is the first to reach the finish after finding all the foxes").
- ardf: caption *mit Wimpel und Zeitnehmer* → "with pennant and timing unit" (the photo shows the fox's equipment, so the electronic timing unit rather than a person keeping time).
- sstv: *Großes Call lesbar* → "Large call sign readable"; the last V value "rauschfreies Bild" capitalised like the other items and like the slides' table.
- notfunk: *Leitstation* → "net control station"; *Notruf* → "distress call", *Notmeldung* → "distress message" (glossary, BF104–BF107); *Mayday* → MAYDAY (glossary §13); *Station des Flug- oder Seefunkdienstes* → "a station of the aeronautical or maritime mobile service" (glossary), on the slides *See- und Flugfunk* → "maritime and aeronautical radio" (informal names).
- notfunk: § 323c StGB → "Section 323c of the Criminal Code (Strafgesetzbuch, StGB)" (glossary §1), section and slides; the quoted provision translated faithfully (no official English text), with singular "them" for *ihm*.
- notfunk: *5 W-Fragen* → "the *5 Ws*"; the five items translated faithfully, so the fourth reads "*How* many people are affected?" — the German acronym of W-words cannot be kept in English without changing what is asked.
- notfunk: "Notfall" kept as the German on-air word, glossed "(German for "emergency")", beside "Emergency" (DECISIONS.md, German phrases quoted as German usage), section and slides.
- notfunk: *Notfunkreferat des DARC* → "DARC emergency communications department (Notfunkreferat)", as the *Auslandsreferat*; *Notfallkommunikation* → "emergency communications"; *MESZ / MEZ* → CEST / CET (glossary, BF108); *Internationale Beteiligung* → "International involvement".
- notfunk: *im $\qty{80}{\meter}$-Band* → "in the $\qty{80}{\meter}$ band" (glossary: band names without hyphen).

## Suspected errors in the German original

- sections/contest.md vs slides/contest.md — the section says calls in a contest *always* (*immer*) contain "Contest" or, in telegraphy, "Test"; the slides say *often* (*Oft*) and give "CQ FD" and "CQ Ruhrgebietscontest" as examples, which contain neither.
- sections/ardf.md, slides/ardf.md — "Gewonnen hat der Erste, der den Zielpunkt erreicht, nachdem er alle Füchse gefunden hat": in ARDF the competitors start at staggered times and are ranked by the number of foxes found and the time taken, so the first to arrive is not necessarily the winner. Imprecise rather than wrong for a course text. Kept.
- Typos with no effect on the English: sections/split_betrieb.md "Häufiger wird eine begehrte Station aber nicht nur eine einzelne Frequenz angegeben" (*gibt … an*); sections/pileup.md "Informationen über interessante Station" and slides/pileup.md "Hinweise über seltene Station" (*Stationen*), "findet man  Rufzeichen" (double space); slides/split_betrieb.md "am Meisten" (*meisten*); sections/contest.md "aus einem speziellen Land oder Region" (*einer*); slides/contest.md "der Namen des Wettbewerbes" (*Name*), "zum testen" (*Testen*); slides/ardf.md "im zeitlichem Wechsel" (*zeitlichen*), "ein anderes der folgende Rufzeichen" (*folgenden*); sections/sstv.md "5 = rauschfreies Bild" (lower case); sections/notfunk.md "eine Station … an Bord eines Schiffs oder Flugzeugs mit, dass es sich in Not befindet" (*sie*).
