Sinusoidal AC voltages change their value continuously. To be able to describe them better, we will look at three important parameters below:

1. $\hat{U}$: the peak value of an AC voltage
2. $U_\text{SS}$: the peak-to-peak value 
3. $U_\text{eff}$: the RMS value

<margin>
[picture:834:e_wechselspannung_kenngroessen:The three parameters of an AC voltage]
</margin>

---

The *peak value* $\hat{U}$ of an AC voltage corresponds to the amplitude, which we already met in Class N (cf. Figure [ref:e_wechselspannung_kenngroessen]). Among other things, it matters for the voltage rating of capacitors. Figure [ref:e_spannungsfestigkeit_elkos] shows two leaded electrolytic capacitors with their permissible voltage rating printed on them. The peak value of the applied voltage must not exceed this limit, otherwise the capacitor may be destroyed. Components with a higher voltage rating than required are often chosen – either for safety reasons or to extend their service life.

<margin>
[photo:198:e_spannungsfestigkeit_elkos:Electrolytic capacitors with voltage ratings of 16 V and 25 V]
</margin>

Another parameter is the *peak-to-peak value*. This is the difference between the highest and the lowest excursion. For sinusoidal AC voltages:

$U_\text{SS} = 2\cdot \hat{U}$.
 
[question:EB406]
[question:EB407]

When it is not the voltage but the power of equipment or the thermal load on components and cables that matters, the peak value is of no help. For this case the *RMS value* has been defined. The RMS value of an AC voltage corresponds to the value of a DC voltage that would heat an ohmic resistor to the same degree. 

---

For sinusoidal voltages, the peak (or crest) value is about 1.4 times the RMS value (see Figure [ref:e_wechselspannung_kenngroessen]). The exact calculation leads to a simple formula:

$U_{eff} = \frac{\hat{U}}{\sqrt{2}}$ or $\hat{U} = U_{eff} \cdot \sqrt{2}$

If an AC voltage is given only with the letter $U$ and no subscript, it is usually the RMS value that is meant. The best-known example is our mains voltage of $\qty{230}{\volt}$ – this, too, is the RMS value. The peak voltage is considerably higher, namely

$\hat{U} = \qty{230}{\volt} \cdot \sqrt{2} \approx \qty{325}{\volt}$.

<indepth>
The exact derivation of this formula uses integral calculus and goes beyond the knowledge required for the amateur radio examination. If you are familiar with integral calculus and interested, you can read the derivation here: [Wikipedia](https://50ohm.de/ew)
</indepth>

[question:EB401]

For the mains voltage, $U_\text{SS}$ then comes to twice the peak value: 

$ U_\text{SS} = 2 \cdot \qty{230}{\volt} \cdot \sqrt{2} \approx \qty{651}{\volt}$

[question:EB402]

The following two questions work on the same principle: 

[question:EB403]
[question:EB404]

---

% TODO referenz auf das Leistungskapitel einfügen:

The next question asks indirectly for the RMS value of the voltage. If you know that $\frac{1}{\sqrt{2}} \approx 0.7$, you can read off the two results directly. 

<indepth>
What matters is that both the DC voltage $\qty{0.7}{\volt}$ and the DC voltage $\qty{-0.7}{\volt}$ lead to the same result. This is because with a negative voltage the sign of the current changes as well, which nevertheless results in the same power – since $P = U \cdot I$.
</indepth>

[question:EB405]

By the way: everything written here about AC voltages applies in the same way to alternating currents.