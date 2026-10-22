An oscilloscope is a voltmeter that can show how voltages vary over time. Just like other voltmeters, oscilloscopes have a high internal resistance. Usually two or more voltages can be measured at the same time. The instrument in Figure [ref:e_oszilloskop_digital], for example, is set so that two signals share the screen.

<margin>
[photo:212:e_oszilloskop_digital: Oscilloscope with numerous additional functions]
</margin>

Let us now look more closely at the oscilloscope display in Figure [ref:e_oszilloskop_bildschirmfoto_sinus]. With an oscilloscope you can, for example, determine the parameters of a sinusoidal AC voltage ($T$, $\hat{U}$, $U_\text{SS}$ and $U_\text{eff}$). Besides the waveform, a time value and a voltage value are shown – in the example $\qty{50.0}{\nano\second}$ and $\qty{500}{\milli\volt}$. This means that one square corresponds to 50 ns horizontally and 500 mV vertically. These squares are often called divisions, hence the notation $\qty{500}{\milli\volt\per\oszidiv}$.

<margin>
[photo:214:e_oszilloskop_bildschirmfoto_sinus:A sinusoidal voltage displayed on a digital oscilloscope]
</margin>

---

We can think of this as a coordinate system and read off the period ($T$) and the amplitude ($\hat{U}$). In the example, one period is 5 squares, or divisions, long. Multiplied by $\qty{50.0}{\nano\second}$ per division, this gives a period of $\qty{250.0}{\nano\second}$. The amplitude, i.e. the largest deviation from the zero position, is $\qty{1500}{\milli\volt}$ or $\qty{1.5}{\volt}$, because it is 3 divisions high and each division corresponds to $\qty{500}{\milli\volt}$. 

[question:EI301]

<tip>
For simple measurements, many digital oscilloscopes have an AUTO button. When you press it, some settings are made automatically and usually a stationary picture of the applied signals appears. The display can be shifted horizontally. A knob with this function is often labelled X position. To read off the period, you move a distinctive point such as a zero crossing onto a vertical line of the grid and count how many divisions correspond to one period.
</tip>
 
---

Once the period of an oscillation is known, the frequency can also be determined from it. In Class N we already met the relationship in qualitative terms: the frequency gives the number of oscillations per second. If the period is one second, the frequency is $\qty{1}{\hertz}$. If we halve the period to half a second, two oscillations fit into one second – the frequency is then $\qty{2}{\hertz}$.

In Class E we now look at this relationship as a formula:
  
$f=\dfrac{1}{T}$ or $T=\dfrac{1}{f}$

The frequency in hertz is the reciprocal of the period in seconds.

The signal in Figure [ref:e_oszilloskop_bildschirmfoto_sinus] therefore has the frequency

$f = \dfrac{1}{\qty{250}{\nano\second}} = \qty{4}{\mega\hertz}$.
 
[question:EB408]
[question:EB409]
[question:EB411]
[question:EB410]
[question:EI302]

---

Sometimes signals are distorted unintentionally. This happens, for example, when too high an input voltage is fed into an amplifier. The amplifier is then said to be overdriven, and its output signal distorted. Severe distortion like that in Figure [ref:e_oszilloskop_verzerrt] can be seen on an oscilloscope. For assessing audio signals in amateur radio, this is usually sufficient.

<margin>
[photo:215:e_oszilloskop_verzerrt:Sinusoidal input signal (top) and distorted output signal of an overdriven amplifier]
</margin>

<indepth>
Whether an RF signal is free of distortion that affects other frequency ranges cannot be judged well enough with an oscilloscope. The right instrument for that is a spectrum analyser.
</indepth>

% EI304 NF-Verzerrungen 
[question:EI304]