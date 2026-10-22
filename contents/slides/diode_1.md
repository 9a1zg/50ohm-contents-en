## Application

<left>
* A diode lets current flow in one direction only
* In the other direction it acts like a high resistance
* Diodes are used, among other things, to rectify AC voltage
</left>
<right>
[picture:689:e_led:Various LEDs in different package styles and colours]
</right>
<note>
* We have already met one special type of diode: the LED
</note>

---
[question:EC501]
---
[question:EC502]
---

## Threshold voltage

<left>
* For a diode to conduct in the forward direction, a certain voltage – the threshold voltage or forward voltage – must be exceeded
* The threshold voltage differs depending on the chemical element the diode is based on
</left>
<right>
* Germanium: $\qtyrange{0.2}{0.4}{\volt}$
* Silicon: $\qtyrange{0.6}{0.8}{\volt}$
* LED (red): $\qtyrange{1.6}{2.2}{\volt}$
* LED (yellow, green): $\qtyrange{1.9}{2.5}{\volt}$
* LED (blue, white): $\qtyrange{2.7}{3.5}{\volt}$
</right>

---
[question:EC503]
---

## Schottky diode

* Allows a high switching frequency
* Needs only a very low threshold voltage, from $\qty{0.4}{\volt}$ down to below $\qty{0.1}{\volt}$

---
[question:EC504]
---

## Characteristics

---
[question:EC506]
---
[question:EC507]
---
[question:EC508]
---
[question:EC505]
---

## Conducting diode

<left>
* A diode always conducts when the voltage at the anode is more positive than at the cathode by the threshold voltage
* This also applies to negative voltages
* The examination only uses silicon diodes with a threshold voltage of $\qty{0.7}{\volt}$
</left>
<right>
[picture:113:e_leitende_siliziumdiode:Voltages across a conducting silicon diode]
</right>

---
[question:EC513]
---
[question:EC510]
---
[question:EC509]
---
[question:EC511]
---
[question:EC512]
---

## LED application 

<left>
* An LED serves as an indicator light
</left>
<right>
[picture:324:e_led_schaltung:LED with series resistor]
</right>

---
[question:EC514]
---
### Series resistor

<left>
* Since the LED itself has hardly any resistance, it would act like a short circuit if connected directly to a voltage source
* A series resistor limits the forward current
</left>
<right>
[picture:324:e_led_schaltung:LED with series resistor]
</right>

---
* Calculation: $R = \dfrac{U_q - U_{\mathrm{LED}}}{I_D}$
* $U_q$: voltage source
* $U_{\mathrm{LED}}$: threshold voltage of the LED
* $I_D$: forward current

---
[question:EC515]
---
[question:EC516]
---

## Zener diode

<left>
* The maximum reverse voltage of a diode is normally around $\qty{1000}{\volt}$
* In Zener diodes, voltage breakdown occurs between $\qty{3}{\volt}$ and $\qty{100}{\volt}$, depending on the type
* Used for voltage stabilisation
</left>
<right>
[picture:560:_e_z_diode:Circuit symbol of a Zener diode]
</right>
<note>
* Originally named after Clarence Melvin Zener
* Today other effects are decisive, but the name Zener diode has stuck
</note>

---
### Polarity

<left>
* Zener diodes are operated in the reverse direction with a series resistor
</left>
<right>
[picture:549:e_z_diode_polung:Zener diode correctly connected in the reverse direction]
</right>

---
[question:EC517]
---
[question:EC518]
---
[question:EC519]
---
[question:EC520]
---

### Series resistor

<left>
[picture:753:e_z_diode_spannungsstabilisierung:Zener diode for voltage stabilisation]
</left>
<right>
* $U_Z$ is the voltage to which the Zener diode stabilises
* $U_V = U_1 - U_Z = \qty{13.8}{\volt} - \qty{5}{\volt} = \qty{8.8}{\volt}$
* $R_V = \frac{U_V}{I} = \frac{\qty{8.8}{\volt}}{\qty{30}{\milli\ampere}} \approx \qty{293}{\ohm}$
</right>
---
[question:EC521]
---
[question:EC522]

<note>
* The currents through the series resistor add up
* Kirchhoff's laws have not been covered yet
</note>