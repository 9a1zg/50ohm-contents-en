# swl_pitanja — translation report

DARC's SWL question set, `contents/questions/fragenkatalog_swl.json`: the 11
questions SWL001–SWL011 and the file's 5 section titles. Batch
`swl_pitanja.json`, applied with
`qbank-prevedi.py --file contents/questions/fragenkatalog_swl.json`
(new option, `50ohm` commit e6af24b): 23 fields, 5 titles, 0 refused, 0
warnings. The file keeps its own formatting (LF, UTF-8 characters, final
newline), which differs from fragenkatalog3b.json (CRLF, `\u` escapes); the
tool now reproduces either byte for byte. `metadata` (edition date, source)
is left in German, as in fragenkatalog3b.json.

## How

- SWL004–SWL011, "Welchem Amateurfunkband entspricht der Frequenzbereich von
  …?" → "Which amateur band corresponds to the frequency range …?", decimal
  points in `\qtyrange`; the answers are band names in `\qty` and need no
  change (24 fields identical to the German).
- SWL001–SWL003 are the DARC's versions of VE201–VE203 with "a person" /
  "an amateur station" for "a radio amateur". Where the German is the same,
  the English is the bank's: all answers of SWL002 and SWL003 (VE202, VE203;
  the German *Sie darf* / *Er darf* makes no difference to the impersonal
  English) and SWL001 a. SWL001 b, c, d follow VE201 b, c, d with the
  German's subjects: "The operator of an amateur station counts as a
  competent person …", "… requires a special authorisation from the BNetzA",
  "Anyone is entitled to do so if technically approved receivers are used."
- Titles: the four shared with fragenkatalog3b.json as there (glossary §15);
  the TDDDG's formal title *Gesetz über den Datenschutz und den Schutz der
  Privatsphäre in der Telekommunikation und bei digitalen Diensten (TDDDG)*
  → "Act on Data Protection and the Protection of Privacy in
  Telecommunications and Digital Services (TDDDG)": a long formal title
  takes the abbreviation only (DECISIONS.md, batch 10). New glossary row
  (§1.2). The course text (swl_abhoerverbot) names the law by its short
  title, "Telecommunications Digital Services Data Protection Act".
- The prose around `[question:SWL…]` (swl_frequenzbereiche,
  swl_abhoerverbot, sections and slides) fits the English wording.

## Suspected errors in the German original

- The TDDDG section title has a double space before "(TDDDG)". Not carried
  into the English.
