For sinusoidal AC signals, power is calculated from the RMS values of current and voltage. So you must not simply use the peak-to-peak voltage $U_\text{SS}$, or the peak voltage $\hat{U}$, in their place.

<margin>
[picture:834:a_wechselstrom_leistung:RMS values for calculating power]
</margin>

This gives the following for calculating power:
$P_\text{Wechselstrom} = U_\text{eff} \cdot I_\text{eff} = \dfrac{{U_\text{eff}}^2}{R} = I_\text{eff}^2 \cdot R$


For sinusoidal signals, however, the following also applies:

$U_\text{eff} = \dfrac {\hat{U}} {\sqrt{2}} = \dfrac {U_\text{SS}} {2 \cdot \sqrt{2}}$ 
$I_\text{eff} = \dfrac {\hat{I}} {\sqrt{2}} = \dfrac {I_\text{SS}} {2 \cdot \sqrt{2}}$ 

For sinusoidal signals, this gives the following relationships, which also allow you to calculate with peak values and peak-to-peak values:

$\begin{split} P_\text{Wechselstrom} &=  U_\text{eff} \cdot I_\text{eff} \\ &= \frac{\hat{U}\cdot\hat{I}}{\sqrt{2}\cdot\sqrt{2}} = \frac{\hat{U} \cdot \hat{I}}{2} \\ &= \frac{U_\text{eff}^2}{R} = \left(\frac{\hat{U}}{\sqrt{2}}\right)^2 \cdot \frac{1}{R} = \frac{\hat{U}^2}{2 \cdot R} \\ &= I_\text{eff}^2 \cdot R = \left(\frac{\hat{I}}{\sqrt{2}}\right)^2 \cdot R = \frac{\hat{I}^2\cdot R}{2} \end{split}$

With these considerations, the following question is very easy to solve ($I_\mathrm{max}$ is just another name for $\hat{I}$):

[question:AB301]

In amateur radio we deal with voltages of different frequencies (e.g. kilohertz or gigahertz) and waveforms (square-wave voltage, sinusoidal voltage, DC voltage). They can also be distorted, rather than being, for example, a pure sine-wave voltage. These different voltages produce different electric currents in a circuit. In principle, you would now need different instruments to measure this range of electric currents with reasonable accuracy. 

In amateur radio, therefore, a *thermocouple converter* is often used.
It makes use of the fact that a current flowing through a conductor wire heats it up (cf. resistance of wires). The more current flows, the warmer the wire becomes. The heating is therefore proportional to the current. The thermocouple converter measures this heating and displays it as a current.  Note that with this measuring method we obtain the *RMS value* of the current. The advantage is that the current can be determined almost *independently* of the waveform or frequency. The thermocouple converter can therefore cover a wide range of signals. 

[question:AI105]
