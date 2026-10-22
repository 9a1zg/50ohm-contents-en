In Classes N and E we met the SWR and the corresponding formulas for the forward and reflected power. In many cases the standing wave ratio can simply be stated if the feed-point impedance of an antenna is known. Provided an antenna (or dummy load) behaves neither inductively nor capacitively, that is, it presents a pure resistance ($R_a$), the standing wave ratio follows from the ratio of the load resistance to the characteristic impedance of the line, with numerator and denominator chosen so that the SWR is greater than or equal to one.

Figure [ref:a_swr] shows the voltage distribution of a standing wave on a line. At certain points the voltage reaches a maximum $U_\mathrm{max}$, at others a minimum $U_\mathrm{min}$. The distance between two adjacent voltage maxima, or between two adjacent voltage minima, is $\frac{\lambda}{2}$ in each case. The standing wave ratio can also be determined from the ratio of the maximum to the minimum voltage:

Expressed mathematically, this means:

$s = \frac{U_\mathrm{max}}{U_\mathrm{min}} = \begin{cases} \dfrac{R_a}{Z}, & \text{for } R_a > Z, \\[6pt] 1, & \text{for } R_a = Z, \\[6pt] \dfrac{Z}{R_a}, & \text{for } R_a < Z. \end{cases}$

<margin>
[picture:978:a_swr:Standing wave]
</margin>

An antenna with a feed-point impedance of $\qty{100}{\ohm}$, fed with a $\qty{50}{\ohm}$ cable, gives a standing wave ratio of $\num{2}$, since the feed-point impedance is twice as large. An antenna with a feed-point impedance of $\qty{10}{\ohm}$ would have a standing wave ratio of $\num{5}$, since the characteristic impedance of the line is five times as large.

To answer the following question we also need to remember that the impedance of a folded dipole is roughly $\qtyrange{240}{300}{\ohm}$.

[question:AG405]
[question:AI403]

A deceptive effect is the influence of line loss on the standing wave ratio. The greater the losses of a line, the smaller (that is, "better") the standing wave ratio on that line can turn out to be. This is because a lossy line reduces both the forward and the reflected power. Even if no antenna is connected at the end of a line (open circuit or short circuit), so that $\qty{100}{\percent}$ of the energy is reflected there and the standing wave ratio there is $\infty$, a considerably better standing wave ratio can be measured at the other end. If, for example, half the power is lost on the way there and half again on the way back, the energy is reduced to a quarter ($\frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4}$). Accordingly, an SWR meter at the transmitter end of the cable shows a standing wave ratio of $\num{3}$, which corresponds to $\qty{25}{\percent}$ reflected power, although $\qty{100}{\percent}$ is reflected at the end – but only $\qty{25}{\percent}$ arrives back at the SWR meter.

[question:AG402]
[question:AG403]

With a line loss of $\qty{5}{\dB}$ and complete reflection at the end of the cable, e.g. because the antenna has been disconnected, we even measure a surprisingly good SWR, although no antenna at all is connected! We can calculate this as follows:

$s = \frac{\sqrt{P_\mathrm{v}}+\sqrt{P_\mathrm{r}}}{\sqrt{P_\mathrm{v}}-\sqrt{P_\mathrm{r}}}$

The following question can be calculated with this, provided we bear in mind that the reflected wave measured is only a tenth of the energy of the forward wave: $\qty{5}{\dB}$ attenuation on the way there and $\qty{5}{\dB}$ attenuation on the way back, corresponding to $\qty{10}{\dB}$ attenuation in total. So in this case $P_\mathrm{r}$ is only a tenth of $P_\mathrm{v}$.

[question:AG404]
