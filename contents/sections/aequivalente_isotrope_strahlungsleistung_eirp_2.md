In Class N we have already met the isotropic radiator (see Figure [ref:e_Kugelstrahler]). The isotropic radiator is not a real antenna; it is a physical model of a radiator that radiates energy equally in all directions in space. 

The equivalent isotropically radiated power (EIRP) of a real antenna is relative to the isotropic radiator. In other words, the radiated power of a real antenna is compared with the radiated power of the isotropic radiator. For the radiated power, only the energy that actually arrives at the antenna is relevant. In the real world, cable loss etc. means that not all of the transmitter's power can be delivered to the antenna. This lost power must not be included in the calculation of the radiated power. The antenna gain in the preferred direction is, of course, part of the calculation. As a formula, this means:

$P_\mathrm{EIRP} = (P_\mathrm{Sender} - P_\mathrm{Verluste}) \cdot G_\mathrm{Antenne}$

Here $G_\mathrm{Antenne}$ represents the antenna gain. EIRP is therefore the product of the power supplied directly to the antenna and its gain in a given direction, relative to the isotropic radiator.

<margin>
[picture:751:e_Kugelstrahler:Isotropic radiator at the centre of a sphere, producing the same radiated power at every point on the surface of the sphere]
</margin>

<tip>
Before the examination you should get thoroughly familiar with your calculator. The calculations and formulas in the various questions should be practised again and again, so that in the examination you can handle the calculator and the steps of the calculation with confidence.
</tip>

[question:EG501]

In the next question, pay close attention to the arithmetic signs. The losses are *subtracted* from the transmit power and the result is then *multiplied* by the gain factor ($G_\mathrm{Antenne}$). Since the EIRP is to be calculated, it must be relative to the isotropic radiator.

[question:EG502]

---

In the chapter on decibels we learnt that it makes sense to calculate with dB values, since this makes many calculations much simpler. In decibels, gains and losses can simply be added and subtracted respectively. Figure [ref:e_verstaerkung_daempfung] shows a radio installation with several stages that amplify or attenuate. The total gain of this installation is obtained by adding the individual contributions: $\qty{-2}{\dB} + \qty{6}{\dB} - \qty{3}{\dB} + \qty{2}{\dB} = \qty{3}{\dB}$, which corresponds to a power ratio of $\num{2}$.

<margin>
[picture:439:e_verstaerkung_daempfung:Gains and losses in a radio installation]
</margin>

---

The following questions require the EIRP to be calculated. This can be done either directly with a formula, or – with a little practice – the problems can be solved entirely in your head. In what follows we will therefore usually show both approaches.

The formula for calculating the EIRP is taken from the formula sheet and reads:

$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}}$

<indepth>
The formula for $P_\mathrm{EIRP}$ is obtained by rearranging the gain formula from the formula sheet accordingly:
  
$g = 10 \cdot \log_{10}\left(\frac{P_2}{P_1}\right) \unit{\dB}$
  
Since a loss $a$ must also be taken into account, it is subtracted from the antenna gain. For $P_1$ we substitute the transmitter power $P_\mathrm{Sender}$, since it is the input power, and for $P_2$ accordingly $P_\mathrm{EIRP}$, since this is the resulting output power.

$g-a = 10 \cdot \log_{10}\left(\frac{P_\mathrm{EIRP}}{P_\mathrm{Sender}}\right) \unit{\dB} \quad\quad\quad | : \qty{10}{\dB}$
  
We divide both sides by $\qty{10}{\dB}$:
  
$\frac{g-a}{\qty{10}{\dB}} = \log_{10}\left(\frac{P_\mathrm{EIRP}}{P_\mathrm{Sender}}\right) \quad\quad\quad | 10^x$
  
Then we apply $10^x$ to both sides to remove the logarithm:
  
$10^{\frac{g-a}{\qty{10}{\dB}}} = \frac{P_\mathrm{EIRP}}{P_\mathrm{Sender}} \quad\quad\quad | \cdot P_\mathrm{Sender}$
  
Multiplying by $P_\mathrm{Sender}$ gives the formula we need:
  
$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}}$
</indepth>

Here $g_i$ is the antenna gain relative to the isotropic radiator, while $a$ is the loss in cables and antenna tuning units.

[question:EG503]

The first method uses the formula mentioned above. Since there are no power losses, the loss is $a=0$ and the formula simplifies to: 

$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}}= \qty{250}{\milli\watt} \cdot 10^{\frac{\qty{26}{\dBi}}{\qty{10}{\dB}}}= \qty{250}{\milli\watt} \cdot 398 \approx \qty{100}{\watt}$

