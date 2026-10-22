In Class E we have already met the *unloaded* potential divider. In Class A we deal with the *loaded* potential divider, in which the output voltage $U_2$ is loaded by a load resistor $R_\mathrm{L}$. This means that the load resistor is in parallel with resistor $R_2$, as can be seen in the circuit diagram in Figure [ref:a_spannungsteiler_belastet].

<margin>
[picture:199:a_spannungsteiler_belastet:Loaded potential divider]
</margin>

With a loaded potential divider, you have to take into account that the total current rises when the load is increased, i.e. when the load resistance $R_\mathrm{L}$ becomes lower. The effects of the load are best explained with an actual example. Suppose that resistors $R_1$ and $R_2$ each have a value of $\qty{1}{\kilo\ohm}$ and the total voltage $U_\mathrm{B}$ is $\qty{12}{\volt}$.

In the unloaded case, the resistance is $R_\mathrm{L}=\infty$, so the resistor does not exist and no current can flow through it. The voltage is divided equally between the two resistors $R_1$ and $R_2$, i.e. $\qty{6}{\volt}$ can be measured across each resistor. The total resistance is $R_{\mathrm{ges}}=\qty{2}{\kilo\ohm}$. The total current is $I_1 = \frac{U_\mathrm{B}}{R_{\mathrm{ges}}}=\qty{6}{\milli\ampere}$. This current also flows through $R_2$. The power dissipated is the same in both resistors: $P_1 = P_2 = \qty{6}{\volt} \cdot \qty{6}{\milli\ampere} = \qty{36}{\milli\watt}$.

In the loaded case, let the load resistance also be $R_\mathrm{L} = \qty{1}{\kilo\ohm}$. The parallel connection of $R_2$ and $R_\mathrm{L}$ gives an equivalent resistance of $R_\mathrm{par}=\qty{500}{\ohm}$. The total resistance of the potential divider is now only $R_{\mathrm{ges}}=\qty{1.5}{\kilo\ohm}$. We now have a potential divider of $\qty{1}{\kilo\ohm}$ to $\qty{500}{\ohm}$, and the total voltage is divided accordingly. $\frac{2}{3}$ of the total voltage ($\qty{8}{\volt}$) can be measured across $R_1$ and $\frac{1}{3}$ of the total voltage ($\qty{4}{\volt}$) across $R_\mathrm{par}$. 

The current $I_1$ is now $I_1 = \frac{\qty{8}{\volt}}{\qty{1}{\kilo\ohm}}= \frac{\qty{12}{\volt}}{\qty{1.5}{\kilo\ohm}} = \qty{8}{\milli\ampere}$. So this current rises. 

The power in $R_1$ is now $P_1 = U_1 \cdot I_1 = \qty{8}{\volt} \cdot \qty{8}{\milli\ampere} = \qty{64}{\milli\watt}$, compared with $\qty{36}{\milli\watt}$ in the unloaded case. In $R_\mathrm{par}$ the power is $P_\mathrm{par} = U_\mathrm{par} \cdot I_\mathrm{par} = \qty{4}{\volt} \cdot \qty{8}{\milli\ampere} = \qty{32}{\milli\watt}$, compared with $\qty{36}{\milli\watt}$ in the unloaded case. Since the ${32}{\milli\watt}$ is shared between $R_2$ and $R_\mathrm{L}$, the power in $R_2$ falls in the loaded case to $P_2 = \qty{4}{\volt} \cdot \qty{4}{\milli\ampere} = \qty{16}{\milli\watt}$.

In summary: when a potential divider is loaded with a resistor, the current $I_1$ rises. As a result, $R_1$ gets warmer and $R_2$ less warm. With this knowledge we can easily solve the next question.

[question:AD115]

In the following question we have to combine what we know about the potential divider and about resistors in parallel. To do this, we break the problem down into steps: first, the equivalent resistance of the parallel connection of $R_2$ and $R_\mathrm{L}$ is found. The circuit can then be treated as a simple potential divider, and the output voltage $U_2$ calculated from it.

[question:AD114]
