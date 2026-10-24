# crtezi_11 — drawing translation report

29 drawings (`crtezi.json`): 951, 954, 958, 968, 969, 970, 971, 972, 973,
974, 976, 979, 980, 981, 987, 988, 991, 994, 995, 996, 997, 998, 999,
1000, 1001, 1002, 1003, 1004, 1005.
28 translated and rebuilt with `darc-drawing.py` at DARC's default 9 cm,
1 with nothing to translate. Every rebuilt drawing was compared side by
side with its original PNG: same drawing, English text, nothing
overlapping or cut off. The untouched one was rendered from its SVG: no
German printed.

## Per drawing

- 951 — the vertical "NF/BB" → "AF/BB" (§14 row *„30 St.“ / „NF/BB“ …*,
  abbreviation rule).
- 954 — decimal comma only: `\qty{0,05}` → 0.05. "MWS" and "ü = 1 : 7"
  kept (§9 *Mantelwellensperre*: the drawing keeps the German
  abbreviation; §4 *Übersetzungsverhältnis*: the symbol $ü$ stays), as 315
  in crtezi_04; λ_max with its `\text{max}` subscript unchanged.
- 958 — "N-Dotiert" / "Dünne Sperrschicht" / "P-Dotiert" → "N-doped" /
  "Thin depletion layer" / "P-doped", "Verbraucher" → "Load", "Sonnenlicht"
  → "Sunlight" (§14 row *„Schottkydiode“ … „Sonnenlicht“ / „Verbraucher“*).
  "0.5 V" was already written with a point.
- 968, 970 — "HF" / "1.ZF" / "2.ZF" / "NF" → "RF" / "1st IF" / "2nd IF" /
  "AF" (abbreviation rule, §14 *„Mischer“ / „1.ZF“* row, as 82–84 and 90).
  VFO, XO, BFO, G and 970's X, Y, Z unchanged.
- 969, 976 — "HF" / "1.ZF" / "2.ZF" / "3.ZF" → "RF" / "1st IF" / "2nd IF"
  / "3rd IF" (§14 row *„Inversionsschicht“ / „Duct“ / „3.ZF“*); 976's
  `\qty{9,455}` → 9.455. VFO, XO1, XO2, G and the frequencies unchanged.
- 971 — decimal commas only: `\qty{2,4}` → 2.4 GHz, `\qty{0,3}` → 0.3 mW.
  PC, SDR, TCXO, LNB, DC, PTT, G and the other levels unchanged.
- 972 — "NF" → "AF", the two-line "Balance-" / "modulator" → "Balanced" /
  "modulator", "Mischer" → "Mixer", "Treiber" → "Driver" (§14 row
  *„RX-Mischer“ … „Balance-modulator“*, as 914 in crtezi_10). XO, VFO, PA,
  ALC, G, "?" unchanged.
- 973, 974 — "1.\,Filter" / "2.\,Filter" → "1st filter" / "2nd filter"
  (as 85/86 in crtezi_01), "HF" → "RF", "Mischer" → "Mixer". RX, XO, f, 9f,
  f_OSZ (symbol) and the frequency ranges unchanged.
- 979, 981 — axis labels "Frequenz in MHz" → "Frequency in MHz",
  "Feldstärke in V/m" → "Field strength in V/m" (§14 row *„Feldstärke in
  V/m“ …*); the unit stays `\unit{\volt\per\metre}` and prints as a
  fraction, as in the German.
- 980 — as 979: "Frequenz in Hz" → "Frequency in Hz", "Feldstärke in kV/m"
  → "Field strength in kV/m".
- 987 — "Inversionsschicht" (twice) → "Inversion layer" (§10, §14 row);
  "Duct" unchanged.
- 988 — x-axis "Jahre" → "Years", legend "Sonnenflecken" → "Sunspots";
  "Flux" unchanged (§14 row).
- 991 — "Stunden" → "Hours", "Frequenz [MHz]" → "Frequency [MHz]"; legend
  "MUF", "LUF" unchanged. The CSV column names are not printed.
- 994, 995, 998 — "Distanz [km]" → "Distance [km]", "Höhe [km]" →
  "Height [km]" (§14 row). The legends (angles, `\qty{3.5}` … in 995) were
  already language-neutral with points.
- 996 — as 994, and the legend "Winter Nacht" / "Sommer Nacht" / "Winter
  Tag" / "Sommer Tag" → "Winter night" / "Summer night" / "Winter day" /
  "Summer day" (§14 row).
