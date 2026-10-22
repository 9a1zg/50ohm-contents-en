Because it takes so little effort, the bridge rectifier is a widely used rectifier circuit. It needs a transformer and 4 diodes.

<latexonly>
Figure [ref:a_brueckenlgeichrichter] shows such a bridge rectifier.

<margin>
[picture:965:a_brueckenlgeichrichter:Bridge rectifier]
</margin>
</latexonly>

<webonly>
The applet alongside shows such a bridge rectifier. With the polarity of the transformer voltage $U_a$ or $U_s$ shown, you can follow the path of the load current and see that it always flows through the load resistor $R$ in the same direction.

<margin>
[include:applet_gleichrichter_2]
</margin>
</webonly>

<tip>
[picture:67:a_brueckenlgeichrichter_2:Arrangement of the diodes in a bridge rectifier]
In a bridge rectifier the diodes point with their cathodes towards the positive terminal and with their anodes towards the negative terminal. So you can remember: the "bars" of the diodes meet at the positive output. This arrangement must not be confused with a diode ring mixer, which we will meet later. 
</tip>

[question:AD305]

---

If a reservoir capacitor $C_L$ and an LC smoothing filter (see Figure [ref:a_netzteil_Ucs] are fitted after the bridge rectifier, this gives a smaller amplitude in the pulsating DC output voltage. We then have a conventional power supply. 

<margin>
[picture:66:a_netzteil_Ucs:Rectifier circuit with smoothing]
</margin>

With the bridge rectifier, too, the capacitor charges up to the peak voltage $\hat{U}$ of the secondary voltage $U_{\mathrm{sek}}$ of the transformer.

$\hat{U}=U_{\mathrm{eff}}\cdot\sqrt{2}$

We also have to check whether the transformer has a transformation ratio $ü$. With this knowledge we can solve the following problem.

[question:AD306]

<indepth>
[photo:296: Brückengleichrichter Bauformen: Package styles of bridge rectifiers]
Pay attention to the marking of the terminals.

1. High-current bridge rectifier 26 MB 20 A ($\qty{200}{\volt}$, $\qty{25}{\ampere}$) in a metal case for mounting directly on a heatsink
2. B80 C 5000/3300 means: maximum operating voltage $\qty{80}{\volt}$, C capacitive load of max. $\qty{2500}{\micro\farad}$ with a protective resistor $R = \qty{1}{\ohm}$, maximum continuous load current: $\qty{5000}{\milli\ampere}$ with a heatsink, $\qty{3300}{\milli\ampere}$ without a heatsink
3. BY 225 bridge rectifier – special package
4. Round package of a bridge rectifier B 80 C 1000
5. B40 C 1500 – note the different order of the terminals
6. FPU 4M ($\qty{1000}{\volt}$, $\qty{4}{\ampere}$)
7. Order of the terminals embossed in the plastic
</indepth>
