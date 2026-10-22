### Parallel tuned circuit

* Inductors and capacitors are combined
* The *inter-winding capacitance* must also be taken into account
* This brings "invisible" capacitances into the circuit

<note>
Self-capacitance of an inductor
</note>
---
[question:AD101]
---
#### Solution

* given: $C_1 = \qty{0.10}{\nano\farad}$
* given: $C_2 = \qty{47}{\pico\farad}$
* given: $C_3 = \qty{22}{\pico\farad}$
* required: $C_{\mathrm{ges}}$

<fragment>
$\begin{split} \tfrac{1}{C_{\mathrm{ges}}} &= \tfrac{1}{C_1} + \tfrac{1}{C_2} + \tfrac{1}{C_3} = \tfrac{1}{\qty{0.10}{\nano\farad}} + \tfrac{1}{\qty{47}{\pico\farad}} + \tfrac{1}{\qty{22}{\pico\farad}}\\ &= \qty{7.67e10}{\farad^{-1}}\\ \Rightarrow C_{\mathrm{ges}} &= \frac{1}{\qty{7.67e10}{\farad^{-1}}} \approx \qty{13.0}{\pico\farad} \end{split}$
</fragment>
---
[question:AD103]
---
#### Solution

* given: $C_1 = \qty{0.1}{\nano\farad}$
* given: $C_2 = \qty{1.5}{\nano\farad}$
* given: $C_3 = \qty{220}{\pico\farad}$
* given: $C_L = \qty{1}{\pico\farad}$
* required: $C_{\mathrm{ges}}$

<fragment>
$\begin{split} C_{\mathrm{ges}} &= C_1 + C_2 + C_3 + C_L\\ &= \qty{0.1}{\nano\farad} + \qty{1.5}{\nano\farad} + \qty{220}{\pico\farad} + \qty{1}{\pico\farad}\\ &= \qty{1821}{\pico\farad} \end{split}$
</fragment>
<note>
Watch the unit prefixes and calculate with reciprocals
</note>

---
[question:AD105]
---
#### Solution

* given: $R = \qty{100}{\ohm}$
* given: $L = \qty{100}{\micro\henry}$
* given: $f = \qty{1}{\mega\hertz}$
* required: $Z$

<fragment>
$\begin{split} X_L &= \omega \cdot L = 2\pi \cdot f \cdot L\\ &= 2\pi \cdot \qty{1}{\mega\hertz} \cdot \qty{100}{\micro\henry} = \qty{628}{\ohm}\end{split}$
</fragment>
<fragment>
$Z = \sqrt{R^2 + X^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{628}{\ohm})^2} \approx \qty{636}{\ohm}$
</fragment>

---
[question:AD104]
---
#### Solution

* given: $R = \qty{100}{\ohm}$
* given: $C = \qty{100}{\nano\farad}$
* given: $f = \qty{1}{\mega\hertz}$
* required: $Z$

<fragment>
$\begin{split} X_C &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{1}{\mega\hertz} \cdot \qty{100}{\nano\farad}} = \qty{159}{\ohm}\end{split}$
</fragment>
<fragment>
$Z = \sqrt{R^2 + X^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{159}{\ohm})^2} \approx \qty{188}{\ohm}$
</fragment>
