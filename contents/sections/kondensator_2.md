In Class E we have already met the capacitance of a capacitor and its qualitative behaviour with AC voltage: a capacitor behaves like a frequency-dependent resistance. We noted at the time that the capacitive reactance is inversely proportional to the frequency. If the frequency is reduced, the reactance $X_C$ becomes larger. If, on the other hand, the frequency is increased, the resistance falls accordingly. How a capacitor behaves with AC voltage can be described by the formula for the capacitive reactance $X_C$:

$|X_C| = \frac{1}{\omega\cdot C} = \frac{1}{2\pi\cdot f \cdot C}$

In Class A we now want to look at this behaviour more closely and also find out why this resistance is called a "reactance". First, however, to be able to answer the following question, we must remember that the reactance of a capacitor is also negative: 

[question:AC102]

<indepth>
Why is the capacitive reactance negative? The reason lies in complex AC calculation, which is not strictly necessary for the amateur radio examination.

For readers who know complex numbers, however, it should be mentioned that the correct form of the capacitive reactance is actually

$X_C = \frac{1}{j\omega C}$

Here $j$ stands for the imaginary unit $\sqrt{-1}$.

Multiplying the numerator and denominator of this expression by $j$ gives:

$X_C = \frac{1}{j\omega C} = \frac{1 \cdot j}{j\omega C \cdot j} =\frac{-j}{\omega C}$

This shows that the capacitive reactance is not only negative but also complex. The negative sign describes the phase relationship between current and voltage in the capacitor, which we will look at more closely in this chapter.
</indepth>

---

Modern, inexpensive measuring instruments that radio amateurs like to use today are antenna analysers or vector network analysers (VNA). They measure how the reactance $X_C$ changes with frequency and can also display the measurement result graphically.
Figure [ref:a_kapazitiver_Blindwiderstand] shows how the capacitive reactance (blue line) of a $\qty{1500}{\pico\farad}$ polystyrene (Styroflex) capacitor changes over the frequency range $\qtyrange{1}{4.5}{\mega\hertz}$. 

<margin>
[photo:248:a_kapazitiver_Blindwiderstand:Capacitive reactance $X_C$ (blue curve) and phase (red curve) of a $\qty{1500}{\pico\farad}$ polystyrene (Styroflex) capacitor over the frequency range $\qtyrange{1}{4.5}{\mega\hertz}$.]
</margin>


Now try to answer the following questions with the formula above. Pay particular attention to the units and the powers of ten so that you get the right results.

[question:AC104]
[question:AC105]
[question:AC106]
[question:AC107]

In the following question, the capacitance is required. Try to rearrange the formula for this so that you can calculate the capacitance $C$:

[question:AC108]

---

If current and voltage in a capacitor are measured at the same time with a dual-channel oscilloscope (see [ref:a_strom_eilt_vor]), the result is surprising at first: there is a phase shift of $\qty{90}{\degree}$ between current and voltage, with the current leading the voltage.

This means that the current has already reached its maximum while the voltage is still rising. This characteristic behaviour is a fundamental property of capacitors and plays an important part in AC engineering, particularly in filters and tuned circuits.
The red line in Figure [ref:a_kapazitiver_Blindwiderstand] shows the phase of the capacitive reactance at an almost constant $\qty{-90}{\degree}$.

[question:AC101]

<margin>
[photo:268:a_strom_eilt_vor:Phase shift between voltage and current in a capacitor]
</margin>

<tip>
Memory aid: Beim Kondensat*ooo*r eilt der Strom v*ooo*r! (in the capacitor, the current leads)
</tip>

---

The phase shift between voltage and current is therefore $\qty{90}{\degree}$, with the current (red) leading the voltage (blue), as shown in Figure [ref:a_blindleistung_kondensator]. If we look at the instantaneous power with $P = U \cdot I$, we get a power curve (green) that swings symmetrically about the zero line, also shown in Figure [ref:a_blindleistung_kondensator].

<margin>
[picture:943:a_blindleistung_kondensator:The product $U \cdot I$ gives the green power curve]
</margin>

The mean value of this power is zero, which means that no real power is dissipated. Instead, energy is periodically stored in the electric field of the capacitor and returned to the source. For an ideal, lossless capacitor we therefore speak of reactive power and a reactance.

Only an ohmic resistance absorbs real power, because in it voltage and current are in phase, that is, there is no phase shift. This means that voltage and current are positive or negative at the same time, so the instantaneous power $P = U \cdot I$ is always positive.

An ideal reactance, on the other hand, absorbs no real power and so, ideally, does not get warm either. Instead, energy is periodically stored and returned to the source.

[question:AC111]

[question:AC103]

---

If a capacitor nevertheless warms up in radio-frequency applications, this indicates losses in the component. An ideal capacitor would convert no energy into heat, but real capacitors have parasitic properties that lead to losses.

These losses can be seen in the equivalent circuit: the resistance $R_\text{ESR}$ (equivalent series resistance) describes the ohmic losses in the capacitor, while $R_\text{Isolator}$ models the losses in the dielectric. In addition, the parasitic inductance $L_\text{ESL}$ affects the behaviour at high frequencies.

To assess these losses technically, the Q factor $Q$ (quality factor) and the dissipation factor $\tan\delta$ are used. Both quantities describe how far a real capacitor departs from ideal behaviour.

There is a direct relationship between the two quantities:

$Q = \frac{1}{\tan\delta}$

Remember: high losses lead to a low Q factor $Q$ and so to a large dissipation factor $\tan\delta$. The higher the frequency, the greater the effect of these losses, because the reactance $X_C$ falls as the frequency rises while the parasitic resistances stay constant.

<margin>
[picture:1065:a_ersatzchaltbild_kondensator:Equivalent circuit of a real capacitor with parasitic losses.]
</margin>

---

[question:AC109]

[question:AC110]

<indepth>
With complex AC calculation, the reactance $X_C$ and the parasitic losses $R$ can be shown in the form of a phasor diagram: 
[picture:1066:a_tan_delta:$\tan\delta$ in the complex phasor diagram]

The tangent, after all, is the ratio of the opposite side to the adjacent side, in this case the losses $R$ in relation to the lossless capacitive reactance $X_C$. 

$\tan\delta = \frac{R}{|X_C|}$

The greater the losses, the larger the angle $\delta$ and so also the dissipation factor $\tan\delta$. An ideal capacitor would have an angle of $\delta = 0$ degrees, since it has no losses.

This complex, or geometric, addition gives the quantity $Z$. It is called the *impedance* and describes the complex total resistance of a component. The magnitude of the impedance, $|Z|$, is what German calls the *Scheinwiderstand*; in English it is usually also just called the impedance.
</indepth>
