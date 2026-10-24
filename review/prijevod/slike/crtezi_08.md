# crtezi_08 — drawing translation report

29 drawings (`crtezi.json`): 745, 748, 749, 751, 758, 759, 762, 766, 767,
768, 769, 772, 773, 778, 779, 780, 781, 782, 783, 784, 786, 790, 793, 803,
807, 808, 809, 810, 828.
20 translated and rebuilt with `darc-drawing.py` at DARC's default 9 cm,
9 with nothing to translate. Every rebuilt drawing was compared side by side
with its original PNG: same drawing, English text, nothing overlapping or
cut off. The untouched ones were rendered from their SVGs: no German
printed.

## Per drawing

- 745 — `\qty{145,9}` → 145.9, "DVB-T2 Kanal 35" → "DVB-T2 channel 35"
  (§14 row 742/745/748). "TV", "f = 582–590 MHz" unchanged.
- 748 — "9 V Block" → "9 V block" (same row). "LR41 1.5 V", "AA 1.5 V",
  "AAA 1.5 V", "G" unchanged (already `\qty{1.5}`). The photo
  `contents/photos/168.png` is in the repository, so the build needed no
  extra step; see "748 and the PNG" for how it was looked at.
- 749 — "HF\\(KW)" → "HF", "VHF\\(UKW)" → "VHF": the German everyday name
  only repeats the English one and goes (§14 row *„HF (KW)“ / „VHF (UKW)“*);
  "LW", "MF" and the band table unchanged. The band frequencies now print
  with a decimal point (British siunitx setup), as DECISIONS.md expects.
- 751 — "Isotroper / Strahler" → "Isotropic / radiator" (§9
  *isotroper Strahler*, §14 row 751), line break kept.
- 758 — decimal commas only: `\qty{4,7}` → 4.7, `\qty{13,8}` → 13.8.
  R_V, I_Z, R_L, I_L, "0 V" unchanged.
- 759, 762 — "Pufferstufe" → "Buffer stage" (§5). f_OSZ (symbol), R_1, C_1
  unchanged.
- 766, 767 — decimal commas only: `\qty{2,7}`, `\qty{0,1}` (twice),
  `\qty{2,2}`, `\qty{0,2}` (twice), `\qty{0,56}` → points. C_1–C_6, T_2,
  "R=180 Ω", "+13 V" unchanged.
- 768, 769 — nothing to translate: "X" labels and "+" only.
- 772 — `\qty{3,7}` → 3.7, "Ausgang" → "Output" (§5 *Eingang / Ausgang*,
  as 740). "f_o = 3.7 MHz" was already written with a point in the `.tex`
  and printed a comma under the old setup; it now prints a point.
- 773 — nothing to translate: already prints "RF_IN" / "RF_OUT" (§14 row
  *HF_IN*); "MMIC", R_BIAS, U_CC, U_D, pin numbers.
- 778, 779, 780, 781 — nothing to translate: "X", "+", C_1, C_2 only.
- 782, 783, 784 — "Eingangs- / anpassung" → "Input / matching",
  "Ausgangs- / anpassung" → "Output / matching" (§14 *Eingangsanpassung /
  Ausgangsanpassung*; the English is two words, so the hyphen goes and the
  break stays), `$\mathrm{HF}_\mathrm{IN}$` / `$\mathrm{HF}_\mathrm{OUT}$` →
  `$\mathrm{RF}_\mathrm{IN}$` / `$\mathrm{RF}_\mathrm{OUT}$` (§14 row
  *„HF_IN“ / „HF_OUT“*, as NF_IN → AF_IN in 488). U_BIAS, ϑ, R_1, R_2, R_4,
  "X", "1", "2", "+5 V", "+50 V" unchanged.
- 786 — `\qty{6,2}` → 6.2, `\qty{6,8}` → 6.8, HF_IN / HF_OUT → RF_IN /
  RF_OUT (as 782). U_BIAS, U_DD, U_Z, K_1, K_2, T_1 (4:1), T_2 (1:9) and the
  other values unchanged.
- 790 — "Periode" → "Period" (§3, as 728). "Amplitude", "t", "0", "+", "−"
  unchanged.
- 793 — nothing to translate: seven-segment digits, "MHz", "100M … 1",
  "10^8 … 10^0".
- 803 — amplifier labels "HF" / "ZF" / "NF" → "RF" / "IF" / "AF" (German
  abbreviations become English). "VFO", "BFO" unchanged.
- 807 — "f_e1 und f_e2" → "f_e1 and f_e2", "Mischer" → "Mixer" (§14 row
  *„Mischer“ …*, as 80). f_o, f_ZF (symbols) unchanged.
