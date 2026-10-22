* *Amplifier class A*: Can amplify the whole signal
* *Amplifier class B*: Half of the signal is amplified well
* *Amplifier class AB*: Combination of A and B, amplifying a little more than half of the signal
* *Amplifier class C*: Less than half of the signal is amplified well

<fragment>
The amplifier classes are determined by the choice of operating point
</fragment>

<note>
The letter designations go back to an early systematic classification of valve and transistor amplifiers
</note>
---
<left>
[picture:377:a_kennlinien_transistor_arbeitspunkt:Characteristic of a transistor with operating points]
</left>
<right>
* The transistor characteristic shows the relationship between input signal and output signal
* Base-emitter or gate-source voltage and collector or drain current
* In linear regions the change is proportional
* Other regions are non-linear
</right>
---
### Operating point

* Optimum operation with the best choice of operating point on the characteristic
* The operating point is set by the bias at the base or gate
* Amplification then takes place around the desired operating point

---
### Quiescent current

* The quiescent current results from the choice of operating point
* Flows even without an input signal
* Affects the efficiency of an amplifier
* Increases the power dissipated as heat
* Reduces the efficiency

--- style="font-size: smaller;"
### AP1
<left>
[picture:377:a_kennlinien_transistor_arbeitspunkt:Characteristic of a transistor with operating points]  
</left>
<right>
* Class C operation of the amplifier
* no bias
* quiescent current zero
* efficiency approx. $\qtyrange{80}{87}{\percent}$
* high harmonic content
</right>
--- style="font-size: smaller;"
### AP2
<left>
[picture:377:a_kennlinien_transistor_arbeitspunkt:Characteristic of a transistor with operating points]  
</left>
<right>
* Class B operation of the amplifier
* Small bias, up to the onset of collector current
* Quiescent current almost zero (low)
* Efficiency up to $\qty{80}{\percent}$
* low harmonic content
</right>
--- style="font-size: smaller;"
### AP3
<left>
[picture:377:a_kennlinien_transistor_arbeitspunkt:Characteristic of a transistor with operating points]  
</left>
<right>
* Class AB operation of the amplifier
* Higher bias than in class B operation, but lower than in class A operation
* Quiescent current larger than in class B operation, but considerably smaller than in class A operation
* Efficiency between $\qty{50}{\percent}$ and $\qty{80}{\percent}$
* low harmonic content
</right>
--- style="font-size: smaller;"
### AP4
<left>
[picture:377:a_kennlinien_transistor_arbeitspunkt:Characteristic of a transistor with operating points]  
</left>
<right>
* Class A operation of the amplifier
* Bias set so that the quiescent current reaches approx. $\qty{50}{\percent}$ of the maximum permitted value
* Efficiency approx. $\qty{40}{\percent}$
* very low harmonic content
</right>
---
[question:AD416]
---
[question:AD419]
---
[question:AD420]
---
[question:AD421]
---
### Output power

* If the operating point is known, the efficiency is known
* Calculate the DC power
* The output power is the product of the DC power and the efficiency

---
[question:AD424]
---
#### Solution
* given: $U=\qty{50}{\volt}$
* given: $I = \qty{2}{\ampere}$
* given: $\eta_\text{A} \approx \qty{40}{\percent}$
* required: $P_\text{ab}$

<fragment>
$P_\text{zu} = U \cdot I = \qty{50}{\volt} \cdot \qty{2}{\ampere} = \qty{100}{\watt}$
</fragment>
<fragment>
$\eta_\text{A} = \frac{P_\text{ab}}{P_\text{zu}} \Rightarrow P_\text{ab} = \eta_\text{A} \cdot P_\text{zu} = 0.4 \cdot \qty{100}{\watt} = \qty{40}{\watt}$
</fragment>
---
[question:AD425]
---
#### Solution
* given: $U=\qty{50}{\volt}$
* given: $I = \qty{2}{\ampere}$
* given: $\eta_\text{C} \approx \qty{85}{\percent}$
* required: $P_\text{ab}$

<fragment>
$P_\text{zu} = U \cdot I = \qty{50}{\volt} \cdot \qty{2}{\ampere} = \qty{100}{\watt}$
</fragment>
<fragment>
$\eta_\text{C} = \frac{P_\text{ab}}{P_\text{zu}} \Rightarrow P_\text{ab} = \eta_\text{C} \cdot P_\text{zu} = 0.85 \cdot \qty{100}{\watt} = \qty{85}{\watt}$
</fragment>
---
[question:AD418]
---
[question:AD417]
---
### SSB operation

* Linear amplification is needed
* Amplification in class A, AB or B operation
* Overdriving leads to distortion of the signal $\rightarrow$ splatter on adjacent frequencies

---
[question:AD422]
---
[question:AJ218]
---
[question:AD423]
---
### Class C operation

* Non-linear operating point produces harmonics
* These must then be suppressed by filtering
* Screening by a metal case

---
[question:AF402]
---
[question:AF403]
