As already shown in the Class E chapter "Rectifiers I", a single diode lets only the positive half cycle through. To turn this into a usable DC voltage, at least one capacitor is also needed, which smooths the pulsating output voltage (see circuit [ref:a_einweggleichrichtung_c]).

<margin>
[picture:795:a_einweggleichrichtung_c:Half-wave rectification with a capacitor]
</margin>

---

During the positive half cycle the diode $D$ conducts and lets current flow. During this time the capacitor $C_L$ charges up to the peak value of the AC voltage. During the negative half cycle the diode $D$ blocks the current, and the capacitor $C_L$ discharges through the load resistor $R_L$.

A slightly pulsating DC voltage $U_L$ therefore appears across the load resistor $R_L$ (see Fig. [ref:a_Restwelligkeit]). The larger the capacitance of the capacitor, the more evenly the DC voltage across the load resistor is smoothed.

<margin>
[picture:75:a_Restwelligkeit:Ripple of the DC output voltage $U_L$]
</margin>

When choosing the diode and the capacitor, however, we need to know that transformer voltages are given as RMS voltages $U_{\mathrm{eff}}$. So we first have to work out the peak voltage $\hat{U}$.

$\hat{U} = \sqrt{2} \cdot U_{\mathrm{eff}}$

If, for example, a transformer is marked with the voltage $U_a = \qty{15}{\volt}$, we calculate:

$\hat{U} = \sqrt{2} \cdot U_{\mathrm{eff}} = \sqrt{2} \cdot \qty{15}{\volt} = \qty{21.21}{\volt}$

So with no load an open-circuit peak voltage of about $\qty{21}{\volt}$ will appear.

[question:AD302]

In the following question we have to apply the transformation ratio of the transformer to find our output voltage. So for the RMS input voltage $U_{\mathrm{eff}}$ we use one twentieth of the transformer input voltage of $\qty{230}{\volt}$. To the peak voltage we can then add half of the voltage again, to allow for the safety margin.

[question:AD303]

To solve the following problem, we must recognise that the peak value of the negative half cycle and the capacitor voltage add up and stress the diode in the reverse direction. This is the highest voltage that can occur across the diode in the reverse direction.

We calculate: $U_{\mathrm{sperr}} = 2 \cdot \hat{u}$
We then also have to take into account the transformation ratio $5 : 1$  of the mains transformer and the safety margin of $\qty{20}{\percent}$.

[question:AD304]

%TODO Simulation einbauen: https://tinyurl.com/22m65xlw