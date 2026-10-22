## Battery types

The most common types of rechargeable battery in amateur radio:
* Lead-acid battery (Pb)
* Nickel-metal hydride (NiMH)
* Lithium iron phosphate (LiFePO4)

---
[photo:175:a_akku_lifepo4:LiFePO4]

<left>
* Capacity: $\qty{4200}{\milli\ampere\hour}$
* Voltage: 4S1P / $\qty{13.2}{\volt}$
</left>
<right>
* Discharge: 30C constant / 40C burst
* Balance connector: JST-XH
</right>

---
### Configurations

Examples:

* 4S1P: 4 cells in series, 1 in parallel
* 4S2P: 4 cells in series, 2 in parallel

<fragment>
Per cell approx. $\qty{3.2}{\volt}$ to $\qty{3.3}{\volt}$, so<br/>$\qty{3.3}{\volt} \cdot 4 = \qty{13.2}{\volt}$
</fragment>

---
### Capacity

Example battery: $\qty{4200}{\milli\ampere\hour} = \qty{4.2}{\ampere\hour}$

<fragment>
$\rightarrow$ load with $\qty{4.2}{\ampere}$ for 1 hour or with $\qty{2.1}{\ampere}$ for 2 hours
</fragment>
<fragment>
$t = \frac{Q}{I}$
</fragment>
<fragment>
$t = \frac{\qty{4.2}{\ampere\hour}}{\qty{4.2}{\ampere}} = \qty{1}{\hour}$
</fragment>
<note>
If necessary, convert hours to seconds with $\qty{1}{\hour} = \qty{3600}{\second}$
</note>
---
### Electrical energy

Electrical energy stored in the battery

$E = Q \cdot U$

<fragment>
Example battery: $E = \qty{4.2}{\ampere\hour} \cdot \qty{13.2}{\volt} = \qty{55.44}{\watt\hour}$
</fragment>
---
### Discharge current

Marking on the example battery: 30C

The battery can be discharged at 30 times the capacity $Q$

<fragment>
Discharge current = $30 \cdot \frac{1}{\unit{\hour}} \cdot \qty{4.2}{\ampere\hour} = \qty{126}{\ampere}$
</fragment>

<fragment>
The battery would be discharged in 128 seconds.
</fragment>

<note>
Mind the cable cross-section
</note>

---
### Connecting batteries in series

<left>
[photo:176:a_akku_4S1P:Series connection]
</left>
<right>
* The voltages add
* Only connect together cells with the same ratings
</right>
<note>
If the ratings differ, the cells affect or damage one another
</note>

---
### Connecting batteries in parallel

<left>
[photo:177:a_akku_4S2P:Parallel connection]
</left>
<right>
* The voltages stay the same
* The capacities add
</right>
<note>
</note>

---
### Balancer

<left>
[photo:178:a_akku_lifepo4_anschluss:LiFePO4 connections]
</left>
<right>
* The balancer connector gives access to the voltage of each cell
* Balancer circuit to equalise the voltages
* Protection of the cells
* Battery monitor
</right>
<note>
</note>

---
[question:AB210]
---
[question:AB209]
---
#### Solution
* given: $U = \qty{2}{\volt}$
* given: $Q = \qty{10}{\ampere\hour}$
* given: $N = 6$
* required: $U_{\mathrm{ges}}, Q_{\mathrm{ges}}$

<fragment>
$U_{\mathrm{ges}} = N \cdot U = 6 \cdot \qty{2}{\volt} = \qty{12}{\volt}$
</fragment>
<fragment>
$Q_{\mathrm{ges}} = Q \cdot 1 = \qty{10}{\ampere\hour}$
</fragment>
---

[question:AB211]
---
#### Solution
* given: $Q_{\mathrm{max}} = \qty{60}{\ampere\hour}$
* given: $Q_{\qty{10}{\percent}} = 0.1 \cdot Q_\mathrm{max} = \qty{6}{\ampere\hour}$
* given: $I = \qty{0.8}{\ampere}$
* required: $t$

<fragment>
$Q = I \cdot t \Rightarrow t = \frac{Q}{I} = \frac{Q_{\mathrm{max}} - Q_{10\%}}{I} = \frac{\qty{54}{\ampere\hour}}{\qty{0.8}{\ampere}} = \qty{67.5}{\hour}$
</fragment>

---
[question:AB501]
---
#### Solution
* given: $U = \qty{12}{\volt}$
* given: $Q = \qty{5}{\ampere\hour}$
* required: $W$

<fragment>
$W = P \cdot t = U \cdot I \cdot t = U \cdot Q = \qty{12}{\volt} \cdot \qty{5}{\ampere\hour} = \qty{60.0}{\watt\hour}$
</fragment>