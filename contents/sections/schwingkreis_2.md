On the formula sheet we find the following formula for calculating the cut-off frequency of RC networks, e.g. of high-pass or low-pass filters:

$f_g = \frac{1}{2 \pi \cdot R \cdot C}$

With this formula we can solve a number of examination questions.

<indepth>
For mathematically minded readers: the formula for the cut-off frequency of an RC network can also be derived by looking at the complex impedances of the resistor and the capacitor. We treat the RC low-pass filter as a frequency-dependent potential divider.

[picture:175:a_rc_tiepass:RC low-pass filter as a frequency-dependent potential divider]

For the ratio of output voltage to input voltage:

$\frac{|U_A|}{|U_E|} = \frac{|X_C|}{|R + X_C|}$

The capacitive reactance of the capacitor is:

$X_C = \frac{1}{j\omega C}$

This gives:

$\frac{|U_A|}{|U_E|} = \frac{\left|\frac{1}{j\omega C}\right|}{\left|R + \frac{1}{j\omega C}\right|}$

For the magnitudes we obtain:

$\frac{|U_A|}{|U_E|} = \frac{\frac{1}{\omega C}}{\sqrt{R^2 + \frac{1}{\omega^2 C^2}}}$

Multiplying the numerator and the denominator by $\omega C$ simplifies the expression to:

$\frac{|U_A|}{|U_E|} = \frac{1}{\sqrt{1 + R^2\omega^2 C^2}}$

The cut-off frequency is defined as the frequency at which the output voltage has fallen to the factor $\frac{1}{\sqrt{2}} \approx 0{.}707$ of its original value. This corresponds to about $\qty{70}{\percent}$ of the output voltage, or a drop in level of $\qty{3}{\dB}$.

$\frac{|U_A|}{|U_E|} = \frac{1}{\sqrt{2}}$

It follows that:

$\frac{1}{\sqrt{1 + R^2\omega^2 C^2}} = \frac{1}{\sqrt{2}}$

So it must be true that:

$R^2\omega^2 C^2 = 1$

and therefore:

$\omega R C = 1$

With $\omega = 2\pi f$ this gives:

$2\pi f_g R C = 1$

From this it follows for the cut-off frequency:

$f_g = \frac{1}{2\pi R C}$
</indepth>

[question:AD201] 
[question:AD202] 
[question:AD203] 

---

The magnitude response of a series tuned circuit made up of a resistor, an inductor and a capacitor, as shown in Figure [ref:a_serienschwingkreis], is calculated with the following formula:
  
$Z = \sqrt{R^2+\left(X_\text{L} - X_\text{C}\right)^2}$

<margin>
[picture:181:a_serienschwingkreis:Series tuned circuit]
</margin>

---

If the reactance of the inductor is exactly as large as the reactance of the capacitor, i.e. $X_\text{L} = X_\text{C}$, the impedance is:

$Z=\sqrt{R^2+\left(0\right)^2}=\sqrt{R^2}=R$

This is the so-called *resonant frequency* $f_0$ of the tuned circuit, at which the impedance is determined by the ohmic resistance alone. At frequencies above and below the resonant frequency the impedance is greater than the ohmic resistance, because either the inductor or the capacitor has a higher reactance. Figure [ref:a_serienschwingkreis_frequenzgang] shows the magnitude response of a series tuned circuit, in which the resonant frequency can be clearly seen. At frequencies above and below the resonant frequency a series tuned circuit therefore has a high total resistance (impedance). At high frequency the inductor has a high resistance. At low frequency the capacitor has a high resistance. 

<margin>
[picture:1037:a_serienschwingkreis_frequenzgang:Magnitude response of a series tuned circuit]
</margin>

[question:AD206]
[question:AD207] 
[question:AD204] 

So, as shown above, the following relationship applies to parallel and series tuned circuits at resonance:

$X_\text{C} = X_\text{L}$

If we now insert the formulas for the reactances of the inductor and the capacitor into the equation above, we obtain:

$2\pi f \cdot L = \frac{1}{2\pi f \cdot C}$
  
This gives the formula: 
  
$f_0 = \frac{1}{2\pi \sqrt{L\cdot C}}$

---

This formula is called Thomson's formula and applies to both parallel and series tuned circuits. On the formula sheet we find it under the topic "tuned circuits" (*Schwingkreise*). It states that the resonant frequency of a tuned circuit depends only on the inductance of the inductor and the capacitance of the capacitor. Ohmic resistances and losses have no influence on the resonant frequency. With the formula we can calculate the resonant frequency of tuned circuits. 

<indepth>
Ohmic resistances in parallel and series tuned circuits do, however, affect the Q factor ($Q$) and therefore the bandwidth ($B$) of the tuned circuit - we will go into this in more detail later.
</indepth>


[question:AD208] 
[question:AD209]
[question:AD210] 

---

The resonant frequency of parallel tuned circuits is calculated with Thomson's formula given above, exactly as for series tuned circuits. 

[question:AD211] 
[question:AD212] 

---

To change the resonant frequency of tuned circuits, either the inductance of the inductor or the capacitance of the capacitor in the tuned circuit can be changed.
As can be seen from Thomson's formula, the quantities $L$ and $C$ are both in the denominator. Increasing $L$ or $C$ therefore lowers the frequency of the tuned circuit, because the denominator of the formula becomes larger. Conversely, reducing $L$ and $C$ raises the resonant frequency of the tuned circuit.

