<left>
[picture:978:a_swr:Standing wave]
</left>
<right>
* The standing wave ratio (SWR) can often be stated directly from the feed-point impedance of an antenna
* For a pure resistance (no inductive or capacitive components), the SWR is calculated from the ratio of the load resistance to the characteristic impedance of the cable (so that SWR ≥ $\num{1}$)
</right>

---

* Example: an antenna of $\qty{100}{\ohm}$ on a $\qty{50}{\ohm}$ cable gives an SWR of $\num{2}$, while one of $\qty{10}{\ohm}$ gives an SWR of $\num{5}$
* Remember: the impedance of a folded dipole is just under $\qty{300}{\ohm}$

---
[question:AG405]
---
#### Solution
* given: $Z = \qty{75}{\ohm}$
* given: $R_2 \approx \qty{300}{\ohm}$ impedance of the folded dipole
* required: $s$

<fragment>
$s = \frac{R_2}{Z} = \frac{\qty{300}{\ohm}}{\qty{75}{\ohm}} = 4$
</fragment>
---

### Effect of line loss on the standing wave ratio

* Line loss reduces both the forward and the reflected power
* Even if $\qty{100}{\percent}$ of the energy is reflected at the end of the cable, a lower (better) SWR can be measured at the transmitter
* Example: if half the power is lost in each direction, there and back, only a quarter of the original power remains – this corresponds to a measured SWR of $\num{3}$ ($\qty{25}{\percent}$ reflected power)

---
[question:AG402]
---
[question:AG403]
---

### Effect of line loss on the measured SWR

* With a line loss of $\qty{5}{\dB}$ in each direction, there and back ($\qty{10}{\dB}$ in total), the reflected power is only a tenth of the forward power
* The measured SWR can be calculated with the formula:
  
<fragment>
$s = \frac{\sqrt{P_\mathrm{v}}+\sqrt{P_\mathrm{r}}}{\sqrt{P_\mathrm{v}}-\sqrt{P_\mathrm{r}}}$
</fragment>

---
[question:AG404]
---

#### Solution
* given: $P_V = \qty{10}{\watt}$
* given: $a = \qty{5}{\dB}$
* required: $s$

<fragment>
Attenuation over the whole cable, there and back: $\qty{10}{\dB}$
$P_R = \qty{-10}{\dB} \cdot P_V = \dfrac{\qty{10}{\watt}}{10} = \qty{1}{\watt}$
</fragment>
<fragment>
$s = \dfrac{\sqrt{P_\mathrm{v}}+\sqrt{P_\mathrm{r}}}{\sqrt{P_\mathrm{v}}-\sqrt{P_\mathrm{r}}} = \dfrac{\sqrt{\qty{10}{\watt}}+\sqrt{\qty{1}{\watt}}}{\sqrt{\qty{10}{\watt}}-\sqrt{\qty{1}{\watt}}} = 1.92$
</fragment>
