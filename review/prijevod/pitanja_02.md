# pitanja_02 — translation report

175 questions (AB5, AB6, NB7, EC1, NC1, AC1, EC2, NC2, AC2, EC3, NC3, AC3,
EC4, AC4, EC5, NC4, AC5, EC6, NC5, AC6, AD1), 779 fields. `qbank-prevedi.py`:
0 refused, 0 warnings.

## Added to `TRANSLATION_GLOSSARY.md`

- §3: *Gleichstromwiderstand / ohmscher Widerstand* → DC / ohmic resistance;
  *Wechselstromwiderstand* → impedance, or AC resistance where contrasted with
  DC resistance; *induktiver Widerstand* → inductive reactance;
  *Gegeninduktion* → mutual induction; *Stromdichte* → current density;
  *eingeschwungener Zustand* → steady state; *(Gleich)stromverstärkung* →
  (DC) current gain.
- §4: *Hochlast- / Präzisionswiderstand*; *induktionsarm* → low-inductance;
  *gewendelt / ungewendelt* → spiral-cut / without a spiral cut;
  *Kennzeichnung* → marking; *Styroflexkondensator* → polystyrene (Styroflex)
  capacitor; *Plattenabstand / -fläche*; *Dielektrizitätszahl / -konstante* →
  relative permittivity / permittivity; *Kondensator- / Spulengüte* → Q;
  *Wickellänge*; *Abschirmbecher* → screening can; *Eigeninduktivität* →
  self-inductance; *Schwellspannung* → threshold voltage; *Varicap*;
  *Freilaufdiode* → freewheeling diode; *Fotodiode / Optokoppler*;
  *n-/p-dotiert*; *Power-MOS-FET / Dual-Gate-MOS-FET*; *Halbleitersubstrat*;
  *vergossene Schaltung* → potted circuit.
- §5: *Brückenzweig* → bridge diagonal; *Basisspannungsteiler* → base
  potential divider; *Emitterwiderstand*; *Strom- / Spannungsgegenkopplung* →
  negative current / voltage feedback; *Stabilisierungsschaltung* → stabiliser
  circuit; *Spannungserhöhung* → voltage step-up; *Transformationsverhältnis*.
- §13: *Lötstelle* → solder joint; *Leuchtanzeige* → indicator light;
  *Stromgewinnung* → electricity generation; *Heizwendel* → heating coil.

## Judgement calls

- *Ohm* as a word → *ohm/ohms*, *kOhm/MOhm* → *kΩ/MΩ*, as in pitanja_01; so
  EC117/EC115 mix "22 kΩ" and "223 ohms" across their answers. `\mOhm` and
  `\milliOhm` (AC523, EC521) left as the German's macros.
- *ca.* → "Approx." / "approx." (capitalised when the answer stands alone);
  *etwa* → "About" (EC401).
- AB601 / NB702: *physikalische / technische Stromrichtung* → "direction of
  electron flow (the physical direction of current)" / "direction of
  conventional current flow", per the glossary.
- NB701: *Masse* / *Erde* → "Chassis" / "Earth", per the glossary trap.
- EC202, EC303: *Wechselstromwiderstand* of an ideal C / L → "impedance";
  AC203 keeps "AC resistance" against "DC resistance". AC203 c/d keep the
  German's deliberately wrong "ohmic resistance $X_L$".
- AC103: German lists *Blindwiderstand / Metalloxidwiderstand /
  Wirkwiderstand / NTC-Widerstand* as "resistances"; English stem "Which of
  the following resistances…" with "The reactance", "The metal-oxide
  resistor", "The resistance (resistive part)", "The NTC thermistor".
- AC209: stem's closing clause recast ("The losses in an inductor are also
  expressed by …") so the answers complete it.
- AC201: German "…eilt der Strom der angelegten Spannung …" → stem ends at
  "the current …", answers "lags/leads the applied voltage by …".
- EC607, EC606: German stem has no "…" and the article ("einen") in the stem;
  English stem "This component is …" with the article in each answer
  (a PNP / an NPN …).
- EC106/EC107: *ungewendelt / gewendelt* → "without a spiral cut" /
  "spiral-cut" (helically trimmed film resistors).
- EC113: *zwischen … bis …* → "between … and …"; EC503 likewise, all four
  answers made "between X and Y V for germanium, and between … for silicon".
- AC517/AC518: *Querwiderstand* → "bleeder resistor" (glossary §14),
  *Vorwiderstand R1* → "series resistor".
- AC522, AC521: the German stems end their value lists with "..."; kept.
- EC615–EC612: *Massepotential* → "chassis potential" (glossary).
- Suspected slips in the German, translated normally: AC306 "Windungverhältnis"
  (missing s); EC103, EC104 stems end with "." instead of "?" ("?" in English);
  AD114 stem has no final "?" (added); AC516 d lacks a final full stop (added
  for parallelism); EC105 d has a full stop the others lack (dropped); EC611
  "fliesst"; NC109/NC108 answers start with a stray space (dropped).

## Provjera

175 questions checked (all five fields, German from `upstream/main` side by
side with the English); 32 fields changed in 19 questions: 21 unit style,
2 glossary, 9 wording / style. No meaning errors, no answer whose correctness
changed. Applied from `pitanja_02.provjera.json` with `--retranslate`:
0 refused, 0 warnings.

- EC117 b/d, EC115 b/d, EC112 a/b, AC107 a/b/d, AC105 a/b/d, AC104 a/c/d,
  AC204 a/b/d, EC521 a/c/d: "ohms" → "Ω" where the same answer set also has
  kΩ (or `\milliOhm`), so each set is written one way. Sets that are all
  plain ohms (EC116, EC113, AC106, AD110 …) keep "ohms".
- AC517, AC518: *Querwiderstand* "bleeder resistor" → "lower divider
  resistor"; a bleeder resistor is the PSU discharge resistor (and the
  glossary already gives it for *Ableitwiderstand*). Glossary §14 corrected
  (and *Querstrom* → divider current added).
- AC515, AC517, AC518: "Calculate the series resistor $R_1$" → "Calculate the
  value of the series resistor $R_1$".
- NC103: "which three colour bands does a 1.2 kΩ resistor have at the start?"
  → "What are the first three colour bands on a 1.2 kΩ resistor …?"
- AC201: "an ideal inductance" → "an ideal inductor" (the component).
- AC407 c, EC517 c: "Varactor" → "Varactor diode", parallel with the other
  diode answers and with AC404.
- EC516: "is operated from an operating voltage" → "is supplied with an
  operating voltage".
- EC522: "The following circuit of a stabiliser with a Zener diode" → "The
  following Zener diode stabiliser circuit".
- AC521: "in the circuit drawn" → "in the circuit shown".
- AC604 b: "constant from as low as 0 Hz" → "constant from 0 Hz upwards".

Left as the translator chose, after checking: "Approx." for *ca.* (lower case
where it continues a stem, EC522) and "About" for *etwa* (EC401) — each set
is consistent; AC209's recast stem ("are also expressed by …") and AC201's
stem ending at "the current …" read correctly with every answer; EC606/EC607
"This component is …" with the article in each answer; AC103's "resistances"
covering both quantities and components, as the German *Widerstände* does;
"chassis potential" (EC612–EC615) per the glossary.
