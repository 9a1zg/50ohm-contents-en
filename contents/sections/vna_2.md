In Class E we have already met the *vector network analyser* (VNA) (see Figure [ref:a_vna_swr]). In Class A we want to look at how it works in a little more detail.

For a measurement, the VNA first generates an RF signal at a set start frequency and applies it to the device under test, for example an antenna or a tuned circuit. It then measures the signal coming back, or reflected, from the device under test. Both its amplitude and its phase are recorded. To reduce the effect of interference, several measurements can also be made at one frequency point and averaged.

After the measurement, the frequency is increased by a set step and the process is repeated. In this way the VNA steps through the whole range from the start frequency to the stop frequency. This process is also called a *frequency sweep*, or, occasionally in the past, *wobbulation*.

From the measured values at the individual frequency points, the VNA can determine various quantities and display them against frequency. These include, for example, the impedance of the device under test and the standing wave ratio (SWR). This shows at once, for example, at which frequencies an antenna is well matched or has a resonance.

<margin>
[photo:323:a_vna_swr:SWR measurement of an end-fed wire antenna. The SWR is close to $1$ at $\qty{14}{\mega\hertz}$]
[picture:526:a_vna_swr_2:Possible SWR curve of an antenna.]
</margin>

[question:AI201]
[question:AI202]
[question:AI203]

---

One way a VNA can display the impedance is by splitting it into its resistive and reactive parts (resistance $R$ and reactance $X$). The resistance is often given in $\unit{\ohm}$, and the reactance sometimes also as $j\unit{\ohm}$. Different instruments do not all display it in the same way. The $j$ comes from a notation used in electrical engineering, in which it stands for what mathematics calls the imaginary unit ($i$). Positive reactances indicate inductive behaviour, negative reactances capacitive behaviour.

<indepth>
*Imaginary numbers* are a popular tool in electrical engineering and mathematics. To be able to solve equations such as $x^2 = -1$, a so-called imaginary number ($i$) was invented which, multiplied by itself, gives a negative number: $i^2 = -1$. No real number satisfies such an equation, since a negative number times a negative number is a positive number. This is why $i$ is called "imaginary". This "invented" number, multiplied by itself, gives a negative number, namely $-1$. Adding a real number (e.g. $54$) to an imaginary number (e.g. $-12i$) gives a complex number: $54 - 12i$. A complex number can be used, for example, to describe the resistive and reactive parts of an impedance. Complex numbers can also be converted into an amplitude and a phase. In electrical engineering the letter $j$ is used instead of $i$, to avoid confusion with the symbol $i$ (for currents).
</indepth>

[question:AI204]
[question:AI205]
[question:AI206]

---

Many VNAs can display the SWR curve against frequency graphically. If the resonant frequency of an antenna is too low, you know that the antenna should be shortened. If it is too high, the antenna would have to be lengthened.

[question:AI207]
[question:AI208]