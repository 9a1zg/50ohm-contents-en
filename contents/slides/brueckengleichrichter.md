<left>
[picture:965:a_brueckenlgeichrichter:Bridge rectifier]
</left>
<right>
* A more elaborate and common rectifier circuit
* Both half cycles are used
* Pulsating DC voltage at the output, at twice the frequency of the input voltage
</right>
--- style="font-size: smaller;"
[include:applet_gleichrichter_2]

---
[question:AD305]
---
### Smoothing
<left>
[picture:66:a_netzteil_Ucs:Rectifier circuit with smoothing]
</left>
<right>
* With reservoir capacitor $C_L$ and LC smoothing filter with $C_S$
* Smaller amplitudes of the pulsating DC voltage
* The capacitors charge up to the secondary peak voltage
</right>
<note>
</note>
---
[question:AD306]
---
#### Solution
* given: $U_P = \qty{230}{\volt}$
* given: $ü = 8:1$
* given: $U_D = \qty{0.6}{\volt}$
* required: $\hat{U}$

<fragment>
$ü = \frac{U_P}{U_S} \Rightarrow U_S = \frac{U_P}{ü} = \frac{\qty{230}{\volt}}{8} = \qty{28.75}{\volt}$
</fragment>
<fragment>
With no load, the diode voltage can be neglected.
$\hat{U} = U_S \cdot \sqrt{2} = \qty{28.75}{\volt} \cdot 1.41 \approx \qty{40}{\volt}$
</fragment>
