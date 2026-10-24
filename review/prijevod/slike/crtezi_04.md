# crtezi_04 — drawing translation report

29 drawings (`crtezi.json`): 311, 315, 326, 341, 342, 354, 355, 378, 385,
400, 401, 402, 403, 408, 409, 410, 411, 420, 421, 422, 423, 424, 430, 434,
435, 436, 437, 438, 439.
23 translated and rebuilt with `darc-drawing.py` (width 9 cm), 6 with
nothing to translate. Every rebuilt drawing was compared side by side with
its original PNG: same drawing, English text, nothing overlapping or cut
off. The six untouched ones were rendered from their SVGs: no German
printed.

## Per drawing

- 311 — "$l$ = 43{,}18 m für 7,1 MHz" → "$l$ = 43.18 m for 7.1 MHz" (§14
  drawing-label row).
- 315 — decimal comma only: `\qty{0,05}` → `\qty{0.05}`. "MWS" kept (§9,
  the drawing keeps the German abbreviation); "ü = 1 : 7" kept (the symbol
  $ü$ stays, §4 *Übersetzungsverhältnis*).
- 326 — nothing to translate (no printed text; the `%` comments only).
- 341, 342, 423, 424 — "Dämpfungsglied" → "Attenuator" (§5); $R_\mathrm{i}$,
  $R_\mathrm{L}$, $P_\mathrm{IN}$, $P_\mathrm{OUT}$, "a", "b" kept.
- 354 — "NF" → "AF", "HF" → "RF" (§14 row for „ZF“/„NF“); "Modulator",
  "FM", "VFO", "G" and the numbers 1–4 unchanged ("Modulator" is the
  English word as well).
- 355 — "HF" → "RF", "ZF" → "IF", "NF" → "AF"; "Demodulator" unchanged (as
  354).
- 378, 385 — nothing to translate ($R_1$ … $R_4$ only).
- 400, 401, 402, 403 — "Durchlass-\\bereich" → "Passband" (one line; the
  hyphenated break was only needed for the long German word),
  "Sperrbereich" → "Stopband" (§14 row, slike_04).
- 408, 409, 410, 411 — axis labels "Zeit" → "Time", "Wert" → "Value".
- 420, 421, 422 — nothing to translate: S, PWR, SWR, ALC, "+60 dB" and the
  scale numbers; the SWR scale's "1.5" is already written with a point in
  the source. The German `%` comments stay.
- 430 — "Kontroll-\\information" → "Control\\information",
  "Weitere\\Teile\\des\\Empfängers" → "Further\\parts\\of the\\receiver"
  (§14 row; same number of lines).
- 434, 435 — "Auf das / Störsignal / abgestimmt" → "Tuned to the /
  interfering / signal" (§14 row; the three lines rewrapped so the middle
  line, beside the arrow, stays about as long as "Störsignal").
- 436, 437 — "Elektrische Länge: / 1/2 (1/4) der Wellenlänge / der
  Störfrequenz" → "Electrical length: / 1/2 (1/4) of the wavelength / of the
  interfering frequency" (§14 row; line breaks as in the German and as the
  description quotes them).
- 438 — "Taktgenerator" → "Clock generator", "Adresszähler" → "Address
  counter", "Sinus-Tabelle" → "Sine table", "D/A Umsetzer" → "D/A
  converter"; "Register", "N", "Bits", $f_\mathrm{out}$ unchanged.
- 439 — "Kabel 1/2" → "Cable 1/2", "Dämpfung" → "attenuation", "6 dB
  Verstärkung" → "6 dB gain", "Antenne" → "Antenna", "Gewinn" → "gain";
  "TX", "PA" unchanged (§14 row, lower case as there).

Descriptions (`N.txt`): the German brackets dropped in 311, 342, 354, 355,
400–403, 408–411, 423, 430, 434–439. The quoted labels already matched the
drawings word for word (436's three-line quote with its slashes matches the
line breaks); no other change. 315, 341 and 424 had no German brackets and
are unchanged.

## Collisions

None. The longer English labels stay clear of everything:
- 436, 437 — "of the interfering frequency" is the widest line and reaches
  further right than "der Störfrequenz", but ends left of the chassis wire
  and below the stub; the drawing gets a little wider (246.6 → 248.4 pt) and
  is therefore slightly smaller at 9 cm.
- 438 — the vertical labels "Clock generator" and "Address counter" are
  longer than the German ones; the drawing gets taller (101.9 → 113.4 pt),
  nothing touches.
- 430 — the four-line "Further / parts / of the / receiver" makes the
  drawing a little taller (155.7 → 163.7 pt).
- 341, 342, 423, 424 — about 2 pt lower ("Attenuator" has no descender).

## Glossary

No new rows: every label is already in the glossary (§5 *Dämpfungsglied*;
§14 the drawing-label rows for „ZF“/„NF“, „l = 43,18 m für 7,1 MHz“,
„Durchlassbereich“/„Sperrbereich“/„Zeit“/„Wert“, 438, 434–437, 439/430).

## Suspected errors

In the German drawings:
- 342.tex, 424.tex — the generator is labelled $R_\mathrm{L}$ 50 Ω, the
  same symbol as the load resistor on the right; in 341 and 423 (the same
  attenuator setting) the generator's internal resistance is
  $R_\mathrm{i}$. Probably a slip for $R_\mathrm{i}$; kept as in the German.

In DARC's German alt text (left as translated):
- 424.txt — calls the generator "a variable resistor R_L of 50 Ω"; the
  drawing shows a sine-wave source (labelled R_L, see above).
- 342.txt — "On the right is a further circle, also labelled R_L"; the
  right-hand R_L is a resistor (rectangle), not a circle.