<indepth>
The square root has no influence on this relationship, since the root of a larger number is also a larger number. The relationship is, however, not linear.
</indepth>

The inductance of a coil can be increased by increasing the number of turns, by pushing the turns closer together or by inserting a ferrite core.
Conversely, the inductance of a coil can be reduced by reducing the number of turns, by pulling the turns apart, by removing a ferrite core or by inserting a copper core. The capacitance of capacitors can be changed by replacing them or by using trimmer or variable capacitors.

With this knowledge we can now answer the following questions.

[question:AD213] 
[question:AD214] 
[question:AD215] 
[question:AD216] 
[question:AD217] 

A combination of parallel and series tuned circuits, suitably arranged, can be used as a band-pass filter. At resonance, the parallel tuned circuits behave like high resistances and the series tuned circuit like a low resistance.

[question:AD205]

The bandwidth of filters and band-pass filters is often stated with reference to a particular attenuation value. The attenuation describes how much a signal is weakened compared with the maximum passed.

The *bandwidth* of a filter is usually defined by the so-called $\qty{-3}{\dB}$ point.

At the $\qty{-3}{\dB}$ point:

- Only half the power still passes the filter
- The signal voltage is still about $0{.}7$ times the maximum value

The bandwidth is the difference between the upper and lower cut-off frequencies at $\qty{-3}{\dB}$:

$ B = f_\mathrm{o} - f_\mathrm{u} $

[question:AD220]

Where:

- $f_\mathrm{o}$: upper cut-off frequency
- $f_\mathrm{u}$: lower cut-off frequency

The $\qty{-3}{\dB}$ bandwidth is used to describe how suitable a filter is for particular modes:

- Narrowband filter with a bandwidth of about $\qty{500}{\hertz}$: suitable for CW (telegraphy)
- Wider filter with a bandwidth of about $\qty{2.7}{\kilo\hertz}$: suitable for SSB voice transmission

[question:AD221] 
[question:AD222]

In the following question, the bandwidth must be read off not at the $\qty{-3}{\dB}$ point but at the $\qty{-60}{\dB}$ point.

[question:AD219]

The Q factor of a tuned circuit is determined by the ratio of the reactances of the capacitance and the inductance at resonance to the ohmic loss resistance. If a tuned circuit contained no ohmic loss resistance at all, its Q factor would be infinite. Real components, however, always have losses. Inductors always have an ohmic loss resistance; capacitors have dielectric losses, which also act as an ohmic resistance. The greater the ohmic resistances in a tuned circuit, the lower its Q factor. Crystal filters are often used for filters with a high Q and steep skirts.

To calculate the Q factor, we use the corresponding formulas from the formula sheet, depending on whether it is a parallel or a series tuned circuit:

For the series tuned circuit at resonance ($X_\text{L} = X_\text{C}$):

$Q = \frac{f_0}{B} = \frac{X_\text{L}}{R_\text{S}}$

For the parallel tuned circuit at resonance ($X_\text{L} = X_\text{C}$):

$Q = \frac{f_0}{B} = \frac{R_\text{P}}{X_\text{L}}$

[question:AD225]


---

In the same way as in the calculation example above, we can now also calculate the Q factor of the parallel tuned circuit. The resonant frequency is calculated as in the previous example. Note, however, that the formula for the parallel tuned circuit must be used to calculate $Q$:

$Q = \frac{f_0}{B} = \frac{R_\text{P}}{X_\text{L}}$

[question:AD226]

The bandwidth of parallel and series tuned circuits can now also be calculated easily from the resonant frequency of the tuned circuit and its Q factor, as follows (the formula is on the formula sheet):

$Q = \frac{f_0}{B}$

Rearranging the formula gives the bandwidth $B$:

$B = \frac{f_0}{Q}$

This formula applies to both the series and the parallel tuned circuit!

[question:AD224]

With the knowledge described above, the following question can now also be worked out step by step.
[question:AD223]

---

Coupled tuned circuits are often used to pass signals between circuit stages and in filters in transmitters and receivers. Here two tuned circuits are coupled to each other inductively or capacitively. Figure [ref:a_gekoppelte_schwingkreise] shows inductive coupling. Depending on the application, this coupling can be 

- *loose* (d),
- *under-critical* (c),
- *critical* (b) or 
- *over-critical* (a).

The degree of coupling determines how much the circuits affect each other and therefore the bandwidth and the passband curve of the whole arrangement.

<margin>
[picture:184:a_gekoppelte_schwingkreise:Coupling of tuned circuits]
</margin>

With loose and under-critical coupling the circuits hardly affect each other; on the other hand, the passband loss of the arrangement is relatively high and the bandwidth relatively small.

With critical coupling the two tuned circuits affect each other just enough to give a passband curve that is flat in the passband with low loss and completely level over the wanted passband (a plateau). The bandwidth of the arrangement is greater here than with loose and under-critical coupling. This also makes critical coupling easy to recognise.

With over-critical coupling the two tuned circuits affect each other very strongly, which shifts both resonant frequencies considerably and so leads to a large bandwidth. As a result, the passband curve is heavily distorted in the passband, and two resonance peaks form to the left and right of the centre frequency. The passband curve gets a "dip". This makes over-critical coupling easy to recognise.

[question:AD227] 
[question:AD228] 
[question:AD229] 