- 997 — as 994, and the legend's `\qty{3,5}` → 3.5 MHz.
- 999 — "Zeit [Stunden]" → "Time [hours]", "Frequenz [MHz]" → "Frequency
  [MHz]", legend "$f_\text{c}$ bzw. $f_\text{oF2}$" → "… or …" (§14 row
  *„fc bzw. foF2“*); the subscripts c and oF2 are symbols and stay, "MUF
  3000 km" unchanged.
- 1000 — "Kurzer Weg" / "Langer Weg" → "Short path" / "Long path" (§2, §14
  row, as 867/873 in crtezi_09). The city names (Berlin, Sydney, New York,
  Tokyo, Buenos Aires) are already the English names; the `%` comments
  stay.
- 1001 — nothing to translate: the same map centred on Sydney prints only
  the degree scale and the five city names, which read the same in
  English; no decimals.
- 1002 — "Physikalische Stromrichtung" → "Electron flow", "Technische
  Stromrichtung" → "Conventional current flow" (§3 *technische /
  physikalische Stromrichtung*, as the description already had them).
  U, e⁻, +, − unchanged.
- 1003 — "zum Netzteil" / "zum TX" → "to power supply" / "to TX" (§14 row
  for 443, the same two edge labels). V, A, PA unchanged.
- 1004 — "Reales Spannungsmessgerät" → "Real voltmeter" (§14 *reales
  Spannungsmessgerät*). R_i, I, V unchanged.
- 1005 — "Impulsdauer" → "Pulse duration" (§14 *Impulsdauer*). "3 V/Div.",
  "50 µs/Div.", "0 V", "50 %" unchanged ("Div." stays, as 38, 52, 880).

Descriptions (`N.txt`): the German brackets dropped in every translated
drawing that had them (951, 958, 968–970, 972–974, 976, 979–981, 987, 988,
991, 994–1000, 1002–1005); 995 had them unquoted. 996's axis labels were
quoted as "Distance in kilometres" ("Distanz in kilo meter") / "Height in
kilometres" ("Höhe in kilo meter"), which is not what the drawing prints;
they now read "Distance [km]" / "Height [km]", as the drawing. The other
quoted labels already matched. 954, 971 and 1001 had no German bracket and
are unchanged.

## Collisions

None. Size changes worth noting:
- 1004 — 265.8 × 127.9 → 252.1 × 120.3 pt. Not a scaling of the drawing
  by hand: DARC's own untranslated `1004.tex`, built with today's setup,
  comes out 270.4 × 130.2 pt, so the build's autoscale lands differently
  with a different label; with "Real voltmeter" the circuit comes out
  about 5 % smaller beside text of the same size (compared at equal scale;
  checked, then the translated `.tex` and its built SVG put back). Nothing
  overlaps; the
  label sits centred under the shaded box as before.
- 958 — 266.1 × 169.2 → 262.9 × 169.0 pt: "Load" is shorter than
  "Verbraucher" left of the resistor. "Thin depletion layer" fits inside
  its grey layer.
- 987 — 2.2 pt higher, 988 — 1.8 pt lower, 1002 — 1.6 pt lower (the
  bottom labels "Electron flow →" / "← Conventional current flow" each on
  their own line as before).
All other widths and heights are within 1.1 pt of the originals. In 1005
the grid lines run through "Pulse duration" exactly as they ran through
"Impulsdauer" in the German; the label sits where DARC put it.

## Glossary

No rows added: every label is already in the glossary (§2 *kurzer / langer
Weg*; §3 *technische / physikalische Stromrichtung*, *Feldstärke*; §10
*Inversionsschicht*, *Duct*; §14 *Impulsdauer*, *reales
Spannungsmessgerät*, and the drawing-label rows for *„Schottkydiode“ …
„Sonnenlicht“ / „Verbraucher“*, *„30 St.“ / „NF/BB“*, *„RX-Mischer“ …
„Balance-modulator“ / „1. Filter“*, *„Mischer“ / „1.ZF“*, *„Inversionsschicht“
/ „Duct“ / „3.ZF“*, *„Feldstärke in V/m“ … „fc bzw. foF2“*, *„Kurzer Weg“
/ „Langer Weg“*, *„zum Netzteil“ / „zum TX“*). HF/ZF/NF → RF/IF/AF follows
the abbreviation rule.

## Suspected errors

None in the German drawings.
