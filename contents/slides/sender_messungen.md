## Measurements for radio amateurs

* Important measurements: output power and RF voltages
* Measuring the transmitter output power requires a defined termination
* Usual impedance in amateur radio: $\qty{50}{\ohm}$
* Measuring directly in the circuit only makes sense at low power

---
## Measuring RF voltage

* RF voltage is measured with an RF probe
* Diode rectification and smoothing with a capacitor after the diode

---
### RF probe with simple rectification



<left>
[picture:576:a_messung_hf_tastkopf_leistungsmessung:Measuring head for RF power measurement via a potential divider]
</left>
<right>
* A diode at the output delivers the peak voltage of the RF voltage
* Minus the forward voltage of the diode and any potential divider
</right>

---
[question:AI608]

---
### RF probe with double rectification

<left>
[picture:770:a_messung_hf_tastkopf_doppeldiode:RF probe with two diodes for both half cycles]
</left>
<right>
* Two diodes to increase the measuring accuracy, especially at low power
* Both half cycles are rectified
* Result: twice the peak voltage minus twice the forward voltage of the diodes
</right>

---
[question:AI605]

---
[question:AI604]

---
### Measuring high RF power

* Requires an attenuator with a suitable power rating
* Absorbs most of the power
* The attenuator must be included in the calculation

---
[question:AI609]

<note>
No calculation needed, since only one answer has an attenuator
</note>

---
## Calibrating measuring circuits

* Necessary for exact power measurements
* Correction values must be produced

---
[question:AI612]

---
### Calculating an RF probe

<left>
[picture:576:a_messung_messschaltung_beispiel_1:Example of an RF measuring circuit]
</left>
<right>
* Input signal is terminated with the correct impedance
* Voltage is halved by the potential divider
* After rectification by the diode, the peak voltage minus the forward voltage remains
</right>

---
[question:AI610]

--- style="font-size: smaller;"
#### Solution

* given: $P_E = \qty{1}{\watt}$
* given: $U_F = \qty{0.23}{\volt}$
* given: $R_V = \qty{110}{\ohm}$, $R_T = \qty{330}{\ohm}$
* required: $U_A$


<fragment>
$\begin{split}R &= \left(\frac{1}{R_T + R_T} + \frac{1}{R_V} + \frac{1}{R_V}\right)^{-1}\\ &= \left(\frac{1}{\qty{330}{\ohm} + \qty{330}{\ohm}} + \frac{1}{\qty{110}{\ohm}} + \frac{1}{\qty{110}{\ohm}}\right)^{-1}\\ &= \qty{50.77}{\ohm}\end{split}$
</fragment>

--- style="font-size: smaller;"
* given: $P_E = \qty{1}{\watt}$
* given: $U_F = \qty{0.23}{\volt}$
* calculated: $R = \qty{50.77}{\ohm}$
* required: $U_A$

<fragment>
$\begin{split}P_E &= \frac{U_{E,eff}^2}{R}\\ \Rightarrow U_{E,eff} &= \sqrt{P_E \cdot R}\\ &= \sqrt{\qty{1}{\watt} \cdot \qty{50.77}{\ohm}}\\ &= \qty{7.125}{\volt}\end{split}$
</fragment>

--- style="font-size: smaller;"
* given: $U_F = \qty{0.23}{\volt}$
* calculated: $U_{E,eff} = \qty{7.125}{\volt}$
* required: $U_A$

