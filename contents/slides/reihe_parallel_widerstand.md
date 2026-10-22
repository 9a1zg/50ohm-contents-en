## Series connection

In a series connection, the resistance values add up

[picture:812:e_reihenschaltung_von_r:Series connection of 3 resistors]

$R_{\mathrm{ges}} = R_{1} + R_{2} + R_{3}$
Example: $R_{\mathrm{ges}} = \qty{100}{\ohm} + \qty{200}{\ohm} + \qty{300}{\ohm}$

--- style="font-size: 0.7em;"

## Parallel connection

When resistors are connected in parallel, the total resistance is smaller than the value of the smallest resistor

[picture:811:e_parallelschaltung_von_r:Parallel connection of 3 resistors]

$\frac{1}{R_{\mathrm{ges}}} = \frac{1}{R_{1}} + \frac{1}{R_{2}} + \frac{1}{R_{3}}$



---

Simplification for two resistors:
$R_{\mathrm{ges}} = \dfrac{R_{1} \cdot R_{2}}{R_{1} + R_{2}}$

---

Simplification for equal resistors:
$R_{\mathrm{ges}} = \dfrac{R}{n}$
$n$ is the number of resistors

---

[question:ED104]

---

[question:ED105]

---

[question:ED106]

---

## Series-parallel circuits

--- style="font-size: 0.7em;"

### Variant 1: two in parallel, plus one in series

[picture:813:e_gemischte_schaltung_1:Series-parallel circuit - variant 1]

<fragment>
Here you first calculate the parallel connection of $R_2$ and $R_3$ and then add $R_1$.
</fragment>

<fragment>
$R_{\mathrm{ges}} = \dfrac{R_{2} \cdot R_{3}}{R_{2} + R_{3}} + R_{1}$
</fragment>

---

### Variant 2: two in series, plus one in parallel

[picture:814:e_gemischte_schaltung_2:Series-parallel circuit - variant 2]

<fragment>
Here you first add $R_1$ and $R_2$, and then use the result to calculate the parallel connection with $R_3$.
</fragment>

<fragment>
$R_{\mathrm{ges}} = \dfrac{(R_{1} + R_{2}) \cdot R_{3}} {(R_{1} + R_{2}) + R_{3}}$
</fragment>

---

[question:ED110]

---

[question:ED111]

---

[question:ED108]

---

[question:ED109]

---

[question:ED112]

---

[question:ED113]

---

### Power rating of resistors in series and parallel connection

* In a series connection, the voltage divides.
* In a parallel connection, the current divides.
* So when calculating with $P = U \cdot I$, one value always stays the same and the other is correspondingly smaller.
* $\rightarrow$ in both cases the total power rating is greater than the individual power rating.

---

[question:ED107]
