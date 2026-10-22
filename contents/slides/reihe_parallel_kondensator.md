## Series connection

* Since it is the voltage that sets up the electric field (and it is divided in a series connection), the capacitance is calculated in exactly the opposite way to resistors.
* Application: at high voltages, several capacitors are connected in series to prevent the risk of breakdown. What helps here is that the total voltage is divided between the capacitors.

---

* When capacitors are connected in series, the total capacitance is smaller than the value of the smallest capacitor

[picture:823:e_reihenschaltung_kondensatoren:Series connection of 3 capacitors]

$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{C_{1}} + \frac{1}{C_{2}} + \frac{1}{C_{3}}$

---

* Simplification for two capacitors:

$C_{\mathrm{ges}} = \dfrac{C_{1} \cdot C_{2}}{C_{1} + C_{2}}$

---

* Simplification for equal capacitors:

$C_{\mathrm{ges}} = \dfrac{C}{n}$

$n$ is the number of capacitors

---

[question:ED119]

---

[question:ED120]

---

## Parallel connection

* Here it is exactly the opposite of resistors, because the same voltage is applied to all the capacitors, and it is the voltage that sets up the electric field.
* Application: capacitors are connected in parallel to make up the value you need from the preferred values.

<note>
* Capacitors connected in parallel act like one large capacitor
</note>

---

* In a parallel connection, the capacitances add up

[picture:822:e_parallelschaltung_kondensatoren:Parallel connection of 3 capacitors]

$C_{\mathrm{ges}} = C_{1} + C_{2} + C_{3}$

---

[question:ED117]

---

[question:ED118]

---

## Series-parallel circuits

--- style="font-size: 0.7em;"

### Variant 1: two in parallel, plus one in series

<left>
* Here you first calculate the parallel connection of $C_{2}$ and $C_{3}$

$C_{\mathrm{ges,p}} = C_{2} + C_{3}$

* Then you calculate the series connection of $C_{1}$ and $C_{\mathrm{ges,p}}$

$C_{\mathrm{ges}} = \frac{C_{1} \cdot C_{\mathrm{ges,p}}}{C_{1} + C_{Gp}}$
</left>
<right>
[picture:820:e_gemischt_variante_1:Series-parallel circuit - variant 1]
</right>

---

[question:ED123]

---

[question:ED124]

---

[question:ED122]

--- style="font-size: 0.7em;"

### Variant 2: two in series, plus one in parallel

<left>
* Here you first calculate the series connection of $C_{1}$ and $C_{2}$

$C_{\mathrm{ges,r}} = \frac{C_{1} \cdot C_{2}}{C_{1} + C_{2}}$

* Then you calculate the parallel connection of $C_{3}$ and $C_{\mathrm{ges,r}}$

$C_{\mathrm{ges}} = \frac{C_{3} \cdot C_{\mathrm{ges,r}}}{C_{3} + C_{\mathrm{ges,r}}}$
</left>
<right>
[picture:457:e_gemischt_variante_2:Series-parallel circuit - variant 2]
</right>

---

[question:ED121]

