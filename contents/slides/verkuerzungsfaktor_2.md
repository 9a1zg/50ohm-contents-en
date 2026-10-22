## Antenna length and shortening factor

* Antenna length depends on the shortening factor  
* Half-wave dipole: half the wavelength $\times$ shortening factor  
* Quarter-wave radiator: a quarter of the wavelength $\times$ shortening factor  
* Typical value: $\num{0.95}$  

---

[question:AG101]

---
#### Solution
<left>
* given: $f = \qty{14.2}{\mega\hertz}$
* given: $k_v = 0.95$
</left>
<right>
* given: $\frac{\lambda}{2}$ dipole
* required: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{1}{2} \cdot \frac{\lambda}{2}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &\approx \frac{1}{4} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{14.2}{\mega\hertz}}\\ &\approx \frac{1}{4} \cdot \qty{21.13}{\meter}\\ &\approx \qty{5.28}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0.95 \cdot \qty{5.28}{\meter}\\ &\approx \qty{5.02}{\meter}\end{split}$
</fragment>
</right>

---

[question:AG102]

---

#### Solution
<left>
* given: $f = \qty{7.1}{\mega\hertz}$
* given: $k_v = 0.95$
</left>
<right>
* given: $\frac{\lambda}{2}$ dipole
* required: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{1}{2} \cdot \frac{\lambda}{2}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &\approx \frac{1}{4} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{7.1}{\mega\hertz}}\\ &\approx \frac{1}{4} \cdot \qty{42.25}{\meter}\\ &\approx \qty{10.56}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0.95 \cdot \qty{10.56}{\meter}\\ &\approx \qty{10.04}{\meter}\end{split}$
</fragment>
</right>

---

[question:AG103]

---
#### Solution
<left>
* given: $l_G = \qty{20}{\meter}$
* given: $k_v = 0.95$
</left>
<right>
* given: dipole
* required: $f$
</right>

<left>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_E &= \frac{l_G}{k_v}\\ &= \frac{\qty{20}{\meter}}{0.95}\\ &\approx \qty{21.05}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}l_E &= \frac{\lambda}{2}\\ &= \frac{1}{2} \cdot \frac{c}{f}\\ \Rightarrow f &= \frac{1}{2} \cdot \frac{c}{l_E}\\ &\approx \frac{1}{2} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{21.05}{\meter}}\\&\approx \qty{7.125}{\mega\hertz}\end{split}$
</fragment>
</right>

---

[question:AG104]

---

#### Solution
<left>
* given: $f = \qty{7.1}{\mega\hertz}$
* given: $k_v = 0.95$
</left>
<right>
* given: $\frac{\lambda}{4}$ ground plane
* required: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{\lambda}{4}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &\approx \frac{1}{4} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{7.1}{\mega\hertz}}\\ &\approx \frac{1}{4} \cdot \qty{42.25}{\meter}\\ &\approx \qty{10.56}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0.95 \cdot \qty{10.56}{\meter}\\ &\approx \qty{10.04}{\meter}\end{split}$
</fragment>
</right>

---

[question:AG105]

---

#### Solution
<left>
* given: $f = \qty{14.2}{\mega\hertz}$
* given: $k_v = 0.97$
</left>
<right>
* given: $\frac{5}{8}\lambda$ vertical antenna
* required: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{5}{8}\lambda\\ &= \frac{5}{8} \cdot \frac{c}{f}\\ &\approx \frac{5}{8} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{14.2}{\mega\hertz}}\\ &\approx \frac{5}{8} \cdot \qty{21.13}{\meter}\\ &\approx \qty{13.20}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0.97 \cdot \qty{13.20}{\meter}\\ &\approx \qty{12.80}{\meter}\end{split}$
</fragment>
</right>

---

### Cause of the shortening factor

* Conductors are not infinitely thin  
* Additional capacitance between the conductor and its surroundings  
* Affects the effective electrical length of the antenna  

---

[question:AG202]

---

### Lengthening factor of loop antennas

* Difference from the shortening factor  
* Leads to an apparent lengthening of the antenna  

<note>
A lengthening factor does <u>not</u> mean that the wave travels *faster than light*. It is the phase velocity, not the group velocity.
</note>

---

[question:AG118]

---

#### Solution
<left>
* given: $f = \qty{7.1}{\mega\hertz}$
* given: $k_v = 1.02$
</left>
<right>
* given: delta loop
* required: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \lambda\\ &= \frac{c}{f}\\ &= \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{7.1}{\mega\hertz}}\\ &\approx \qty{42.23}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 1.02 \cdot \qty{42.23}{\meter}\\ &\approx \qty{43.10}{\meter}\end{split}$
</fragment>
</right>

---

### Velocity factor of open-wire lines

* The wave is between the conductors  
* The skin effect prevents deep penetration into the metal  
* Velocity factor approximately $1$ (like propagation in free space)  

---

[question:AG313]

---

### Velocity factor of coaxial cables

* The wave is in the dielectric between the conductors
* Example for polyethylene: $\epsilon_\mathrm{r} = 2.29$  
* The skin effect prevents deep penetration into the metal  
* The geometry of the cable has hardly any influence  
* Calculating the velocity factor:  

<fragment>
$v_\mathrm{k} = \dfrac{1}{\sqrt{\epsilon_\mathrm{r}}}$
</fragment>

---

[question:AG315]

---

[question:AG316]

---
#### Solution
* given: $f = \qty{145}{\mega\hertz}$
* given: $k_v = 0.66$
* required: $l_G$

<left>
<fragment>
$\begin{split}l_E &= \lambda\\ &= \frac{c}{f}\\ &\approx \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{145}{\mega\hertz}}\\ &\approx \qty{2.07}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0.66 \cdot \qty{2.07}{\meter}\\ &\approx \qty{1.37}{\meter}\end{split}$
</fragment>
</right>