## Cut-off frequency

For high-pass and low-pass filters the cut-off frequency is given by

<left>
For RL networks
$R = X_\text{L}$
$f_\text{g} = \frac{R}{2 \pi \cdot L}$
</left>
<right>
For RC networks
$R = X_\text{C}$
$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C}$
</right>


---
[question:AD201]
---
#### Solution
* given: $R = \qty{4.7}{\kilo\ohm}$
* given: $C = \qty{2.2}{\nano\farad}$
* required: $f_\text{g}$

<fragment>
$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C} = \frac{1}{2 \pi \cdot \qty{4.7}{\kilo\ohm} \cdot \qty{2.2}{\nano\farad}} \approx \qty{15.4}{\kilo\hertz}$
</fragment>
---
[question:AD202]
---
#### Solution
* given: $R = \qty{10}{\kilo\ohm}$
* given: $C = \qty{47}{\nano\farad}$
* required: $f_\text{g}$

<fragment>
$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C} = \frac{1}{2 \pi \cdot \qty{10}{\kilo\ohm} \cdot \qty{47}{\nano\farad}} \approx \qty{339}{\hertz}$
</fragment>
---
[question:AD203]
---
#### Solution
* given: $R_1 = \qty{4.7}{\kilo\ohm}$
* given: $C_1 = \qty{6.8}{\nano\farad}$
* required: $f_\text{g}$

<fragment>
$C_2$ and all the other details are irrelevant for the low-pass filter.
</fragment>

<fragment>
$f_\text{g} = \frac{1}{2 \pi \cdot R_1 \cdot C_1} = \frac{1}{2 \pi \cdot \qty{4.7}{\kilo\ohm} \cdot \qty{6.8}{\nano\farad}} \approx \qty{5}{\kilo\hertz}$
</fragment>
---
## Resonant frequency

* Inductor and capacitor in parallel or in series $\rightarrow$ tuned circuit
* High frequencies $\rightarrow$ high resistance of the inductor
* Low frequencies $\rightarrow$ high resistance of the capacitor
* There is one frequency at which the inductor and the capacitor have the same resistance $\rightarrow$ *resonant frequency*

---
[question:AD206]
--- style="font-size: smaller;"
## Parallel tuned circuit

[picture:233:a_schwingkreis_parallelschwingkreis:Parallel tuned circuit and its impedance plotted against frequency]

* Ideal components keep recharging each other
* In theory the impedance at the resonant frequency is infinitely high
* In practice the component with the lowest resistance determines the total impedance
* At frequencies above and below the resonant frequency the parallel tuned circuit has a lower impedance

--- style="font-size: smaller;"
## Series tuned circuit

[picture:230:a_schwingkreis_reihenschwingkreis:Series tuned circuit and its impedance plotted against frequency]

* Called *Reihenschwingkreis* or *Serienschwingkreis* in German
* In theory the impedance at the resonant frequency is $\qty{0}{\ohm}$
* In practice the impedance is determined by the ohmic resistance
* At frequencies above and below the resonant frequency the series tuned circuit has a higher impedance

---
[question:AD207]
---
[question:AD204]
---
## Resonance

For parallel and series tuned circuits:

$X_\text{C} = X_\text{L}$

The impedances are equal.

<fragment>
Resonant frequency from Thomson's formula:

$f_0 = \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}$
</fragment>

<note>
William Thomson, later Lord Kelvin, in 1853
</note>
---


[question:AD208]
---
#### Solution
* given: $L = \qty{1.2}{\micro\henry}$
* given: $C = \qty{6.8}{\pico\farad}$
* given: $R = \qty{10}{\ohm}$
* required: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{1.2}{\micro\henry} \cdot \qty{6.8}{\pico\farad}}} \approx \qty{55.7}{\mega\hertz} \end{split}$
</fragment>
<fragment>
The resistor $R$ is not needed for the calculation.
</fragment>
---
[question:AD209]
---
#### Solution
* given: $L = \qty{10}{\micro\henry}$
* given: $C = \qty{1}{\nano\farad}$
* required: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{10}{\micro\henry} \cdot \qty{1}{\nano\farad}}} \approx \qty{1.592}{\mega\hertz} \end{split}$
</fragment>
---
[question:AD210]
---
#### Solution
* given: $L = \qty{100}{\micro\henry}$
* given: $C = \qty{0.01}{\micro\farad}$
* required: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{100}{\micro\henry} \cdot \qty{0.01}{\micro\farad}}} \approx \qty{159}{\kilo\hertz} \end{split}$
</fragment>
---
[question:AD211]
---
#### Solution
* given: $L = \qty{2.2}{\micro\henry}$
* given: $C = \qty{56}{\pico\farad}$
* required: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{2.2}{\micro\henry} \cdot \qty{56}{\pico\farad}}} \approx \qty{14.34}{\mega\hertz} \end{split}$
</fragment>
---
[question:AD212]
--- style="font-size: 0.7em;"
#### Solution
* given: $C_1 = \qty{0.1}{\nano\farad}$
* given: $C_2 = \qty{1.5}{\nano\farad}$
* given: $C_3 = \qty{220}{\pico\farad}$
* given: $L = \qty{1.2}{\milli\henry}$
* required: $f_0$

