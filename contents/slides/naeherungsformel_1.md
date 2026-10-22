## Approximation formula for field strength
<left>
* Calculating the electric field strength
* At a distance from a radiator
* For a given power and gain
* Only valid in free space <br/> ($d > \frac{\lambda}{2\pi}$)
</left>
<right>
$\begin{split} E &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_A \cdot G_i}}{d}\\ &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_{\textrm{EIRP}}}}{d} \end{split}$
</right>

---
## Approximation formula for distance
<left>
* For a given field strength
* Rearrange for $d$
</left>
<right>
$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_A \cdot G_i}}{E}\\ &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_{\textrm{EIRP}}}}{E} \end{split}$
</right>

---
[question:EK108]
---
### Solution
<left>
* given: $E = \qty{28}{\volt\per\meter}$
* given: $g_d = \qty{7.5}{\dBd}$
* given: $P_S = \qty{100}{\watt}$
</left>
<right>
* given: $a_{\textrm{Kabel}} = \qty{1.5}{\dB}$
* required: $P_{\textrm{EIRP}}$
* required: $d$
</right>

<left>
<fragment>
$\begin{split} P_{\textrm{EIRP}} &= P_S \cdot 10^{\frac{g_d - a + \qty{2.15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{100}{\watt} \cdot 10^{\frac{\qty{7.5}{\dBd} - \qty{1.5}{\dB} + \qty{2.15}{\dB}}{\qty{10}{\dB}}}\\ &\approx \qty{100}{\watt} \cdot 6.5\\ &= \qty{650}{\watt} \end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_{\textrm{EIRP}}}}{E}\\ &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{650}{\watt}}}{\qty{28}{\volt\per\meter}}\\ &\approx \qty{5}{\meter} \end{split}$
</fragment>
</right>

---
### Bonus question

Isn't the calculated $\qty{5}{\meter}$ in the near field for the $\qty{10}{\meter}$ band in the question?

<fragment>
$\begin{split} d &> \frac{\lambda}{2\pi}\\ \qty{5}{\meter} &> \frac{\qty{10}{\meter}}{2\pi}\\ \qty{5}{\meter} &\gtrapprox \qty{1.6}{\meter} \end{split}$
</fragment>

---
[question:EK106]
---
### Solution

* The safety distance for the protection of persons is only valid in free space
* $d > \frac{\lambda}{2\pi}$
* $\qty{160}{\meter}$ band: $\qty{25.5}{\meter}$
* $\qty{80}{\meter}$ band: $\qty{12.7}{\meter}$

---
[question:EK105]

<note>
What we calculated before lies in the near field
</note>

