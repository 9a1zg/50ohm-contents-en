In Class N we have already met the *effective radiated power* (ERP). Unlike the EIRP, it is not relative to an isotropic radiator but to a half-wave dipole. For the calculation, only the power that actually arrives at the feed point of the antenna counts. Losses in the feeder, for example due to cable loss, must therefore be subtracted from the transmitter output power.

The effective radiated power is obtained from the power supplied to the antenna and the antenna gain in the direction under consideration:

$P_\mathrm{ERP}=P_\mathrm{Ant}\cdot G_\mathrm{d}$

Here $G_\mathrm{d}$ is the antenna gain relative to a half-wave dipole, as a linear factor.

[question:AG501]

The power at the feed point of the antenna can be determined from the transmitter output power and the loss in the feeder. To do this, the loss is converted into a linear attenuation factor $D$. With a loss of $\qty{10}{\dB}$, for example, this factor is $\num{0.1}$, so that only a tenth of the transmitter power arrives at the antenna:

$P_\mathrm{Ant}=D\cdot P_\mathrm{Sender}$

Only this power actually supplied is then multiplied by the antenna gain to calculate the ERP.

[question:AK104]

In the next question, pay close attention to the arithmetic signs. The losses are subtracted from the transmit power and the result is then multiplied by the gain factor ($G_\mathrm{Antenne}$).
Since the ERP is to be calculated, it must be relative to a half-wave dipole.

[question:AG502]

[Annex 1 to the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV)](https://50ohm.de/a1) already gives a hint to the correct answer to the next question. It specifies a maximum power of $\qty{1}{\watt}$ ERP for the $\qty{630}{\meter}$ band. A half-wave dipole for this frequency would be about $\qty{315}{\meter}$ long and is therefore hardly feasible for most radio amateurs. In practice, heavily shortened antennas are therefore mostly used, whose efficiency is considerably lower than that of a full-size half-wave dipole. An antenna gain of $\qty{-20}{\dBd}$ is therefore entirely plausible. Since the coaxial cable used is only short, its loss in this frequency range can be neglected. Now try to solve the following question. 

[question:AG503]