---

The second possible method uses the fact that dB values can be "split up". In the question the antenna gain is $g = \qty{26}{\dBi}$. On the formula sheet, Table [ref:e_dezibel_leistungsfaktoren] gives an overview of the power ratios for important dB values. There is no direct entry there for $\qty{26}{\dB}$. However, since levels in decibels can be added, the value can be split up sensibly:

$\qty{26}{\dBi} = \qty{20}{\dBi} + \qty{6}{\dB}$

<margin>
| c:dB | c:≈ Power ratio |
| $\num{0}$ | $\num{1}$ |
| $\num{1.5}$ | $\sqrt{2} = 1.41$ |
| $\num{2.15}$ | $\num{1.64}$ |
| $\num{3}$ | $\num{2}$ |
| $\num{5}$ | $\sqrt{10} = 3.16$ |
| $\num{6}$ | $\num{4}$ |
| $\num{10}$ | $\num{10}$ |
| $\num{20}$ | $\num{100}$ |
[table:e_dezibel_leistungsfaktoren:Important power ratios in dB]
</margin>

For $\qty{20}{\dB}$ the table gives a power ratio of $\num{100}$, for $\qty{6}{\dB}$ a factor of $\num{4}$. This makes it very easy to calculate the equivalent isotropically radiated power:

$P_\mathrm{EIRP} = \qty{250}{\milli\watt} \cdot 100 \cdot 4 = \qty{100}{\watt}$

The correct answer is therefore $\qty{100}{\watt}$ EIRP.

For the next question we can proceed in exactly the same way as for the previous one. 

[question:EG504]

---

For many radio amateurs it is difficult to keep the necessary safety distance at a transmit power of, for example, $\qty{100}{\watt}$. In these cases QRP operation is a solution. If you keep the radiated power below the $\qty{10}{\watt}$ EIRP limit, there is no need to notify a fixed amateur radio installation under Section 9 BEMFV. Even with equipment that is not a QRP rig, the output power can be reduced to a particular value, as shown in Figure [ref:e_ausgangsleistung_ic].

<margin>
[photo:229:e_ausgangsleistung_ic:On many transceivers the output power can be set continuously or, as here on the IC-705, in small steps.]
</margin>

[question:EG511]

The vertical antenna given in this question has a gain of $g=\qty{5.15}{\dBi}$; cable losses are neglected, i.e. $a = 0$. If the antenna had no gain ($\qty{0}{\dBi}$), the transmit power would simply have to be limited to a maximum of $\qty{10}{\watt}$. The radiated power would then be only $\qty{10}{\watt}$ EIRP. But since there is an antenna gain of $\qty{5.15}{\dBi}$, the transmit power must be reduced accordingly. The transmit power must be at least $\qty{5.15}{\dB}$ lower than $\qty{10}{\watt}$.

Here again there are two possible methods. Let us start with the one using the familiar formula. In this problem, however, we are not looking for the radiated power $P_\mathrm{EIRP}$ but for the transmit power $P_\mathrm{Sender}$. We therefore have to rearrange the formula accordingly:

$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}} \quad\quad\quad | : 10^{\frac{g_i-a}{\qty{10}{\dB}}}$

This gives:

$ P_\mathrm{Sender} = \frac{P_\mathrm{EIRP}}{10^{\frac{g_i-a}{\qty{10}{\dB}}}} $

We substitute the values:

$ P_\mathrm{Sender} = \frac{\qty{10}{\watt}}{10^{\frac{\qty{5.15}{\dBi}}{\qty{10}{\dB}}}} = \frac{\qty{10}{\watt}}{3.27} \approx \qty{3.05}{\watt} $

The calculator gives $\qty{3.05}{\watt}$. Limiting the power to $\qty{3}{\watt}$ keeps you within the limit of less than $\qty{10}{\watt}$ EIRP.

The second method again works by splitting up the dB values. Looking at the value $g=\qty{5.15}{\dBi}$, you can see that it can be split up into 

$\qty{5.15}{\dBi} = \qty{3}{\dBi} + \qty{2.15}{\dB}$

and Table [ref:e_dezibel_leistungsfaktoren] gives the factor for $\qty{2.15}{\dB}$ as $\num{1.64}$. The maximum transmit power is therefore:

$P_\mathrm{Sender} = \frac{\qty{10}{\watt}}{2\cdot 1.64} = \frac{\qty{10}{\watt}}{3.28} \approx \qty{3}{\watt}$

