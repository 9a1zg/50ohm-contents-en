<left>
[photo:267:a_U_eilt_vor:Phase shift between voltage and current in an inductor]
</left>
<right>
* Phase shift of $\qty{90}{\degree}$
* The voltage leads the current
</right>
<note>
Remember: Bei Induktivitäten, Ströme sich verspäten -or- Induktivitääät, Strom zu spääät! (in the inductance, the current is late)
</note>

---
[question:AC201]

---
### Real power

<left>
[picture:944:a_Blindleistung Spule:The product $U \cdot I$ gives the green power curve]
</left>
<right>
* The green power curve is the product of current and voltage
* The power swings symmetrically about the zero line and cancels out
* *Reactive power* in a *reactance*
</right>

---

* A reactance absorbs no real energy
* An ideal inductor does not get warm
* However, an inductor is made of wire and so has ohmic losses
* In addition, the skin effect acts

---
[question:AC202]

--- style="font-size: smaller;"
### Inductive reactance $X_{\textrm{L}}$

An inductor connected to an AC voltage constantly reverses its magnetic field $\rightarrow$ AC resistance / inductive reactance

1. If the frequency of the AC voltage across an inductor is increased, less current flows; this means that the inductive reactance has become larger.
2. If the inductance of the inductor is increased, the current also decreases, i.e. the reactance also becomes larger.

<fragment>
$|X_{\textrm{L}}| = \omega \cdot L = 2\pi \cdot f \cdot L$
</fragment>

---
[question:AC203]
---
[question:AC204]
---
#### Solution
* given: $L = \qty{3}{\micro\henry}$
* given: $f = \qty{100}{\mega\hertz}$
* required: $X_{\textrm{L}}$

<fragment>
$\begin{split} |X_{\textrm{L}}| &= \omega \cdot L = 2\pi \cdot f \cdot L\\ &= 2\pi \cdot \qty{100}{\mega\hertz} \cdot \qty{3}{\micro\henry}\\ &\approx \qty{1885}{\ohm} \end{split}$
</fragment>

---
### Increasing the inductance
<left>
Solenoid
<fragment>
$L = \dfrac{\mu_0 \cdot \mu_r \cdot N^2 \cdot A_S}{l}$
</fragment>

* Increase the number of turns $N$
* Shorten the length $l$ of the coil
* Enlarge the cross-sectional area $A_S$ of the coil

</left>
<right>
Toroidal inductor
<fragment>
$L = N^2 \cdot A_{\textrm{L}}$
</fragment>
  
* Increase the number of turns $N$
* Use a core material that conducts magnetic flux better (with a larger inductance factor $A_{\textrm{L}}$)

</right>

<note>
That is why (toroidal) cores are used
</note>
---
[question:AC211]

---
[question:AC205]
---
#### Solution
* given: $N = 14$
* given: $A_{\textrm{L}} = \qty{1.5}{\nano\henry}$
* required: $L$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ &= 14^2 \cdot \qty{1.5}{\nano\henry}\\ &= \qty{0.294}{\micro\henry} \end{split}$
</fragment>

---
[question:AC206]
---
#### Solution
* given: $N = 300$
* given: $A_{\textrm{L}} = \qty{1250}{\nano\henry}$
* required: $L$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ &= 300^2 \cdot \qty{1250}{\nano\henry}\\ &= \qty{112.5}{\milli\henry} \end{split}$
</fragment>

---
[question:AC207]
---
#### Solution
* given: $L = \qty{2}{\milli\henry}$
* given: $A_{\textrm{L}} = \qty{250}{\nano\henry}$
* required: $N$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ N &= \sqrt{\frac{L}{A_{\textrm{L}}}} = \sqrt{\frac{\qty{2}{\milli\henry}}{\qty{250}{\nano\henry}}} \\ &= 89\,\text{turns} \end{split}$
</fragment>

---
[question:AC208]
---
#### Solution
* given: $L = \qty{12}{\micro\henry}$
* given: $A_{\textrm{L}} = \qty{30}{\nano\henry}$
* required: $N$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ N &= \sqrt{\frac{L}{A_{\textrm{L}}}} = \sqrt{\frac{\qty{12}{\micro\henry}}{\qty{30}{\nano\henry}}} \\ &= 20\,\text{turns} \end{split}$
</fragment>

---
### Inductor losses

* Dissipation factor $\tan(\delta) = \frac{R}{X_L}$
* Losses in the conductor

---
[question:AC209]

---
### Impedance

* Series connection of reactance and resistance $\rightarrow$ impedance $Z$
* Occurs only with AC voltage
* Cannot be measured with an ohmmeter
* Inductor in radio engineering $\rightarrow$ *impedance*
* Antenna impedance, input and output impedance, impedance transformer, …
* Impedance $Z$ in $\unit{\ohm}$

---
<left>
[picture:1067:a_impedanzdreieck:Impedance $Z$ as the geometric sum of $R$ and $X$]
  
$Z = \sqrt{R^2 + X^2}$
</left>
<right>
* Resistance $R$
* Reactance $X_{\textrm{L}}$
* The impedance is calculated with Pythagoras
</right>

---
[question:AA101]

---
### Screening magnetic fields

<left>
* For screening: a case made of a highly conductive material.
* Example: screening can made of steel or iron.
* Adjustable ferrite core to change the inductance.
</left>
<right>
[photo:333:a_abschirmbecher:Example of inductors with screening cans for screening magnetic fields]
</right>


---
[question:AC210]
