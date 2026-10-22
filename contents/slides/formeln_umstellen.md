## Rearranging formulas

* In Class N: two ready-made tailored quantity equations
  * $f[[\unit{\mega\hertz}]] = \dfrac{300}{\lambda[[\unit{\meter}]]}$
  * $\lambda[[\unit{\meter}]] = \dfrac{300}{f[[\unit{\mega\hertz}]]}$
* This is only *one* equation – rearranged once for $f$, once for $\lambda$

<note>
* In-depth on the website: definition of "tailored quantity equation" and the relationship $\lambda = c_0 / f$ in base units
</note>

---

* In Class E and A the formula sheet gives only the basic form
  * There, rearranging is essential
* Method: apply the necessary operation ($\cdot$, $:$, $+$, $-$, …) to *both* sides at the same time

---

We already had $\lambda = \dfrac{c_0}{f}$

But how do we get to $c_0 = f \cdot \lambda$ and $f = \dfrac{c_0}{\lambda}$?

---
## Mathematical approach

$\lambda = \dfrac{c_0}{f}$ is to be rearranged for $f$.

* $|~\cdot f$ or $|~: \lambda$: carry out the operation on *both* sides
* A quantity in the numerator *and* the denominator cancels out ($\frac{f}{f} = 1$)

---
#### Step 1
Multiply both sides by $f$ to get it on the left.

<fragment>
$\lambda = \dfrac{c_0}{f} \quad\quad\quad | \cdot f$
</fragment>
<fragment>
$\lambda\cdot f = \dfrac{c_0 \cdot f}{f}$
</fragment>
<fragment>
After cancelling
$\lambda \cdot f = c_0$
</fragment>

---
#### Step 2
Divide both sides by $\lambda$ to get it on the right.

<fragment>
$\lambda \cdot f = c_0 \quad\quad\quad |: \lambda$
</fragment>
<fragment>
$\frac{\lambda\cdot f}{\lambda} = \frac{c_0}{\lambda}$
</fragment>
<fragment>
$f = \dfrac{c_0}{\lambda}$
</fragment>

---
## Numerical example

Which frequency corresponds to $\lambda = \qty{2.069}{\meter}$?

* Use base units ($\unit{\meter}$, $\unit{\second}$)
  * $\frac{1}{\unit{\second}} = \qty{1}{\hertz}$ applies

$f = \dfrac{c_0}{\lambda} = \dfrac{\qty{3e8}{\meter\per\second}}{\qty{2.069}{\meter}} \approx \qty{145}{\mega\hertz}$

---
## Looking ahead

* We can now rearrange using multiplication and division
* Class E: also addition, subtraction, powers, roots
* Class A: also logarithms
* Each is explained step by step where it comes up
