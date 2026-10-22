## Wave impedance and field strengths
* Wave impedance in a vacuum:
* $Z_{F0} = \sqrt{\dfrac{\mu_0}{\varepsilon_0}}$
* $\mu_0$ is the magnetic constant, $\varepsilon_0$ the electric constant  
* The magnetic field strength is calculated from $\mu_0$, the magnetic flux density and the magnetisation  

---

* In a medium (e.g. air):
* $Z_{F} = \sqrt{\dfrac{\mu}{\varepsilon}}$
* The electric and magnetic field strengths depend on the wave impedance of the medium

---
[question:AK102]

---
### Power at the feed point of the antenna

* The power at the antenna input is the transmitter power minus the cable loss  
* Cable losses are taken into account as an attenuation factor (e.g. $\qty{10}{\dB}$ → $\num{0.1}$)  
* Formula: $P_{Ant} = D \cdot P_{Sender}$

---
[question:AK104]

---
## Maximum transmit power under the BEMFV

* The safety distance must lie in the far field:  

<fragment>
$d > \dfrac{\lambda}{2\pi}$  
</fragment>

---

[question:AK107]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $g_d = \qty{6}{\dBd}$
* given: $E = \qty{28}{\volt\per\meter}$
</left>
<right>
* given: $d = \qty{5}{\meter}$
* required: $P_S$
</right>

<fragment>
<left>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{d}\\ \Rightarrow P_{EIRP} &= \frac{(E \cdot d)^2}{\qty{30}{\ohm}}\\ &= \frac{(\qty{28}{\volt\per\meter} \cdot \qty{5}{\meter})^2}{\qty{30}{\ohm}}\\ &\approx \qty{653}{\watt}\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d - a + 2.15dB}{\qty{10}{\dB}}}\\ \Rightarrow P_S &= \frac{P_{EIRP}}{10^{\frac{g_d - a + 2.15dB}{\qty{10}{\dB}}}}\\ &= \frac{\qty{653}{\watt}}{10^{\frac{\qty{6}{\dBd} - \qty{0}{\dB} + 2.15dB}{\qty{10}{\dB}}}}\\ &\approx \frac{\qty{653}{\watt}}{6.53}\\ &= \qty{100}{\watt}\end{split}$
</right>
</fragment>

---

[question:AK113]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $g_i = \qty{12.15}{\dBi}$
* given: $P_A = \qty{250}{\watt}$
</left>
<right>
* given: $d = \qty{30}{\meter}$
* required: $E$
</right>

<fragment>
<left>
$\begin{split}G_i &= 10^{\frac{g_i}{\qty{10}{\dB}}}\\ &= 10^{\frac{\qty{12.15}{\dBi}}{\qty{10}{\dB}}}\\ &\approx 16.4\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_A \cdot G_i}}{d}\\ &= \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{250}{\watt} \cdot 16.4}}{\qty{30}{\meter}}\\ &\approx \frac{\qty{350}{\volt}}{\qty{30}{\meter}}\\ &\approx \qty{11.7}{\volt\per\meter}\end{split}$
</right>
</fragment>

---

[question:AK114]

--- style="font-size: smaller;"
#### Solution
* given: $P_{ERP} = \qty{100}{\watt}$
* given: $d = \qty{100}{\meter}$
* required: $E$

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_{ERP} \cdot 1.64\\ &= \qty{100}{\watt} \cdot 1.64\\ &= \qty{164}{\watt}\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{d}\\ &= \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{164}{\watt}}}{\qty{100}{\meter}}\\ &\approx \qty{0.7}{\volt\per\meter}\end{split}$
</right>
</fragment>

---

[question:AK115]

--- style="font-size: smaller;"
#### Solution
* given: $P_{ERP} = \qty{100}{\watt}$
* given: $d = \qty{100}{\meter}$
* required: $E$

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_{ERP} \cdot 1.64\\ &= \qty{100}{\watt} \cdot 1.64\\ &= \qty{164}{\watt}\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{d}\\ &= \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{164}{\watt}}}{\qty{100}{\meter}}\\ &\approx \qty{0.7}{\volt\per\meter}\end{split}$
</right>
</fragment>