- 808 — "Filtert f_e2 raus" → "Filters out f_e2", "Mischer" → "Mixer" (same
  row). "f_e1/f_e2", f_e1, f_o, f_ZF unchanged.
- 809 — nothing to translate: a world map drawn as one SVG path, no text.
- 810 — "HF" → "RF", "1.ZF" / "2.ZF" → "1st IF" / "2nd IF", "NF" → "AF",
  "1. Mischer" / "2. Mischer" → "1st mixer" / "2nd mixer", "Produktdetektor"
  → "Product detector" (§14 row *„Mischer“ / „1. Mischer“ …*, wording as in
  82–84). "AGC", "G" unchanged; the commented-out X/Y/Z labels stay.
- 828 — titles "Eingangssignal" / "Verstärkung" / "Ausgangssignal" →
  "Input signal" / "Amplification" / "Output signal", "Begrenzung" →
  "Limiting" (§14 row 828). "Amplitude", "t" unchanged. The axis option
  `use comma` (in `xticklabel style`) is a style setting with no tick label
  printed (`xticklabels={}`), so it stays.

Descriptions (`N.txt`): the German brackets dropped in 745, 748, 749, 751,
759, 762, 772, 782–784, 786, 790, 803, 807, 808, 810 and 828. In 749
`"HF" ("HF (KW)")` / `"VHF" ("VHF (UKW)")` become `"HF"` / `"VHF"`, as the
drawing now prints them. The quoted labels match the drawings (labels set on
two lines quoted as one, as before: "Isotropic radiator", "Input matching",
"Output matching"; 808 keeps its own way of writing the symbols, "fe1/fe2",
"Filters out fe2", as it does for all of them). 758, 766, 767 had no German
brackets (their values were already given with a point) and are unchanged,
as are the nine drawings with nothing to translate.

## Collisions

None. Everything fits without a change:
- 810 — "Product detector" (anchored south west over the product detector)
  is wider than "Produktdetektor": the drawing is 2.8 pt wider
  (256.1 → 258.9 pt); it ends inside the drawing and clears "AGC" and "2nd
  mixer".
- 782–784 — "Input matching" / "Output matching" sit inside their blocks,
  as the German did.
- 749 — without "(KW)" / "(UKW)" the left label column is narrower, the
  drawing 0.9 pt narrower and 7.6 pt taller (954.5 → 962.1 pt), the axis
  being scaled to the width; labels unchanged in place.

All other widths and heights are within 1.5 pt of the originals.

## 748 and the PNG

`darc-drawing.py` built 748 ("ok", 260.7 × 261.1 → 260.6 × 261.0 pt) but
could not write its PNGs: the SVG embeds the photo and is 13 MB, and
`rsvg-convert` refused it ("XML parse error … Huge input lookup"). The new
and the old SVG (`git show HEAD:…`) were rendered by hand with
`rsvg-convert -u` (allow huge files) and compared: same photo, same labels,
only "Block" → "block" and the decimal points. A checker rendering 748 needs
the same `-u`.

## Glossary

No new rows: every label is already in the glossary (§3 *Periode*; §5
*Pufferstufe*, *Eingang / Ausgang*; §9 *isotroper Strahler*; §14
*Eingangsanpassung / Ausgangsanpassung* and the drawing-label rows for
742/745/748, 749/829, 751/759/762/782–784, *„HF_IN“ / „HF_OUT“*,
*„Mischer“ / „1. Mischer“ …*, 828). HF/ZF/NF → RF/IF/AF follows the
abbreviation rule in TRANSLATION.md.

## Suspected errors

In the German drawings: none noticed.

In DARC's German alt text (left as translated; not in slike_07's list):
- 786.txt — "über einen 100-pF-Kondensator C_2": the drawing labels C_2
  "100 nF"; and "über einen 470-nF-Kondensator C_5": the 470 nF capacitor
  is labelled C_3 (there is no C_5 in `786.tex`). Translated as written
  ("100 pF capacitor C_2", "470 nF capacitor C_5").
- 793.txt — the display is said to read "433.075000" / "4 3 3 . 0 7 5 0 0
  0" (ten digits, although the text says nine): `793.tex` sets nine digits
  4 3 3 1 7 5 0 0 0, with the point after the third, and the render reads
  433.175000. Translated as written.
- 749.txt — the 17 m band is given as "18.068 MHz–18.186 MHz"
  (German „18,068 MHz–18,186 MHz“); `749.tex` and the drawing say 18.168.
  Translated as written.
