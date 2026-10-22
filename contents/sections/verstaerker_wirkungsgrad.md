An amplifier draws DC power from its power supply and converts part of it into RF output power (see Figure [ref:a_wirkungsgrad_verstaerker]). A further part is converted, mainly into heat, in the transistor and in other components. A particular contributor to this is the quiescent current, which flows even when there is no input signal and which we will look at more closely in the next chapter. 

<margin>
[picture:1120:a_wirkungsgrad_verstaerker:Power flow in an amplifier, with the DC input power, the RF output power and the power dissipation]
</margin>

The *efficiency* $\eta$ states what proportion of the DC input power supplied is available as usable RF power at the output of the amplifier:

$\eta = \frac{P_\mathrm{HF}}{P_\mathrm{DC}}$

Here $P_\mathrm{HF}$ is the RF output power and $P_\mathrm{DC}$ is the DC power drawn from the power supply. This can be calculated from the supply voltage and the current drawn:

$P_\mathrm{DC} = U_\mathrm{B} \cdot I_\mathrm{B}$

The efficiency is a ratio without a unit and can at most reach the value $\num{1}$. It is usually given as a percentage, however:

$\eta_\mathrm{\%} = \eta \cdot \qty{100}{\percent}$

The efficiency of an RF power amplifier is therefore defined as the ratio of the RF output power delivered by the power amplifier to the DC supply power fed to the amplifier.

[question:AF401]

A high efficiency means that only a small part of the power drawn is lost as heat. With a low efficiency, on the other hand, a correspondingly larger power dissipation has to be removed by heatsinks or other measures.

<tip>
In the following examination questions, the efficiency is taken as the ratio of the RF output power to the DC power drawn. Any RF input power that may also be given is not taken into account in this simplified calculation.
</tip>

[question:AD430]
[question:AD429]