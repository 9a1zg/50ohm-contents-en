<left>
[picture:342:daempfungsglied_pi:Attenuator in pi configuration with source and load resistor]
</left>
<right>
* Reduce signal levels by a defined amount
* Avoid overloading or damaging measuring instruments
* Reduce input levels for amplifiers and receivers to a defined level
</right>
<note>
The name pi configuration comes from the arrangement of the resistors as a &Pi;
</note>

---
<left>
[picture:342:daempfungsglied_pi:Attenuator in pi configuration with source and load resistor]
</left>
<right>
* Attenuation by resistors, with conversion into heat
* In symmetrical attenuators the input and output impedances are equal
* Usually $\qty{50}{\ohm}$
</right>

---
<left>
[picture:341:daempfungsglied_t:Attenuator in T configuration with source and load resistor]
</left>
<right>
* Attenuation is given in $\unit{\dB}$
* e.g. $\qty{20}{\dB}$ = factor of $\num{100}$
* $\qty{100}{\watt}$ input power $\rightarrow\qty{1}{\watt}$ output power
</right>
<note>
The name T configuration comes from the arrangement of the resistors as a T
</note>

---
[question:AD806]
--- style="font-size: smaller;"
#### Solution
* given: $P_1 = \qty{100}{\watt}$
* given: $a = \qty{20}{\dB}$
* required: $\Delta P = P_2 - P_1$

<fragment>
$\begin{split} a &= \qty{10 \cdot \log_{10}{\left(\frac{P_1}{P_2}\right)}}{\dB}\\ \Rightarrow \frac{a}{\qty{10}{\dB}} &= \log_{10}{\left(\frac{P_1}{P_2}\right)}\\ \Rightarrow 10^{\frac{a}{\qty{10}{\dB}}} &= \frac{P_1}{P_2}\\ \Rightarrow P_2 &= \frac{P_1}{10^{\frac{a}{\qty{10}{\dB}}}}\end{split}$
</fragment>
---
<fragment>
$P_2 = \frac{P_1}{10^{\frac{a}{10}}} = \frac{\qty{100}{\watt}}{10^{\frac{20}{10}}} = \qty{1}{\watt}$
</fragment>
<fragment>
$\Delta P = P_2 - P_1 = \qty{100}{\watt} - \qty{1}{\watt} = \qty{99}{\watt}$
</fragment>
---
[question:AD803]
---
#### Solution

* $\qty{20}{\dB}$ corresponds to a power attenuation by a factor of $\num{100}$

---
[question:AD804]
---
#### Solution

* $\qty{6}{\dB}$ corresponds to a power attenuation by a factor of $\num{4}$

---
[question:AD805]
---
#### Solution

* The impedance of the circuit as a whole does not change – so $\qty{50}{\ohm}$


---
[question:AD801]
---
[question:AD802]