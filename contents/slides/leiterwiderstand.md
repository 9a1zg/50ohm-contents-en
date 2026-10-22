## Resistance of wires

<left>
* Conductive material consists of atoms in a (lattice) structure
* Electrons are shared and are therefore free to move
* Depending on the material, there are more or fewer free electrons, which collide with atoms
</left>
<right>
[picture:713:a_leitermodell:Atoms (+) and mobile electrons (-) in a metallic conductor]
</right>

---
### Resistivity $\rho$
<left>
$R = \frac{\rho\cdot l}{A_{\textrm{Dr}}}$

* $l$: wire length
* $A_{\textrm{Dr}}$: wire cross-section
* $\rho$: resistivity in $\unit{\ohm\cdot\milli\meter\squared\per\meter}$
</left>
<right>
<fragment>
* Copper: 0.018
* Aluminium: 0.028
* Gold: 0.022
* Silver: 0.016
* Zinc: 0.11
* Iron: 0.1
* Brass: 0.07
</fragment>
</right>
<note>
This allows the ohmic resistance of a wire to be calculated when the material, the length and the cross-section are known
</note>

---
[question:AB101]
--- style="font-size: smaller;"
### Solution
* given: $l = \qty{1.8}{\meter}$
* given: $d = \qty{0.2}{\milli\meter}$
* given: $\rho = \qty{0.018}{\ohm\cdot\milli\meter\squared\per\meter}$
* required: $R$

<fragment>
$$A_{\textrm{Dr}} = \frac{d^2\cdot \pi}{4} = \frac{(\qty{0.2}{\milli\meter})^2 \cdot \pi}{4} = \frac{\pi}{100}\unit{\milli\meter\squared} = \qty{0.0314}{\milli\meter\squared}$$
</fragment>
<fragment>
$$R = \frac{\rho\cdot l}{A_{\textrm{Dr}}} = \frac{\qty{0.018}{\ohm\cdot\milli\meter\squared\per\meter} \cdot \qty{1.8}{\meter}}{\qty{0.0314}{\milli\meter\squared}} \approx \qty{1.02}{\ohm}$$
</fragment>
---
[question:AB102]
---
### Solution
* given: $A_{\textrm{Dr}} = \qty{0.5}{\milli\meter\squared}$
* given: $R = \qty{1.5}{\ohm}$
* given: $\rho = \qty{0.018}{\ohm\cdot\milli\meter\squared\per\meter}$
* required: $l$

<fragment>
$\begin{split} R &= \frac{\rho\cdot l}{A_{\textrm{Dr}}}\\ \Rightarrow l &= \frac{R\cdot A_{\textrm{Dr}}}{\rho} = \frac{\qty{1.5}{\ohm} \cdot \qty{0.5}{\milli\meter\squared}}{\qty{0.018}{\ohm\cdot\milli\meter\squared\per\meter}} \approx \qty{41.7}{\meter} \end{split}$
</fragment>

---
## Temperature coefficient

* The resistance of metals rises as the temperature increases
* At higher temperatures the atoms move more, which leads to more collisions with electrons

---
[question:AB103]