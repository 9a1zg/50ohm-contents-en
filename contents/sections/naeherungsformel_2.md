In Class E we have already met an approximation formula with which the safety distance from an antenna can be calculated:

$d = \frac{\sqrt{\qty{30}{\ohm}\cdot P_{\textrm{EIRP}}}}{E}$

This formula can be applied to many types of antenna if the condition

$d > \frac{\lambda}{2\pi}$

is met, that is, if we are outside the reactive near field. Below we look at where this restriction and the value of $\qty{30}{\ohm}$ that appears in the formula come from.

In general form, the approximation formula is:

$d = \frac{\sqrt{\frac{Z_0}{4\pi}\cdot P_{\textrm{EIRP}}}}{E}$

Here $Z_0$ denotes the impedance of free space. As we saw in the previous chapter, with increasing distance from the antenna it approaches the far-field value

$Z_0 \approx \qty{120\pi}{\ohm} \approx \qty{377}{\ohm}$

(see Figure [ref:a_feldwellenwiderstand]). If we put this value into the expression $\frac{Z_0}{4\pi}$, we get:

$\frac{Z_0}{4\pi} \approx \frac{\qty{120\pi}{\ohm}}{4\pi} = \qty{30}{\ohm}$

This gives the approximation formula known from Class E. At the same time it becomes clear why it must not be used in the reactive near field: there the wave impedance is not constant but depends strongly on the distance, on the type of antenna and on the direction considered. For calculations in the reactive near field, i.e. for distances $d \le \frac{\lambda}{2\pi}$, more detailed calculations, numerical simulations or measurements are therefore generally required. 

<margin>
[picture:1116:a_feldwellenwiderstand:Variation of the wave impedance across the near-field and far-field regions (logarithmic).]
</margin>

If the far-field approximation formula is applied to a dipole antenna already in the radiating near field, it generally gives a larger safety distance than is actually required. The wave impedance there is below $\qty{377}{\ohm}$, while the approximation formula works with the higher far-field value. The result is therefore conservative and on the safe side. This approach is accepted by the Federal Network Agency (Bundesnetzagentur, BNetzA).

This does not apply, however, to magnetic antennas and electrically very short antennas. Figure [ref:a_feldwellenwiderstand], for example, shows that the wave impedance of a magnetic loop antenna in the radiating near field can be well above $\qty{377}{\ohm}$. In that case the far-field approximation formula would give a safety distance that is too small. For such antennas, other procedures must therefore be used, for example special programs for near-field calculation (simulations) or measurements.

[question:AK103]

In the far field, the familiar approximation formula can be used to calculate the safety distances for the protection of persons. This often avoids elaborate measurements or simulations. In portable operation in particular, it allows a quick rough estimate of the required safety distance.