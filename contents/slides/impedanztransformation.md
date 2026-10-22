## Impedance transformation in the feeder

* A characteristic impedance that differs from the load resistance leads to impedance transformation as well as to standing waves
* The signal source "sees" different resistances at the ends of the cable
* $\lambda/4$ lines transform low resistances into high ones and high resistances into low ones
* $\lambda/2$ lines cause no impedance transformation

---
[question:AG412]

---
[question:AG416]
---

### Feeding half-wave and full-wave dipoles

<left>
[picture:312:a_impedanztransformation_speiseleitung:Half-wave dipole with impedance transformation via the feeder]
</left>
<right>
* Half-wave dipole: current-fed (low impedance)
* Full-wave dipole: voltage-fed (high impedance)
</right>

---
[question:AG413]

---
[question:AG414]

---
[question:AG415]
---

### Calculating the characteristic impedance
* For a specific impedance transformation: $Z = \sqrt{Z_\mathrm{E} \cdot Z_\mathrm{A}}$
* The characteristic impedance is the geometric mean of the input impedance and the load resistance

---
[question:AG417]
---
#### Solution
* given: $Z_A = \qty{60}{\ohm}$
* given: $Z_E = \qty{240}{\ohm}$
* required: $Z$

<fragment>
$\begin{split}Z &= \sqrt{Z_E \cdot Z_A}\\ &= \sqrt{\qty{240}{\ohm} \cdot \qty{60}{\ohm}}\\ &= \qty{120}{\ohm}\end{split}$ 
</fragment>
---
[question:AG418]
---
#### Solution
* given: $Z_A = \qty{240}{\ohm}$
* given: $Z_E = \qty{600}{\ohm}$
* required: $Z$

<fragment>
$\begin{split}Z &= \sqrt{Z_E \cdot Z_A}\\ &= \sqrt{\qty{600}{\ohm} \cdot \qty{240}{\ohm}}\\ &= \qty{380}{\ohm}\end{split}$ 
</fragment>
---

### Impedance matching with pi filters

<left>
[picture:425:a_impedanztransformation_pi_filter:Pi filter for impedance transformation]
</left>
<right>
* Inductors and capacitors are used for impedance matching
* Pi filters act as low-pass filters and transform the impedance
* They can be used as antenna tuners
</right>

<note>
The name "pi filter" comes from the arrangement of the components, which resembles the Greek letter $\pi$; it has nothing to do with the mathematical constant.
</note>

---
[question:AG406]
