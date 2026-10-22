<left>
[photo:268:a_I eilt vor:Phase shift between voltage and current in a capacitor]
</left>
<right>
* Phase shift of $\qty{90}{\degree}$
* The current leads the voltage
</right>
<note>
Remember: Kondensatoooor, Strom eilt vooor! (capacitor: the current leads)
</note>
---
[question:AC101]
---
### Real power
<left>
[picture:943:a_Blindleistung Kondensator:The product $U \cdot I$ gives the green power curve]
</left>
<right>
* The green power curve is the product of current and voltage
* The power swings symmetrically about the zero line and cancels out
* *Reactive power* in a *reactance*
</right>
---
[question:AC111]
<note>
In the steady state almost no current flows any more, which is why the power is also almost 0 W.
</note>
---
* Real power is dissipated only in an ohmic resistance (current and voltage in phase)
* A reactance absorbs no real energy
* So it does not get warm
* A capacitor that gets warm at radio frequency has a resistive part and should be replaced

---
[question:AC103]

--- style="font-size: smaller;"
### Capacitive reactance $X_{\textrm{C}}$

A capacitor connected to an AC voltage is constantly charged and discharged $\rightarrow$ AC resistance / capacitive reactance

<fragment>
1. If the frequency of the AC voltage across a capacitor is increased, more current flows; this means that the capacitive reactance has become smaller.
</fragment>
<fragment>
2. If the capacitance of the capacitor is increased, the current rises as well, i.e. the reactance also becomes smaller.
</fragment>

<fragment>
$X_{\textrm{C}} = \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}$
</fragment>

<note>
A VNA measures how the reactance $X_C$ changes with frequency
</note>
---
[question:AC102]
---
[question:AC104]
---
#### Solution
* given: $C = \qty{10}{\pico\farad}$
* given: $f = \qty{100}{\mega\hertz}$
* required: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{100}{\mega\hertz} \cdot \qty{10}{\pico\farad}}\\ &\approx \qty{159}{\ohm} \end{split}$
</fragment>

---
[question:AC105]
---
#### Solution
* given: $C = \qty{50}{\pico\farad}$
* given: $f = \qty{145}{\mega\hertz}$
* required: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{145}{\mega\hertz} \cdot \qty{50}{\pico\farad}}\\ &\approx \qty{22}{\ohm} \end{split}$
</fragment>
---
[question:AC106]
---
#### Solution
* given: $C = \qty{100}{\pico\farad}$
* given: $f = \qty{100}{\mega\hertz}$
* required: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{100}{\mega\hertz} \cdot \qty{100}{\pico\farad}}\\ &\approx \qty{15.9}{\ohm} \end{split}$
</fragment>

---
[question:AC107]
---
#### Solution
* given: $C = \qty{100}{\pico\farad}$
* given: $f = \qty{435}{\mega\hertz}$
* required: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{435}{\mega\hertz} \cdot \qty{100}{\pico\farad}}\\ &\approx \qty{3.7}{\ohm} \end{split}$
</fragment>

---
[question:AC108]
---
#### Solution
<left>
* given: $U = \qty{16}{\volt}$
* given: $I = \qty{32}{\milli\ampere}$
</left>
<right>
* given: $f = \qty{50}{\hertz}$
* required: $C$
</right>

<fragment>
$X_{\textrm{C}} = \frac{U}{I} = \frac{\qty{16}{\volt}}{\qty{32}{\milli\ampere}} = \qty{500}{\ohm}$
</fragment>

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} \\ \Rightarrow C &= \frac{1}{\omega \cdot X_{\textrm{C}}} = \frac{1}{2\pi \cdot f \cdot X_{\textrm{C}}}\\ &= \frac{1}{2\pi \cdot \qty{50}{\hertz} \cdot \qty{500}{\ohm}}\\ &\approx \qty{6.37}{\micro\farad}\end{split}$
</fragment>

---
### Capacitor losses

<left>
[photo:260:a_Kondensator Ersatzschaltbild:Equivalent circuit of a real capacitor with a series loss resistance (ESR).]
</left>
<right>
* Dissipation factor<br/>$\tan(\delta) = \frac{R}{X_C}$
* Losses in the dielectric and the leads
</right>

---
[question:AC109]
---
[question:AC110]
