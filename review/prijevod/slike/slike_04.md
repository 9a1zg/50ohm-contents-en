# slike_04 — translation report

107 files in `contents/drawings/` (34–47, 324–478 as listed in
`serije.json`).

## Files translated (106)

- With a description (106): 34, 35, 36, 38, 39, 40, 41, 43, 44, 45, 46, 47,
  324, 326, 341–345, 354–362, 364–370, 374–378, 381, 383–393, 395–403,
  408–411, 420–440, 442, 443, 445–452, 457, 458, 470, 471, 473–478. Of these,
  56 carry DARC's marker, translated.

## Files left as they are (1)

- `TODO` only (1): 328.

`alttext-check.py`: 107 files, 0 with findings. Line counts are the same as
in the German (256 lines changed, 256 replaced); no file of the batch ends
in a newline, in German or English.

## Added to `TRANSLATION_GLOSSARY.md` (§14)

7 rows: the labels „Durchlassbereich“ / „Sperrbereich“ / „Zeit“ / „Wert“;
the DDS labels of 438; the labels of the interference filters 434–437; the
labels of 439, 430 and 45; *Relais-Spule / Schließerkontakt / Schalterzunge
/ Polpunkt / Kopplungsstrich*; *Versorgungsschiene / Schiene / Leiterbahn*;
*Skala / Teilstrich / dachförmig / Bus-Markierung*.

## Judgement calls

- Section labels as glossary §14; 410's *Kurz: / Details:* → "Short: /
  Details:" (as 300 in slike_03), 447's *Kurz: / Detail:* → "Short: /
  Detail:". Numbering `1)`, `1.` (434) or none kept per file, and so are the
  label lines of 443 and the bullet list of 428.
- Labels that are German words: English, then the German in brackets, the
  bracket not repeated when the same paragraph names the label again (as
  slike_01): "Attenuator" ("Dämpfungsglied"), "Passband"
  ("Durchlassbereich"), "Time" ("Zeit"), "to power supply" ("zum Netzteil"),
  "Output" ("Ausgang"), "AF" ("NF"), "RF" ("HF"), "IF" ("ZF") … Labels that
  read the same in English get no bracket: "Amplitude", "Modulator",
  "Demodulator", "Register", "Bits".
- 436: the three-line label is quoted with its slashes, as the German does:
  "Electrical length: / 1/2 of the wavelength / of the interfering
  frequency".
- Decimal point in labels and values: "0.6 V", "2.2 kΩ", "9.0015 MHz",
  "0.3 – 3.4 kHz", "1.5 V", "0.3" / "2.7", "0.3 mW -5 dBm", "2.4 GHz", 8.7,
  0.5; the meter scales "1, 1.5, 2, 3" were already printed with a point.
  *50 Ohm* (341, 424) → "50 Ω"; 46's "1A" → "1 A", "0,6V" → "0.6 V".
- 470: "TXCO" kept as written: `470.tex` prints TXCO (the usual
  abbreviation is TCXO).
- *Spule* → "inductor"; *Spule (Induktivität)* (399, 434, 435, 447, 448) →
  "coil (inductor)", as 1016 in slike_01. *Spulen/Wicklungen* (370) →
  "inductors/windings".
- *Baugruppen* in block diagrams → "modules", as slike_02/03;
  *Übertragungskurve* (401, 402) → "response curve" (§5); *Kennlinie* (400)
  → "characteristic"; *Flanken* (38) → "slopes" (§14).
- *Masse* → "chassis"; *Erdungssymbol (Massezeichen)* (434) → "earth symbol
  (chassis symbol)", *Massezeichen (Erdungssymbol)* (437) the other way
  round, *Masse-/Erdungssymbol* (448) → "chassis/earth symbol".
- *Leiterbahn* in a drawn circuit (442, 447) → "conductor track" (§14
  *Leiterbahnen* → PCB tracks would claim a board the drawing does not
  show).
- *Analoginstrument* → "analogue meter", *Zeiger* → "needle",
  *Teilstriche* → "tick marks"; the German's English word *Labels* (420–422)
  → "labels".