<fragment>
$C = C_1 + C_2 + C_3 = \qty{0.1}{\nano\farad} + \qty{1.5}{\nano\farad} + \qty{220}{\pico\farad} = \qty{1.82}{\nano\farad}$
</fragment>
<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{1.2}{\milli\henry} \cdot \qty{1.82}{\nano\farad}}} \approx \qty{107.7}{\kilo\hertz} \end{split}$
</fragment>
---
### Changing the resonant frequency

* Larger inductor or capacitor $\rightarrow$ lower resonant frequency
* Smaller inductor or capacitor $\rightarrow$ higher resonant frequency

<fragment>
Increasing the inductance
* Increase the number of turns
* Push the turns closer together
* Insert a ferrite core

</fragment>

---
[question:AD213]
---
[question:AD214]
---
[question:AD215]
---
[question:AD216]
---
[question:AD217]
---
### Voltage-controlled tuned circuit

[picture:752:a_schwingkreis_potentiometer:Changing the capacitance with a varicap]

* The varicap is varied by a control voltage from the resistive potential divider
* Lower voltage across the varicap $\rightarrow$ narrower junction in the varicap $\rightarrow$ higher capacitance
* Capacitors connected in series $\rightarrow$ capacitance becomes smaller $\rightarrow$ resonant frequency rises

---
[question:AD218]
--- style="font-size: smaller;"
## Band-pass filter

[picture:785:a_schwingkreis_bandpass:Band-pass filter made of several tuned circuits]

* Combination of parallel and series tuned circuits
* Passes a particular frequency range
* Parallel tuned circuits act like high resistances
* Series tuned circuit acts like a low resistance

---
[question:AD205]
---
## Bandwidth

* Depends strongly on the ohmic resistance
* Stated in dB relative to a reference value of the filter
* E.g. *bandwidth* at the *$\qty{-3}{\dB}$ value*
* Half the power of a signal can still pass the filter
* Or $\num{0.7}$ times the signal voltage

---
[question:AD219]
---
[question:AD220]
---
### Typical bandwidths

* Narrowband, $\qty{500}{\hertz}$, for telegraphy (CW)
* Wideband, $\qty{2.7}{\kilo\hertz}$, for voice modulation (SSB)

---
[question:AD221]
---
[question:AD222]
---
## Q factor of a tuned circuit

* Also called the quality factor
* A measure of energy loss
* Ratio of the reactances to the ohmic resistance at resonance ($X_\text{L} = X_\text{C}$)

<fragment>
<left>
Series tuned circuit
$Q = \frac{f_0}{B} = \frac{X_\text{L}}{R_\text{S}}$
</left>
<right>
Parallel tuned circuit
$Q = \frac{f_0}{B} = \frac{R_\text{P}}{X_\text{L}}$
</right>
</fragment>
  
---
[question:AD225]
--- style="font-size: 0.7em;"
#### Solution
<left>
* given: $L = \qty{100}{\micro\henry}$
* given: $C = \qty{0.01}{\micro\farad}$
</left>
<right>
* given: $R_\text{S} = \qty{10}{\ohm}$
* required: $Q$
</right>

