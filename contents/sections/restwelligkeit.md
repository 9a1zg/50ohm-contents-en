Since no circuit works ideally, the voltage across the load resistor $R_L$ of a rectifier is not a perfectly constant DC voltage but a pulsating one. It results from the successive positive sinusoidal half cycles and the smoothing effect of the capacitors. This remaining AC component is called the ripple.
Its frequency is $f=\qty{100}{\hertz}$, because the negative half cycle is also mirrored into the positive range, which doubles the mains frequency of $\qty{50}{\hertz}$. If this pulsating DC voltage were fed through a potential divider into an amplifier with a loudspeaker, you could hear a $\qty{100}{\hertz}$ hum.

<webonly>
<margin>
[include:applet_brumm]
</margin>
</webonly>

[question:AD310]

This voltage can be observed with an oscilloscope by displaying only the AC component (see Figure [ref:a_AC-Kopplung]: AC coupling of the input).

<indepth>
[photo:306:a_AC-Kopplung:AC/DC coupling of the oscilloscope input]
The "GD" button switches the oscilloscope input to zero volts.
With the AC/DC button not pressed, the oscilloscope input is capacitively coupled and only the AC component of the input signal is displayed.
With the AC/DC button pressed, the oscilloscope input is DC-coupled (galvanically coupled), and the DC component of an AC voltage is displayed as well.
</indepth>

In the following question, both the frequency and the amplitude of the ripple have to be determined. 

[question:AD309]