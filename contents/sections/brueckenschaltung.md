The bridge circuit is an arrangement of four resistors that is used, among other things, for precise resistance measurement. A well-known practical example is the Wheatstone bridge. The circuit consists of two potential dividers connected in parallel. Between the midpoints of the two potential dividers is what is called the bridge diagonal, across which the bridge voltage $U_\mathrm{AB}$ can be measured.

<margin>
[picture:343:a_Brückenschaltung:Typical bridge circuit with 4 resistors]
</margin>

The case of the balanced bridge is particularly interesting. It occurs when the divider ratios on both sides are equal. The two midpoints are then at the same electrical potential, and no current flows through the bridge diagonal or through the meter connected to it.

The individual resistors do not need to have the same value. All that matters is that the ratio of the resistors is the same on both sides.

For the balanced condition, therefore:

$ U_\mathrm{AB} = \qty{0}{\volt} $

and so:

$ \frac{R_1}{R_2} = \frac{R_3}{R_4} $

This makes the Wheatstone bridge particularly well suited to determining unknown resistances or small changes in resistance. Exactly how this works is described in the *In depth* box alongside.

<indepth>
The special case in which the divider ratios on the left and right of the bridge circuit are equal is used to measure unknown resistances. Charles Wheatstone (a British physicist) recognised the importance of the bridge circuit for measuring unknown resistances as early as 1833. 

During the measurement, an adjustable precision resistor is varied until the sensitive meter movement in the bridge diagonal no longer shows any current. The bridge is then balanced, and the value of the unknown resistor can be found from the scale and the range multiplier.

An example can be seen in Figure [ref:a_pontavi]. It has a multiplier that can take the values 0.1/1/10/100. For fine adjustment there is the large knob. 
[photo:286:a_pontavi:Wheatstone resistance measuring bridge (Pontavi)]

Figure [ref:a_pontavi_schaltung] shows the simplified circuit diagram of this instrument. The unknown resistor is connected at point $X$. First, the multiplier is set to the estimated order of magnitude of the unknown resistance. Then the precision resistor is varied with the large knob until the bridge is balanced. The meter movement then shows that no more current is flowing through the bridge diagonal.

[picture:1076:a_pontavi_schaltung:Circuit diagram of the resistance measuring bridge (Pontavi)]
</indepth>

[question:AD111]

Since all the resistors in the following question have the same value, the divider ratios must also be equal. This is the special case described above.

[question:AD112]

In the following question the special case does not apply, as the divider ratios are unequal. Similar resistors are present, but, looking from top to bottom, they are swapped round. The question can be solved with what we know about the unloaded potential divider.

[question:AD113]

On the left we find the ratio $\qty{1}{\kilo\ohm}$ to $\qty{10}{\kilo\ohm} = 1/10$.
Provided that the meter movement has a very high resistance or is disconnected, with an operating voltage of $\qty{11}{\volt}$ we measure exactly $\qty{1}{\volt}$ across the upper resistor ($R_1$) on the left and $\qty{10}{\volt}$ across the lower resistor ($R_2$). The potential at measuring point A is therefore $\qty{10}{\volt}$, measured with respect to chassis.

On the right we find the ratio $\qty{10}{\kilo\ohm}$ to $\qty{1}{\kilo\ohm} = 10/1$ and therefore measure $\qty{10}{\volt}$ across the upper resistor ($R_3$) and $\qty{1}{\volt}$ across the lower resistor ($R_4$). The potential at measuring point B is therefore $\qty{1}{\volt}$, measured with respect to chassis.

The potential difference between A and B is therefore $\qty{9}{\volt}$, with measuring point A $\qty{9}{\volt}$ more positive than measuring point B.
