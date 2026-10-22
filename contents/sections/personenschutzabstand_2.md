Every fixed amateur radio installation with an equivalent isotropically radiated power (EIRP) of $\qty{10}{\watt}$ or more must be notified to the Federal Network Agency (Bundesnetzagentur, BNetzA) under Section 9 BEMFV. This must be done before radio operation begins. In doing so, the radio amateur must provide verification that the limits are complied with, that the safety distances required for this have been determined, and that they lie within the controlled area. Radio amateurs informally call this a *self-declaration*.

A self-declaration can only be dispensed with if the equivalent isotropically radiated power (EIRP) is *less* than $\qty{10}{\watt}$ EIRP - not $\qty{10}{\watt}$ of transmit power, nor $\qty{10}{\watt}$ ERP!

Even without an exact calculation it quickly becomes clear that the combination of $\qty{6}{\watt}$ transmit power and an antenna gain of $\qty{13}{\dBd}$ (a factor of $\num{20}$) in the following question clearly exceeds the limit of $\qty{10}{\watt}$ EIRP.

<indepth>
For practice you can calculate it anyway. We again use the formula from the formula sheet: 

$P_\mathrm{EIRP} = P_\mathrm{Sender} \cdot 10^{\frac{g_d-a+\qty{2.15}{\dB}}{\qty{10}{\dB}}} = \qty{6}{\watt} \cdot 10^{\frac{\qty{13}{\dBd}+\qty{2.15}{\dB}}{\qty{10}{\dB}}} \approx \qty{197}{\watt}$

This calculation, too, can easily be done in your head by splitting the total gain into sensible parts:
  
$\qty{13}{\dBd} + \qty{2.15}{\dB} = \qty{10}{\dBd} + \qty{3}{\dB} + \qty{2.15}{\dB}$

This gives:

$P_\mathrm{EIRP} = \qty{6}{\watt} \cdot 10 \cdot 2 \cdot 1.64 \approx \qty{197}{\watt}$
</indepth>

[question:EK104]
  
The [Instructions for notifying fixed amateur radio installations under Section 9 BEMFV](https://50ohm.de/abemfv) lay down exactly what is meant by the safety distance. The site-specific safety distance describes the distance required between the reference antenna and the area in which the applicable limits must be complied with. The relevant field strengths of surrounding fixed radio installations must also be taken into account.

What matters here is that the safety distance does not refer to a single point of the antenna, but to the entire antenna structure. In other words, for every point of the antenna it must be ensured that the limits are complied with outside the calculated safety distance.

[question:EK107]