<fragment>
First calculate $f_0$
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{100}{\micro\henry} \cdot \qty{0.01}{\micro\farad}}} \approx \qty{159.2}{\kilo\hertz} \end{split}$
</fragment>
<fragment>
Then calculate $B$ or $X_\text{L}$
$\begin{split} X_\text{L} &= \omega \cdot L = 2 \pi \cdot f_0 \cdot L\\ &= 2 \pi \cdot \qty{159.2}{\kilo\hertz} \cdot \qty{100}{\micro\henry} \approx \qty{100.03}{\ohm} \end{split}$
</fragment>
<fragment>
$Q = \frac{X_\text{L}}{R_\text{S}} = \frac{\qty{100.03}{\ohm}}{\qty{10}{\ohm}} \approx 10$
</fragment>
---
[question:AD226]
--- style="font-size: 0.7em;"
#### Solution
<left>
* given: $L = \qty{2.2}{\micro\henry}$
* given: $C = \qty{56}{\pico\farad}$
</left>
<right>
* given: $R_\text{P} = \qty{1}{\kilo\ohm}$
* required: $Q$
</right>

<fragment>
First calculate $f_0$
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{2.2}{\micro\henry} \cdot \qty{56}{\pico\farad}}} \approx \qty{14.34}{\mega\hertz} \end{split}$
</fragment>
<fragment>
Then calculate $B$ or $X_\text{L}$
$\begin{split} X_\text{L} &= \omega \cdot L = 2 \pi \cdot f_0 \cdot L\\ &= 2 \pi \cdot \qty{14.34}{\mega\hertz} \cdot \qty{2.2}{\micro\henry} \approx \qty{198.2}{\ohm} \end{split}$
</fragment>
<fragment>
$Q = \frac{R_\text{P}}{X_\text{L}} = \frac{\qty{1}{\kilo\ohm}}{\qty{198.2}{\ohm}} \approx 5$
</fragment>
---
### Calculating the bandwidth

From the resonant frequency and the Q factor

$Q = \frac{f_0}{B} \Rightarrow B = \frac{f_0}{Q}$

<fragment>
Or, substituting Thomson's formula

<left>
Series tuned circuit
$B = \frac{R_\text{S}}{2 \pi \cdot L}$
</left>
<right>
Parallel tuned circuit
$B = \frac{1}{2 \pi \cdot R_\text{P} \cdot C}$
</right>
</fragment>
<note>
Derivation not shown
</note>

---
[question:AD224]
---
#### Solution
* given: $L = \qty{2.2}{\micro\henry}$
* given: $C = \qty{56}{\pico\farad}$
* given: $R_\text{P} = \qty{1}{\kilo\ohm}$
* required: $B$

<fragment>
$\begin{split} B &= \frac{1}{2 \pi \cdot R_\text{P} \cdot C}\\ &= \frac{1}{2 \pi \cdot \qty{1}{\kilo\ohm} \cdot \qty{56}{\pico\farad}} \approx \qty{2.84}{\mega\hertz} \end{split}$
</fragment>

---
[question:AD223]
---
#### Solution
* given: $L = \qty{100}{\micro\henry}$
* given: $C = \qty{0.01}{\micro\farad}$
* given: $R_\text{S} = \qty{10}{\ohm}$
* required: $B$

<fragment>
$B = \frac{R_\text{S}}{2 \pi \cdot L} = \frac{\qty{10}{\ohm}}{2 \pi \cdot \qty{100}{\micro\henry}} \approx \qty{15.9}{\kilo\hertz}$
</fragment>
--- style="font-size: 0.7em;" data-transition="none"
## Coupling

[picture:184:a_schwingkreis_kopplung:Inductive coupling of two tuned circuits and the voltage plotted against frequency]

* Coupled tuned circuits are often used between circuit stages or filters
* Two tuned circuits coupled to each other inductively or capacitively
* The degree of coupling determines how much they affect each other, the bandwidth and the passband curve

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Inductive coupling of two tuned circuits and the voltage plotted against frequency]

* d: *loose coupling* $\rightarrow$ the circuits hardly affect each other, very high passband loss and very small bandwidth
* c: *under-critical coupling* $\rightarrow$ the circuits hardly affect each other, high passband loss and small bandwidth

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Inductive coupling of two tuned circuits and the voltage plotted against frequency]

* b: *critical coupling* $\rightarrow$ the circuits affect each other somewhat, flat passband curve with low loss and a plateau in the passband, and a good bandwidth

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Inductive coupling of two tuned circuits and the voltage plotted against frequency]
* a: *over-critical coupling* $\rightarrow$ the circuits affect each other strongly, the resonant frequencies shift, large bandwidth and distortion of the passband curve in the passband, with "dips"

---
[question:AD227]
---
[question:AD228]
---
[question:AD229]
