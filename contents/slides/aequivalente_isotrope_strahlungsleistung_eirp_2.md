
* In the calculation, only take into account the energy that arrives at the antenna
* Subtract losses $a$ due to cables, connectors or other components
* Only then multiply by the gain factor
* Various general formulas for ERP and EIRP follow

---
### ERP

Known from Class N:

$P_{\mathrm{ERP}} = (P_{\mathrm{Sender}} - P_{\mathrm{Verluste}}) \cdot G_{\mathrm{Antenne}}$

<fragment>
To be used when calculating in $\unit{\dB}$:

$P_{\mathrm{ERP}} = P_{\mathrm{Sender}} - a + g_d$
</fragment>

<fragment>
From the formula sheet, with conversion from $\unit{\dB}$ to a power ratio:

$P_{\mathrm{ERP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a}{\qty{10}{\dB}}}$
</fragment>

---
### EIRP

Converting ERP to EIRP:

$P_{\mathrm{EIRP}} = P_{\mathrm{ERP}} + \qty{2.15}{\dB}$

<fragment>
From the formula sheet, with conversion from $\unit{\dB}$ to a power ratio:

$P_{\mathrm{EIRP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a + \qty{2.15}{\dB}}{\qty{10}{\dB}}}$
</fragment>

<fragment>
If the gain is given in $\unit{\dBi}$:

$P_{\mathrm{EIRP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{\qty{10}{\dB}}}$
</fragment>

---
[question:EG501]
---
[question:EG502]
---
## Fixed amateur radio installation

Under Section 9 BEMFV, a fixed amateur radio installation must be notified to the BNetzA if a radiated power of $\qty{10}{\watt}$ EIRP is exceeded.
---
[question:EG503]
--- style="font-size: smaller;"
### Solution

* given: $P_{\mathrm{Sender}} = \qty{250}{\milli\watt}$
* given: $g_i = \qty{26}{\dBi}$
* given: $a = \qty{0}{\dB}$
* required: $P_{\mathrm{EIRP}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{\qty{10}{\dB}}}\\ &= \qty{250}{\milli\watt} \cdot 10^{\frac{\qty{26}{\dBi}}{\qty{10}{\dB}}}\\ &= \qty{250}{\milli\watt} \cdot 398\\ &\approx \qty{100}{\watt} \end{split}$
</fragment>

---
[question:EG504]

<note>
* Same method as before
</note>
---
[question:EG511]
--- style="font-size: smaller;"
### Solution

* given: $P_{\mathrm{EIRP}} = \qty{10}{\watt}$
* given: $g_i = \qty{5.15}{\dBi}$
* given: $a = \qty{0}{\dB}$
* required: $P_{\mathrm{Sender}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{\qty{10}{\dB}}}\\ \Rightarrow P_{\mathrm{Sender}} &= \dfrac{P_{\mathrm{EIRP}}}{10^{\frac{g_i - a}{\qty{10}{\dB}}}}\\ &= \dfrac{\qty{10}{\watt}}{10^{\frac{\qty{5.15}{\dBi}}{\qty{10}{\dB}}}}\\ &\approx \frac{\qty{10}{\watt}}{3.27} \approx \qty{3}{\watt} \end{split}$
</fragment>

<note>
There are several ways to the answer. You can also calculate directly with logarithms.
</note>
---
[question:EG505]

<note>
Gain: $\qty{10}{\dB}$, so also a factor of $\num{10}$
</note>
---
[question:EG507]

<note>
* A loss of $\qty{10}{\dB}$ is a factor of $\num{10}$, so $\qty{10}{\watt}$ ERP arrives at the antenna
* The factor from ERP to EIRP is $\num{1.64}$
</note>
---
[question:EG506]

<note>
* The dipole's gain of $\qty{2.15}{\dBi}$ exactly cancels out the cable losses
</note>
---

* If the antenna gain is given relative to the dipole, we must also take the gain of the dipole into account when the EIRP is asked for.

---
[question:EG508]
---
### Solution

* given: $P_{\mathrm{Sender}} = \qty{5}{\watt}$
* given: $g_d = \qty{5}{\dBd}$
* given: $a = \qty{2}{\dB}$
* required: $P_{\mathrm{EIRP}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a + \qty{2.15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{5}{\watt} \cdot 10^{\frac{\qty{5}{\dBd} - \qty{2}{\dB} + \qty{2.15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{5}{\watt} \cdot 3.27\\ &\approx \qty{16.4}{\watt} \end{split}$
</fragment>

---
[question:EG509]

<note>
Same method as before
</note>
---
[question:EG510]

<note>
Same method as before
</note>