As expected, we arrive at the same result. With $\qty{3}{\watt}$ you are on the safe side.

The next question could again be solved with the formula sheet by substituting $a=\qty{1}{\dB}$, but it is quite easy to do in your head. 

[question:EG505]

As described at the very beginning of this section, the radiated power EIRP takes into account the antenna gain ($\qty{11}{\dBi}$) and the power that actually arrives at the antenna. The transmit power is attenuated by $\qty{1}{\dB}$ in the cable, so the antenna system as a whole has an actual gain of $\qty{10}{\dBi}$. In our Table [ref:e_dezibel_leistungsfaktoren] from the formula sheet, the factor given for $\qty{10}{\dB}$ is $\num{10}$. The transmit power of $\qty{100}{\watt}$ becomes a radiated power of $\qty{1000}{\watt}$.

For the next question, note that a dipole antenna is used. This one, too, can easily be worked out in your head.

[question:EG506]

The gain of a dipole antenna relative to the isotropic radiator is $\qty{2.15}{\dB}$. This corresponds to a factor of $\num{1.64}$. This is also given on the formula sheet:

$P_\mathrm{EIRP} = P_\mathrm{ERP} + \qty{2.15}{\dB}$

or, as a factor:

$P_\mathrm{EIRP} = P_\mathrm{ERP} \cdot 1.64$

Here $P_\mathrm{ERP}$ represents the radiated power relative to the dipole. 

The gain of the dipole is $\qty{2.15}{\dBi}$, which here is exactly equal to the cable loss in the question. The two therefore cancel each other out. The dipole antenna radiates $\qty{75}{\watt}$ EIRP.

In the next question, too, the antenna given is a dipole. 

[question:EG507]

We are looking for the equivalent isotropically radiated power $P_\mathrm{EIRP}$. First the cable loss must be taken into account. A loss of $\qty{10}{\dB}$ corresponds to a power ratio of $\num{0.1}$. With this attenuation factor and the dipole's antenna gain factor of $\num{1.64}$, the radiated power can then be calculated.

$P_\mathrm{EIRP} = \qty{100}{\watt} \cdot 0.1 \cdot 1.64 = \qty{16.4}{\watt}$


For the next question, too, there is a formula on the formula sheet that can be applied directly. Since we have a directional antenna whose gain is given relative to the dipole (ERP), $\qty{2.15}{\dB}$ must also be added to calculate $P_\mathrm{EIRP}$:

$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_d-a+\qty{2.15}{\dB}}{\qty{10}{\dB}}}$

[question:EG508]

---

Substituting into the formula solves the question quickly. But here, too, it can be done in your head. Let us work out the total gain of the system and split it up accordingly again:

$\qty{-2}{\dB} + \qty{5}{\dB} + \qty{2.15}{\dB} = \qty{3}{\dB} + \qty{2.15}{\dB}$ 

Now we can read the factors from the table again:

$P_\mathrm{EIRP} = \qty{5}{\watt} \cdot 2 \cdot 1.64 = \qty{16.4}{\watt}$

The next question can be solved in the same way. You only have to note that the gain is given relative to the dipole. 

[question:EG509]

We again work out the total gain and split it up:

$\qty{-1}{\dB} + \qty{11}{\dB} + \qty{2.15}{\dB} = \qty{10}{\dB} + \qty{2.15}{\dB}$ 

Now we can read the factors from the table again:

$P_\mathrm{EIRP} = \qty{0.6}{\watt} \cdot 10 \cdot 1.64 = \qty{9.8}{\watt}$

In the next question an antenna with a gain of $\qty{0}{\dB}$ relative to the dipole is given. That simply means that this antenna is a dipole. 

[question:EG510]

Here, too, the formula from the formula sheet can be used:

$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_d-a+\qty{2.15}{\dB}}{\qty{10}{\dB}}} = \qty{8.5}{\watt} \cdot 10^{\frac{\qty{0}{\dB}-\qty{1.5}{\dB}+\qty{2.15}{\dB}}{\qty{10}{\dB}}} = \qty{9.9}{\watt}$

You can also estimate it in your head: if you again work out the total gain of the system, it is only $\qty{0.65}{\dB}$, i.e. not even $\qty{1}{\dB}$. According to our Table [ref:e_dezibel_leistungsfaktoren], $\qty{1}{\dB}$ corresponds to a factor of $\num{1.26}$. The target value must therefore lie between $\qty{8.5}{\watt}$ and $\qty{10.71}{\watt}$. So only the $\qty{9.9}{\watt}$ is possible.