<left>
<fragment>
$\begin{split}U_S &= U_{E,eff} \cdot \sqrt{2}\\ &= \qty{7.071}{\volt} \cdot 1.414\\ &= \qty{10.07}{\volt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_A &= \frac{U_S}{2}\,-\,U_F\\ &= \frac{\qty{10.07}{\volt}}{2}\,-\,\qty{0.23}{\volt}\\ &= \qty{5.035}{\volt}\,-\,\qty{0.23}{\volt}\\ &= \qty{4.805}{\volt} \approx \qty{4.8}{\volt}\end{split}$
</fragment>
</right>

---
### Calculating the input power from the DC voltage measured

<left>
[picture:577:a_messung_messschaltung_beispiel_2:Example of an RF measuring circuit]
</left>
<right>
* Voltage at the potential divider equals the output voltage plus the diode voltage
* Calculate RMS values
* Find the input power from the circuit resistance
</right>

---
[question:AI611]

--- style="font-size: smaller;"
#### Solution
* given: $U_A = \qty{14.9}{\volt}\text{ DC}$
* given: $U_F = \qty{0.7}{\volt}$
* given: $R_1 = \qty{54.1}{\ohm}$, $R_T = \qty{330}{\ohm}$
* required: $P_E$

<left>
<fragment>
$\begin{split}R &= \left(\frac{1}{R_T + R_T} + \frac{1}{R_1}\right)^{-1}\\ &= \left(\frac{1}{\qty{330}{\ohm} + \qty{330}{\ohm}} + \frac{1}{\qty{54.1}{\ohm}}\right)^{-1}\\ &= \qty{50}{\ohm}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_S &= \left(U_A + U_F\right) \cdot 2\\ &= \left(\qty{14.9}{\volt} + \qty{0.7}{\volt}\right) \cdot 2\\ &= \qty{31.2}{\volt}\end{split}$
</fragment>
</right>

--- style="font-size: smaller;"
<left>
* calculated: $R = \qty{50}{\ohm}$
* calculated: $U_S = \qty{31.2}{\volt}$
* required: $P_E$

<fragment>
$\begin{split}U_{E,eff}\\ &= \frac{U_S}{\sqrt{2}}\\ &= \frac{\qty{31.2}{\volt}}{1.414}\\ &= \qty{22.06}{\volt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}P_E &= \frac{U_{E,eff}^2}{R}\\ &= \frac{(\qty{22.06}{\volt})^2}{\qty{50}{\ohm}}\\ &\approx \qty{9.7}{\watt}\end{split}$
</fragment>
</right>

---
### RF probe with double peak rectification

<left>
[picture:771:a_messung_hf_tastkopf_doppeldiode_2:RF probe with double peak rectification]
</left>
<right>
* Calculation as with simple rectification
* Also take into account the doubled peak voltage
* Note the double forward voltage of the diodes
</right>

---
[question:AI607]

--- style="font-size: smaller;"
#### Solution

* given: $U_A = \qty{15.3}{\volt}\text{ DC}$
* given: $U_F = \qty{0.23}{\volt}$
* given: $R_{V1} = \qty{56}{\ohm}$, $R_{V2} = \qty{470}{\ohm}$
* required: $P_E$

<left>
<fragment>
$\begin{split}R &= \left(\frac{1}{R_{V1}} + \frac{1}{R_{V2}}\right)^{-1}\\ &= \left(\frac{1}{\qty{56}{\ohm}} + \frac{1}{\qty{470}{\ohm}}\right)^{-1}\\ &= \qty{50.04}{\ohm}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_S &= \frac{U_A}{2} + U_F\\ &= \frac{\qty{15.3}{\volt}}{2} + \qty{0.23}{\volt}\\ &= \qty{7.88}{\volt}\end{split}$
</fragment>
</right>

--- style="font-size: smaller;"
<left>
* calculated: $R = \qty{50.04}{\ohm}$
* calculated: $U_S = \qty{7.88}{\volt}$
* required: $P_E$

<fragment>
$\begin{split}U_{E,eff} &= \frac{U_S}{\sqrt{2}}\\ &= \frac{\qty{7.88}{\volt}}{1.414}\\ &= \qty{5.57}{\volt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}P_E &= \frac{U_{E,eff}^2}{R}\\ &= \frac{{\qty{5.57}{\volt}}^2}{\qty{50.04}{\ohm}}\\ &\approx \qty{600}{\milli\watt}\end{split}$
</fragment>
</right>

---
[question:AI606]

--- style="font-size: smaller;"
#### Solution

* given: $U_A = \qty{15.3}{\volt}\text{ DC}$
* given: $U_F = \qty{0.23}{\volt}$
* given: $R = \qty{50}{\ohm}$ from the measuring system
* required: $P_E$

<left>
<fragment>
$\begin{split}U_S &= \frac{U_A}{2} + U_F\\ &= \frac{\qty{15.3}{\volt}}{2} + \qty{0.23}{\volt}\\ &= \qty{7.88}{\volt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_{E,eff} &= \frac{U_S}{\sqrt{2}}\\ &= \frac{\qty{7.88}{\volt}}{1.414}\\ &= \qty{5.57}{\volt}\end{split}$
</fragment>
</right>
  
--- style="font-size: smaller;"
* calculated: $U_{E,eff} = \qty{5.57}{\volt}$
* given: $R = \qty{50}{\ohm}$ from the measuring system
* required: $P_E$

<fragment>
$\begin{split}P_E &= \frac{(U_{E,eff} \cdot 10)^2}{R}\\ &= \frac{(\qty{5.57}{\volt} \cdot 10)^2}{\qty{50}{\ohm}}\\ &\approx \qty{60}{\watt}\end{split}$
</fragment>

--- style="font-size: smaller;"
## Field-strength meter for power measurement

<left>
[picture:496:a_messung_feldstaerkeanzeiger:Field-strength meter]
</left>
<right>
* Measuring the RF power via an antenna
* Received RF is rectified and stored
* Reading on a sensitive ammeter
* The greater the needle deflection, the higher the RF field strength
* Exact measurements require calibration
</right>

---
[question:AI613]
