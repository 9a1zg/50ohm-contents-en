## Characteristic impedance of a twin feeder

* The characteristic impedance $Z$ depends on the ratio of twice the centre-to-centre spacing of the conductors ($a$) to the diameter of the conductors $d$, and on the dielectric
* Formula from the formula sheet, with $\epsilon_\mathrm{r}$ as the relative permittivity:

<fragment>
$Z = \dfrac{\qty{120}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{2 \cdot a}{d}\right)}$
</fragment>

---
[question:AG305]
---
#### Solution
* given: $d = \qty{2}{\milli\meter}$
* given: $a = \qty{20}{\centi\meter}$
* given: $\epsilon_\mathrm{r} \approx 1$ for air
* required: $Z$

<fragment>
$\begin{split}Z &= \dfrac{\qty{120}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{2 \cdot a}{d}\right)}\\ &= \dfrac{\qty{120}{\ohm}}{\sqrt{1}} \cdot \ln{\left(\dfrac{2 \cdot \qty{200}{\milli\meter}}{\qty{2}{\milli\meter}}\right)}\\ &\approx \qty{635}{\ohm}\end{split}$
</fragment>
---
## Characteristic impedance of a coaxial line

* The characteristic impedance $Z$ depends on the ratio of the inside diameter of the outer conductor ($D$) to the diameter of the inner conductor ($d$), and on the dielectric
* Formula from the formula sheet, with $\epsilon_\mathrm{r}$ as the relative permittivity

<fragment>
$Z = \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\dfrac{D}{d}}$
</fragment>

---
[question:AG306]
----
#### Solution
* given: $D = \qty{5}{\milli\meter}$
* given: $d = \qty{1}{\milli\meter}$
* given: $\epsilon_\mathrm{r} \approx 1$ for air
* required: $Z$

<fragment>
$\begin{split}Z &= \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{D}{d}\right)}\\ &= \dfrac{\qty{60}{\ohm}}{\sqrt{1}} \cdot \ln{\left(\dfrac{\qty{5}{\milli\meter}}{\qty{1}{\milli\meter}}\right)}\\ &\approx \qty{97}{\ohm}\end{split}$
</fragment>
---
[question:AG307]
---
#### Solution
* given: $d = \qty{0.7}{\milli\meter}$
* given: $D = \qty{4.4}{\milli\meter}$
* given: $\epsilon_\mathrm{r} = 2.29$
* required: $Z$

<fragment>
$\begin{split}Z &= \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{D}{d}\right)}\\ &= \dfrac{\qty{60}{\ohm}}{\sqrt{2.29}} \cdot \ln{\left(\dfrac{\qty{4.4}{\milli\meter}}{\qty{0.7}{\milli\meter}}\right)}\\ &\approx \qty{75}{\ohm}\end{split}$
</fragment>
---
### Matching of coaxial lines

* If a component or an antenna is connected that has exactly the characteristic impedance of the line, the line is said to be matched
* When the line is matched, waves are not reflected back at the termination

---
[question:AG304]