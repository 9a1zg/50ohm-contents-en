* Input voltage can vary
* For example in battery-powered equipment
* Sensitive circuits (e.g. oscillators) would change their frequency
* Remedy: voltage stabilisation

---
## Stabilisation with a Zener diode
<left>
[picture:323:a_Stabilisierung mit Z-Diode:Voltage stabilisation with a Zener diode]
</left>
<right>
* Very simple circuit
* Can keep the output voltage stable within limits
</right>
<note>
</note>
---
[question:AD321]
--- style="font-size: 0.7em;"
#### Solution
* given: $R_L = \qty{470}{\ohm}$
* given: $I_L = \qty{10}{\milli\ampere}$
* given: $I_Z = \qty{15}{\milli\ampere}$
* given: $U_{\mathrm{in}} = \qty{13.8}{\volt}$
* required: $\eta = \frac{P_L}{P_{\mathrm{in}}}$

<fragment>
$P_L = I_L^2 \cdot R_L = (\qty{10}{\milli\ampere})^2 \cdot \qty{470}{\ohm} = \qty{47}{\milli\watt}$
</fragment>
<fragment>
$P_{\mathrm{in}} = U_{\mathrm{in}} \cdot I_{\mathrm{in}} = U_{\mathrm{in}} \cdot (I_Z + I_L) = \qty{13.8}{\volt} \cdot (\qty{15}{\milli\ampere} + \qty{10}{\milli\ampere}) = \qty{345}{\milli\watt}$
</fragment>
<fragment>
$\eta = \frac{P_L}{P_{\mathrm{in}}} = \frac{\qty{47}{\milli\watt}}{\qty{345}{\milli\watt}} \approx \num{0.14}$
</fragment>
---
## Linear voltage regulator

<left>
[picture:985:a_spannungsregler_linear:Circuit diagram of a linear voltage regulator]
</left>
<right>
* Power transistor is operated as a variable resistor
* Forms a potential divider together with the load resistance
* Efficiency is often very low
</right>

---
[question:AD315]
---
[question:AD319]
---
#### Solution
* given: $U_{\mathrm{in}} = \qty{13.8}{\volt}$
* given: $U_{\mathrm{out}} = \qty{9}{\volt}$
* given: $I = \qty{900}{\milli\ampere}$
* required: $P_V$

<fragment>
$U_{IC1} = U_{\mathrm{in}} - U_{\mathrm{out}} = \qty{13.8}{\volt} - \qty{9}{\volt} = \qty{4.8}{\volt}$
</fragment>
<fragment>
$P_V = U_{IC1} \cdot I = \qty{4.8}{\volt} \cdot \qty{900}{\milli\ampere} = \qty{4.32}{\watt}$
</fragment>
---
[question:AD320]
---
#### Solution
* given: $U_{\mathrm{in}} = \qty{13.8}{\volt}$
* given: $U_{\mathrm{out}} = \qty{5}{\volt}$
* given: $I_{\mathrm{in}} = \qty{455}{\milli\ampere}$
* given: $I_{\mathrm{out}} = \qty{450}{\milli\ampere}$
* required: $\eta$

<fragment>
$\eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}} = \frac{U_{\mathrm{out}} \cdot I_{\mathrm{out}}}{U_{\mathrm{in}} \cdot I_{\mathrm{in}}} = \frac{\qty{5}{\volt} \cdot \qty{450}{\milli\ampere}}{\qty{13.8}{\volt} \cdot \qty{455}{\milli\ampere}} \approx \num{0.36}$
</fragment>
---
## Fixed voltage regulator
<left>
[picture:200:a_Festspannungsregler:Fixed voltage regulator]
</left>
<right>
* Implemented as an IC
* Work like linear voltage regulators, with a very accurate voltage reference and optimised electronic control
* Even when the input side fluctuates strongly, the output side is very stable
</right>

---
[question:AD317]
---
[question:AD316]
---
[question:AD318]
---
#### Solution
* given: $U_{\mathrm{in}} = \qty{13.8}{\volt}$
* given: $U_{\mathrm{out}} = \qty{5}{\volt}$
* given: $R_L = \qty{10}{\ohm}$
* required: $P_V$

<fragment>
$I = \frac{U_{\mathrm{in}}}{R_L} = \frac{\qty{5}{\volt}}{\qty{10}{\ohm}} = \qty{500}{\milli\ampere}$
</fragment>
<fragment>
$U_{IC1} = U_{\mathrm{in}} - U_{\mathrm{out}} = \qty{13.8}{\volt} - \qty{5}{\volt} = \qty{8.8}{\volt}$
</fragment>
<fragment>
$P_V = U_{IC1} \cdot I = \qty{8.8}{\volt} \cdot \qty{500}{\milli\ampere} = \qty{4.4}{\watt}$
</fragment>
