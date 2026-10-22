There is an approximation formula for calculating the safety distance. We find it on the formula sheet: 

$ E = \frac{\sqrt{\qty{30}{\ohm}\cdot P_\text{EIRP}}}{d} $

It can quickly be rearranged for the safety distance $d$: 

$ d = \frac{\sqrt{\qty{30}{\ohm}\cdot P_\text{EIRP}}}{E} $

The formula sheet also notes that the formula above only applies to calculations in the far field (or radiating near field), from $ d > \frac{\lambda}{2\pi} $. We will discuss why this is so in more detail in Class A. For calculating the safety distance, however, it is important that we are in the far field (or radiating near field) and that this condition is met.

<indepth>
The far field of a radiation source is the region in which the vectors of the electric field strength ($E$) and the magnetic field strength ($H$) are perpendicular to each other and show no phase difference. 

The boundary between the far field and the near field depends primarily on the wavelength. According to the [Explanations of the BEMFV](https://50ohm.de/ebemfv), the far field forms at a distance of about $4\cdot\lambda$. 

The near field is divided into the *reactive* and the *radiating near field*. Conveniently, the formula for the far field can nevertheless be used in the radiating near field. This is because the approximation formula gives very conservative estimates there, that is, the actual field strengths are lower than the calculated ones. You are on the safe side. 
  
With the formula $ d > \frac{\lambda}{2\pi} $ we therefore make sure that we are outside the *reactive near field*.
</indepth>

%TODO Applet basteln: https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-wellen/versuche/dipolstrahlung-animation

The following question addresses exactly this point:

[question:EK105]

For $\qty{3.5}{\mega\hertz}$ the far field (radiating near field) only begins at $\qty{13.64}{\meter}$.

 $\begin{split} d &> \frac{\lambda}{2 \cdot \pi}\\ d &> \frac{\qty{85.7}{\meter}}{2 \cdot \pi}\\ d &> \qty{13.64}{\meter}\end{split}$
 
The distance of $\qty{3.65}{\meter}$ that was determined lies well inside the reactive near field and is therefore invalid. Instead of the far-field approximation formula, another method must be chosen. Possible methods are measurements of the E- and H-field components, simulations or near-field calculations.

To answer the following question, you have to calculate where the far field (radiating near field) begins for the $\qty{160}{\meter}$ and $\qty{80}{\meter}$ bands.

[question:EK106]

For $\qty{160}{\meter}$: $d > \frac{\qty{160}{\meter}}{2\pi} = \qty{25.5}{\meter}$
 
For $\qty{80}{\meter}$: $d > \frac{\qty{80}{\meter}}{2\pi} = \qty{12.7}{\meter}$

The calculation is invalid if the distance is less than $\qty{25.5}{\meter}$ for $\qty{160}{\meter}$ and less than $\qty{12.7}{\meter}$ for $\qty{80}{\meter}$.

%%%%

In the following question, a real safety distance now has to be calculated for the first time. 

[question:EK108]

First we have to calculate the radiated power as $P_\textrm{EIRP}$. We also notice that the antenna gain is given in $\unit{\dBd}$. For this we again use the formula from the formula sheet:

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_d-a+\qty{2.15}{\dB}}{\qty{10}{\dB}}} = \qty{100}{\watt} \cdot 10^{\frac{\qty{7.5}{\dBd}-\qty{1.5}{\dB}+\qty{2.15}{\dB}}{\qty{10}{\dB}}} \approx \qty{653}{\watt}$

The sum of the gains and losses of the whole antenna system is the antenna gain of $\qty{7.5}{\dBd}$, minus the cable loss of $\qty{1.5}{\dB}$, plus the gain of $\qty{2.15}{\dBi}$ for referring it to the isotropic radiator (the antenna gain is relative to the dipole).

Alternatively, as in the previous chapters, we can determine the corresponding factors for the gains and the loss.
$\qty{7.5}{\dB} - \qty{1.5}{dB} = \qty{6}{\dB}$, which corresponds to a factor of $\num{4}$. The factor for $\qty{2.15}{\dBi}$ is $\num{1.64}$.

$P_\textrm{EIRP} = \qty{100}{\watt} \cdot 4 \cdot 1.64 = \qty{656}{\watt}$

---

The results of the two methods should really be the same. They differ slightly, however. This is the result of rounding the two factors. The power calculated with the rounded factors is nevertheless accurate enough to answer the question correctly. So we put this value into the distance formula:

$ d = \frac{\sqrt{\qty{30}{\ohm}\cdot P_\text{EIRP}}}{E} = \frac{\sqrt{\qty{30}{\ohm}\cdot \qty{656}{\watt}}}{\qty{28}{\volt\per\meter}} \approx \qty{5}{\meter}  $

The safety distance of $\qty{5}{\meter}$ was determined with the formula for the far field. It is therefore only valid if it also lies in the far field (or radiating near field). This can be checked quickly, as above.

$\begin{split} d &> \frac{\lambda}{2\pi}\\ d &> \frac{\qty{10}{\meter}}{2\pi}\\ d &> \qty{1.6}{\meter} \end{split}$

The calculated safety distance of $\qty{5}{\meter}$ is greater than $\qty{1.6}{\meter}$ and clearly lies in the far field (or radiating near field). The calculation is therefore valid. The correct answer is $\qty{5}{\meter}$.

<indepth>
The table gives a factor of $\num{4}$ for $\qty{6}{\dB}$. This is a rounded value; the exact value is $\num{3.981071706}$. That is where the rounding error comes from.
</indepth>
