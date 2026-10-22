### Transformer principle

<left>
[photo:239:e_Trafo mit getrennten Wicklungen:Transformer with visibly separate windings]
</left>
<right>
* Magnetically coupled coils
* Changing current in one coil
* Produces a voltage in the other coil
* $\rightarrow$ mutual induction
</right>

---
[question:AC301]
--- style="font-size: 0.7em;"
The turns ratio, primary to secondary, is equal to the voltage ratio, primary to secondary, but to the current ratio, secondary to primary:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S} = \frac{I_S}{I_P}$

<fragment>
The ratio of the primary to the secondary impedance is the square of the ratios above:

$ü^2 = \frac{Z_P}{Z_S} = \left(\frac{N_P}{N_S}\right)^2 = \left(\frac{U_P}{U_S}\right)^2 = \left(\frac{I_S}{I_P}\right)^2$
</fragment>

<fragment>
Or, after taking the square root:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S} = \frac{I_S}{I_P} = \sqrt{\frac{Z_P}{Z_S}}$
</fragment>

<note>
The last formula appears in this form on the formula sheet
</note>
---
[question:AC302]
---
#### Solution
* given: $U_P = \qty{230}{\volt}$
* given: $U_S = \qty{6}{\volt}$
* given: $I_S = \qty{1.15}{\ampere}$
* required: $I_P$

<fragment>
$\begin{split} \frac{U_P}{U_S} &= \frac{I_S}{I_P} \\ \Rightarrow I_P &= \frac{I_S \cdot U_S}{U_P} = \frac{\qty{1.15}{\ampere} \cdot \qty{6}{\volt}}{\qty{230}{\volt}} \\ &= \qty{30}{\milli\ampere} \end{split}$
</fragment>

---
## Impedance matching

<left>
[picture:260:a_impedanzanpassung:Matching $\qty{2450}{\ohm}$ to $\qty{50}{\ohm}$ with a transformer with a turns ratio of 1 to 7]
</left>
<right>
[photo:332:a_unun:Example of an unun transformer with a turns ratio of 2 to 14, with the primary and secondary wound together bifilar (twisted)]
</right>

---
[question:AC306]
---
#### Solution
* given: $Z_P = \qty{50}{\ohm}$
* given: $Z_S = \qty{2.5}{\kilo\ohm}$
* required: $ü$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} = \sqrt{\frac{\qty{50}{\ohm}}{\qty{2.5}{\kilo\ohm}}} \\ &= \sqrt{\frac{1}{50}} \approx \frac{1}{7} \end{split}$
</fragment>

---
[question:AC303]
---
#### Solution
* given: $Z_S = \qty{16}{\kilo\ohm}$
* given: $ü = \frac{1}{4}$
* required: $Z_P$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} \\ \Rightarrow Z_P &= ü^2 \cdot Z_S = \frac{1^2}{4^2} \cdot \qty{16}{\kilo\ohm} \\ &= \frac{\qty{16}{\kilo\ohm}}{16} = \qty{1}{\kilo\ohm} \end{split}$
</fragment>

---
[question:AC304]
---
#### Solution
* given: $Z_S = \qty{6.4}{\kilo\ohm}$
* given: $ü = \frac{1}{4}$
* required: $Z_P$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} \\ \Rightarrow Z_P &= ü^2 \cdot Z_S = \frac{1^2}{4^2} \cdot \qty{6.4}{\kilo\ohm} \\ &= \frac{\qty{6.4}{\kilo\ohm}}{16} = \qty{0.4}{\kilo\ohm} \end{split}$
</fragment>

---
[question:AC305]
---
#### Solution
* given: $Z_P = \qty{450}{\ohm}$
* given: $Z_S = \qty{50}{\ohm}$
* required: $ü$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} = \sqrt{\frac{\qty{450}{\ohm}}{\qty{50}{\ohm}}} \\ &= \sqrt{\frac{9}{1}} = \frac{3}{1} \end{split}$
</fragment>


---
### Maximum current
<left>
* The wire must not get too warm
* Otherwise the insulation melts
* Or the conductor glows
* $\rightarrow$ permissible current density: current relative to the cross-sectional area of the conductor
</left>
<right>
<fragment>
[photo:236:e_HF Übertrager:RF transformer (balun) that can melt if too much power is applied]
</fragment>
</right>
<note>
Melted home-made baluns in plastic cases are not uncommon when "just a bit more power" is applied
</note>

---
### Examples of permissible current density

according to the VDE

* Copper conductors installed in free air: $\frac{\qty{12}{\ampere}}{\qty{0.75}{\milli\meter\squared}}$
* Fuses: up to $\qty{3000}{\ampere\per\milli\meter\squared}$
* Transformers: $\qty{2.5}{\ampere\per\milli\meter\squared}$ (windings radiate heat poorly)

---
[question:AC307]
---
#### Solution
* given: $d = \qty{0.5}{\milli\meter}$
* given: current density $\frac{I}{A} = \frac{\qty{2.5}{\ampere}}{\qty{1}{\milli\meter\squared}}$
* required: $I_{\mathrm{max}}$

<fragment>
$A_{Dr} = \frac{d^2 \cdot \pi}{4} = \frac{(\qty{0.5}{\milli\meter})^2 \cdot \pi}{4} \approx \qty{0.196}{\milli\meter\squared}$
</fragment>
<fragment>
$I_{\mathrm{max}} = \frac{I}{A} \cdot A_{Dr} = \frac{\qty{2.5}{\ampere}}{\qty{1}{\milli\meter\squared}} \cdot \qty{0.196}{\milli\meter\squared} = \qty{0.49}{\ampere}$
</fragment>
