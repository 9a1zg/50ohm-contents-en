---
## Dummy load for RF

<left>
[picture:47:a_dummy_load:Dummy load made of several chains of resistors]
</left>
<right>
* Often consists of several individual resistors, for better cooling and a higher power rating
* The resistors can be connected in parallel, in series or in combination
</right>
---

* Identical resistor values share the power dissipation equally
* Calculated with Ohm's law and the rules for series and parallel connections

---
[question:AI601]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $R = \qty{150}{\ohm}$
* given: $R_S = 4\cdot \qty{150}{\ohm} = \qty{600}{\ohm}$
</left>
<right>
* given: $R_{ges} = \qty{50}{\ohm}$
* given: $P_R = \qty{1}{\watt}$
* required: $n$ resistors, $P$
</right>

<fragment>
Chains of 4 resistors each:
$\frac{1}{R_{ges}} = n_S \cdot \frac{1}{R_S} \Rightarrow n_S = \frac{R_S}{R_{ges}} = \frac{\qty{600}{\ohm}}{\qty{50}{\ohm}} = 12$
$n = 4 \cdot n_S = 4 \cdot 12 = 48$ 
</fragment>
<fragment>
$P = n \cdot P_R = 48 \cdot \qty{1}{\watt} = \qty{48}{\watt}$
</fragment>

---
### Dummy load with a measurement output

* Can be used for indirect measurement of a transmitter's output power
* A peak rectifier converts the RF voltage into a DC voltage

---
[question:AI602]

---
### Measuring the RF output power via a potential divider

* A dummy load with a tap allows a rough determination of the power
* The partial RF voltage is converted using the divider ratio
* Can be measured with an RF probe and a multimeter

---
[question:AI603]