- 471: the unquoted labels *Röntgenstrahlung, Radar und Funkwellen* →
  "X-rays, radar and radio waves", without brackets, as the German does not
  quote them.
- 367, 370: the primes in „L1’“, „N’“ kept as printed; 368/369 write "L1'"
  with an apostrophe, also kept. 370's "L1◯" marks unchanged.
- 367: the German's English word *unlabeled* → "unlabelled" (as 1038).
- 35: *horiontalen* → "horizontal"; 431 *simd* → "are"; 44 *varaibler* →
  "variable" (typos, translated as meant).
- 374, 375, 432: the label "Ausführliche  Beschreibung" (two spaces) →
  "Detailed description"; the double spaces in 433 and 451 and the soft
  hyphen in 445's "Verbindungs­punkt" not reproduced.
- 47: the short description has no closing full stop; none added.

## Suspected errors in the German descriptions

- 386 — "Die Wellenlänge ist in Abschnitten von T, 2T und 3T markiert": T
  on a time axis is the period, not the wavelength. Translated as written.
- 429 — calls the rectangle with a diagonal line a *Sicherungssymbol* and
  the dashed links run "an Sicherung und Transistor"; `429.tex` draws a
  relay coil (`genericshape` with a diagonal, dashed link to the switch),
  which 428 correctly calls *Relais-Spule*. Translated as written ("fuse").
- 46 — describes "30 Kondensatoren" in parallel; `46.tex` draws `battery1`
  cells (0.6 V each, solar cells for TB201), not capacitors. Translated as
  written.
- 427 — "zwei Rechtecke mit diagonalen Linien, die Transistoren darstellen
  können": `427.tex` has one rectangle with a diagonal (a relay coil) and a
  transistor in a circle. "Rechte Kreise" is unclear (perhaps *Runde* or
  *Rechts*); translated literally "Right-hand circles".
- 35 — the short description lists "einem Siebkondensator … und einem
  Transformator" after "ein elektronischer Schalter" (case slip); harmless.
- 477 — "einem dachförmigen Bereichen" (case slip); harmless.
- 367 — "unlabeled" is an English word in the German text (as 1038).

## Provjera

Checked all 107 files against the German at `793aa5f~1`, sentence by
sentence: 106 full descriptions (56 with DARC's marker) and 1 `TODO` (328),
left as it is. 10 files changed, 11 lines. `alttext-check.py --rev
793aa5f~1`: 107 files, 0 with findings.

- 364, 365 — *Stromquelle* (the + / − supply of the drawing; `364.tex`
  draws only the terminals) "current source" → "power source", as §14
  *Stromquelle (wie eine Batterie)*; *current source* is the circuit element.
- 41 — *auf der Markierung 29 (außen) bzw. nahe 8,7 (innen)* "or" → "and",
  as the detailed description: the needle reads both at once; *für jeweils
  1 Einheit* / *0,5 Einheiten* "for every 1 unit" → "at intervals of 1 unit"
  / "0.5 units" (natural English).
- 420, 421, 422 — *Ganz innen* "Right on the inside" → "Innermost" (natural
  English).
- 400 — *Koordinatenursprung* "The origin of the coordinates" → "The
  origin" (the English term).
- 409 — *Auf der Grafik* "In the graphic" → "On the graph" (natural
  English).
- 443 — *auf dieser Senkrechten* "on this vertical" → "on this vertical
  line" (the noun needs its head in English).
- 35 — *mit „230 V“ und einer Wellenlinie beschriftet* "labelled "230 V"
  and with a wavy line" → "carry the label "230 V" and a wavy line"
  (grammar).

Left as translated: "Shown is …" for *Gezeigt ist …* (as slike_02/03),
*Masse* → "chassis" and *Spule (Induktivität)* → "coil (inductor)" as the
judgement calls above, "Short: / Detail(s):" in 410 and 447, TXCO in 470,
the second bracket in 402's "(labelled "Passband" ("Durchlassbereich"))"
(glossary §14, as slike_02), and the suspected German errors listed above
(386, 429, 46, 427), which are reported, not fixed.
