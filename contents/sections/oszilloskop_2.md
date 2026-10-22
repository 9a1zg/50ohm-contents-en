In Class E we learnt that an oscilloscope displays how voltages vary over time. So we can use an oscilloscope to examine waveforms. 

[question:AI301]

<margin>
[picture:1005:a_impulsbreite:Determining the pulse width of a non-ideal square-wave signal]
</margin>

---

Besides sinusoidal AC voltages, digital technology also brings square-wave voltages. A perfectly rectangular voltage waveform, however, cannot exist. The edges are always somewhat sloping or distorted. The time between the rise and the fall of a rectangular pulse, which is called the pulse width or pulse duration, is therefore always measured at half height, i.e. at 50% of the voltage. This ensures that everyone gets the same measurement result for the same signal.

<indepth>
These distortions are caused by the unavoidable capacitances and inductances in cables and components, which act like filters and attenuate the high-frequency components of a square-wave signal.
</indepth>

[question:AI303]
[question:EI303]


Oscilloscopes can display signals of the most varied frequencies and waveforms. So that these signals appear stable on the screen, oscilloscopes have a trigger circuit. The instrument continuously monitors the input signal and starts the recording exactly when a previously defined condition is met – for example when the signal exceeds a certain voltage, known as the trigger voltage. From that moment, the measured values are sampled and stored, and then displayed as a trace on the screen.


As a result, every display always starts at the same state of the signal, so that periodic signals such as sine waves or square pulses appear frozen and are clearly recognisable. Digital oscilloscopes can also show single frames, that is, "freeze" the screen. This makes it easier to analyse non-periodic signals. The button for this is usually labelled SINGLE. Several measurements can also be superimposed, for example to make fluctuations of a signal over time (jitter) visible.

[question:AI302]

%<indepth>
%Abbildung [ref:a_oszilloskop_einzelbild] zeigt ein Einzelbild aus der Musikaufnahme von Abbildung [ref:a_oszilloskop_ueberlagerung]. Es wurde von einem älteren Oszilloskop abfotografiert, das hauptsächlich analog arbeitet und zusätzlich einen kleinen digitalen %Speicher besitzt.
%[photo:222:a_oszilloskop_einzelbild:Einzelbild aus einer Musikaufnahme]
%</indepth>

Not every cable is suitable for RF signals – and that includes the connection between the device under test and the oscilloscope. For this, probes are normally used. They make the connection and ensure that the signal is passed on with as little distortion as possible, without loading the circuit heavily. To do this, they reduce the signal voltage (e.g. in the ratio 10:1), match resistance and capacitance, and often contain compensation for high frequencies.

A probe consists of a body shaped like a handle, comparable to a ballpoint pen. Various hooks or needles can be fitted to its tip to make contact with the measuring point. The earth connection is made with a crocodile clip (see Figure [ref:a_oszilloskop_messung]). Figure [ref:a_oszilloskop_tastkoepfe] shows three examples of such probes. High-quality models are correspondingly expensive, since they must offer high bandwidth, minimal signal distortion and precise mechanics.

<margin>
[photo:224:a_oszilloskop_messung:Measuring with a probe. The probe tip can be seen between diodes D1 and D2, and further to the left the crocodile clip for the earth connection.]
</margin>

<margin>
[photo:223:a_oszilloskop_tastkoepfe:Probes with various probe tips. The crocodile clips were removed for this photograph.]
</margin>

The simplest probes connect the probe tip directly to the measuring input. They are called 1:1 probes, because the voltage at the tip reaches the oscilloscope unchanged. Probes for high frequencies are of more elaborate construction. They divide the input voltage down to a smaller value, often one tenth. If you measure a voltage of 10 V with such a 10:1 probe, 1 V is displayed on the screen.

<indepth>
On some oscilloscopes you can set the division ratio of the probe. The actual voltage is then displayed on the screen. Passive 10:1 probes contain, among other things, a $\qty{9}{\mega\ohm}$ resistor in the signal path. Oscilloscopes usually have an internal resistance of $\qty{1}{\mega\ohm}$. This gives a 10:1 potential divider. In addition, there is a small variable capacitor in the probe or in the connector. It is used to match the capacitance of the probe and cable to the measuring input, and is adjusted so that a square-wave signal appears on the screen with as little distortion as possible. Besides the passive probes described here, there are several other types. There are, for example, probes with matched $\qty{50}{\ohm}$ coax cable. They are particularly well suited to very high frequencies, but have only a relatively low internal resistance. Active versions solve this problem by amplifying the signal directly in the probe.
</indepth>
