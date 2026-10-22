<left>
[picture:795:a_einweggleichrichtung_c:Half-wave rectification with a capacitor]
</left>
<right>
* During the positive half cycle the diode $D$ lets current flow
* Charges the capacitor $C_L$ to the peak value of the AC voltage and supplies the load resistor $R_L$
* During the negative half cycle the diode $D$ blocks
* The capacitor $C_L$ discharges through the load resistor $R_L$
</right>
---
<left>
[picture:75:a_Restwelligkeit:Ripple of the DC output voltage $U_L$]
A pulsating DC voltage $U_L$ appears across the load resistor $R_L$
</left>
<right>
* The larger the capacitance, the smoother the DC voltage
* Transformer voltages are RMS voltages
* To choose the capacitor, the peak voltage has to be worked out
* For the diode, the peak-to-peak voltage is what matters
</right>

---
[question:AD302]
---
#### Solution
* given: $U_{\mathrm{eff}} = \qty{15}{\volt}$
* required: $\hat{U}$

<fragment>
$\hat{U} = U_{\mathrm{eff}} \cdot \sqrt{2} = \qty{15}{\volt} \cdot 1.41 = \qty{21.21}{\volt}$
</fragment>
---
[question:AD303]
---
#### Solution
* given: $U_P = \qty{230}{\volt}$
* given: $ü = 20:1$
* required: $\hat{U} + \qty{50}{\percent}$

<fragment>
$ü = \frac{U_P}{U_S} \Rightarrow U_S = \frac{U_P}{ü} = \frac{\qty{230}{\volt}}{20} = \qty{11.5}{\volt}$
</fragment>
<fragment>
$\hat{U} = U_S \cdot \sqrt{2} = \qty{11.5}{\volt} \cdot 1.41 \approx \qty{16.26}{\volt}$
</fragment>
<fragment>
$\hat{U} + \qty{50}{\percent} \approx \qty{25}{\volt}$
</fragment>
---
[question:AD304]
---
#### Solution
* given: $U_P = \qty{230}{\volt}$
* given: $ü = 5:1$
* required: $U_{SS} + \qty{20}{\percent}$

<fragment>
$ü = \frac{U_P}{U_S} \Rightarrow U_S = \frac{U_P}{ü} = \frac{\qty{230}{\volt}}{5} = \qty{46}{\volt}$
</fragment>
<fragment>
$\hat{U} = U_S \cdot \sqrt{2} = \qty{46}{\volt} \cdot 1.41 \approx \qty{65.05}{\volt}$
</fragment>
<fragment>
$U_{SS} + \qty{20}{\percent} = 2 \cdot \hat{U} + \qty{20}{\percent} \approx \qty{156}{\volt}$
</fragment>