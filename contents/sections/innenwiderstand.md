In Class E we have already met voltage sources. First we want to deal with the current source, before we look more closely at the internal resistance of voltage and current sources.

In a similar way to the voltage source, a current source is designed to deliver as constant a current as possible. Figure [ref:a_isource_schematic] shows its equivalent circuit.

<margin>
[picture:1058:a_isource_schematic:Equivalent circuit of a current source, $R_i$ high]
</margin>

<indepth>
A look at a constant-current source, using a laboratory power supply as an example:

[photo:298:a_Strombegrenzung:Laboratory power supply with the current limit set to $\qty{500}{\milli\ampere}$]

Laboratory power supplies have built-in current limiting, i.e. if the load current exceeds a maximum current, the terminal voltage is lowered so that the load current stays constant. This corresponds to the function of a constant-current source -- if the output terminals are short-circuited, the maximum current that has been set flows.
</indepth>

An ideal constant-current source delivers a constant continuous current regardless of the load connected. In theory this is possible with an infinite internal resistance. In practice, current sources have a very high internal resistance.

<margin>
[picture:1018:a_vsource_schematic:Equivalent circuit of a voltage source]
</margin>

---

Figure [ref:a_vsource_schematic] shows an equivalent circuit of a voltage source. The internal resistance $R_i$ is in series with the ideal voltage source and should ideally be $\qty{0}{\ohm}$. In practice, voltage sources have a small internal resistance.

[question:AB201]

If a real voltage source is loaded with $R_L$, the terminal voltage $U_k$ falls. The reason for this is the internal resistance $R_i$ of the voltage source. It effectively forms a potential divider. Since the source voltage $U_q$ at open circuit, i.e. without a load, is $U_q=U_L$, it is also called the open-circuit voltage. 

The internal resistance cannot be measured with a multimeter, but it can be calculated using Ohm's law (see the formula sheet):

$R_i = \frac{\Delta U}{\Delta I}$

The calculation needs two load cases:
1. Open circuit, without a load: $I = \qty{0}{\ampere}$ and $U_L = U_q$
2. Loaded with $R_L$: we measure $I_L$ and $U_L$

From the change in voltage ($\Delta U = U_q~-~U_L$) at the terminals and the change in load current ($\Delta I = I_L~-~\qty{0}{\ampere}$), the internal resistance can be calculated with the formula above.

$R_i = \frac{\Delta U}{\Delta I} = \frac{U_q - U_L}{I_L-\qty{0}{\ampere}} = \frac{U_q - U_L}{I_L}$

With this knowledge we can answer the following examination questions:

[question:AB205]
[question:AB206]
[question:AB207]
[question:AB208]

To sum up:

* Voltage sources should have a very low internal resistance $R_i \ll R_L$, ideally $\qty{0}{\ohm}$; the output voltage then stays unchanged under load. If the terminal voltage stays constant under load, this is called voltage matching.
* Current sources should have a very high internal resistance $R_i \gg R_L$. Ideally: $\qty{\infty}{\ohm}$; the load current then stays constant when the load resistance changes, which is why this is also called current matching.

[question:AB203]
[question:AB204]

---

If a voltage source is to deliver the maximum power to a load, this is called power matching. This is also important, for example, for a transmitter that is to transfer as much power as possible to an antenna.

The maximum power transfer is achieved when

$R_i = R_L$

holds, i.e. when the internal resistance and the load resistance are equal.

In this case the source voltage is shared equally between the internal resistance and the load. This gives the maximum product of voltage and current at the load, and so the greatest possible power.

Figure [ref:a_Leistungsanpassung] shows the normalised power in the load as a function of the ratio $R_L/R_i$. The maximum is reached exactly at $R_L/R_i = 1$, that is, when the internal resistance and the load resistance are equal. However, the efficiency with power matching is only $\qty{50}{\percent}$, because the same power is dissipated in the load as in the internal resistance.

<margin>
[picture:1077:a_Leistungsanpassung:Optimum power matching at $R_i = R_L$: here the quotient $\frac{R_L}{R_i}=1$, and so the maximum power is delivered to the load. The plot is logarithmic.]
[picture:937:a_Leistungsanpassung:Optimum output power with a $\qty{50}{\ohm}$ load resistance and an internal resistance of $\qty{50}{\ohm}$. The plot is not logarithmic.]
</margin>

<indepth>
AC voltage sources, e.g. sine-wave generators, also have an internal resistance, which is stated at the output socket.
[photo:292:Sinusgenerator 50 Ohm:Sine-wave generator with an internal resistance of 50 Ω]
</indepth>

% GGF muss das woanders hin? 
<indepth>
The value of $\qty{50}{\ohm}$ often used in RF engineering is a technical compromise between maximum power transfer and the lowest possible losses in lines.

Coaxial cables with a characteristic impedance of about $\qty{30}{\ohm}$ can carry particularly high power, because of the way the current is distributed in the cable. Cables of about $\qty{77}{\ohm}$, on the other hand, have the lowest attenuation losses and are particularly well suited to low-loss signal transmission.

The value of $\qty{50}{\ohm}$, which is in widespread use today, lies between the two optima and is a good compromise between high power handling, moderate losses and a practical cable design. That is why $\qty{50}{\ohm}$ has become established as the standard in radio engineering.

If a transmitter, a cable and an antenna are each matched to $\qty{50}{\ohm}$, the power is transferred in the best possible way and reflections on the line are minimised.

[picture:1078:a_50ohm:50 Ω as a compromise between maximum power transfer and minimum losses in RF engineering]

Now you also know why our platform is called 50ohm.de: we want to help you master the examination questions and so deliver the optimum performance in the examination 🤓
</indepth>

[question:AG401]
[question:AB202]