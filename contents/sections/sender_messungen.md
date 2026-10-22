Important measurements on transmitters for the radio amateur are measurements of output power or the measurement of RF voltages in RF parts of a circuit. When transmitter output power is measured, the transmitter must be terminated with a defined impedance that matches its output impedance. In amateur radio the usual impedance (transmitter termination) is $\qty{50}{\ohm}$. The termination can also be part of the measuring circuit itself, but this only makes sense at low power.

RF voltages are measured with an RF probe, by diode rectification followed by smoothing of the resulting DC voltage with a capacitor after the diode. Figure [ref:hf_messkopf_0] shows the principle of an RF probe with simple rectification and smoothing of the DC voltage. The RF voltage is terminated at the input with the correct impedance by a resistor (or a combination of resistors). It is then rectified by a diode, whose output voltage is the peak value minus the forward voltage of the diode, and which is held in the capacitor that follows. Figure [ref:hf_messkopf_1] shows a home-built RF probe, Figure [ref:hf_messkopf_2] its circuit diagram.

<margin>
[picture:576:hf_messkopf_0:Principle of an RF probe with simple rectification and smoothing of the DC voltage]
[photo:338:hf_messkopf_1:Home-built RF probe by DL3JOP]
[photo:339:hf_messkopf_2:Circuit diagram of the RF probe by DL3JOP]
</margin>

[question:AI608]

At higher RF power, an attenuator with a suitable power rating must be connected ahead of it, to absorb most of the transmitter output power that is to be measured. The attenuator must be taken into account when the power is calculated.

[question:AI609]

---

For RF voltages and powers to be measured as accurately as possible, the measuring circuit used must first be calibrated. To do this, known reference signals are fed in and the differences between the actual and the measured value are determined. From these differences, frequency- and level-dependent correction values can be worked out and stored, for example, in a table like Table [ref:a_frequenzgang_messwerte].

In a later measurement, the value displayed is corrected by the appropriate correction value. If the measured values are given in $\unit{\dBm}$, the difference determined during calibration for the frequency concerned can, for example, be added to the measured value as a correction value in $\unit{\dB}$.

<margin>
| c: Frequency in MHz | c: Transmit power $\qty{-40}{\dBm}$ | c: Transmit power $\qty{-20}{\dBm}$ |
| 10   | $\qty{-40.24}{\dBm}$ | $\qty{-20}{\dBm}$    |
| 50   | $\qty{-40.24}{\dBm}$ | $\qty{-20}{\dBm}$    |
| 100  | $\qty{-40.26}{\dBm}$ | $\qty{-20.12}{\dBm}$ |
| 200  | $\qty{-40.26}{\dBm}$ | $\qty{-20.2}{\dBm}$  |
| 300  | $\qty{-40.51}{\dBm}$ | $\qty{-20.32}{\dBm}$ |
| 400  | $\qty{-40.46}{\dBm}$ | $\qty{-20.28}{\dBm}$ |
| 500  | $\qty{-40.84}{\dBm}$ | $\qty{-20.64}{\dBm}$ |
| 600  | $\qty{-40.7}{\dBm}$  | $\qty{-20.41}{\dBm}$ |
| 700  | $\qty{-40.7}{\dBm}$  | $\qty{-20.53}{\dBm}$ |
| 800  | $\qty{-40.8}{\dBm}$  | $\qty{-20.55}{\dBm}$ |
| 900  | $\qty{-40.37}{\dBm}$ | $\qty{-20.2}{\dBm}$  |
| 1000 | $\qty{-40.33}{\dBm}$ | $\qty{-20.09}{\dBm}$ |
| 1100 | $\qty{-40.12}{\dBm}$ | $\qty{-19.85}{\dBm}$ |
| 1200 | $\qty{-39.94}{\dBm}$ | $\qty{-19.62}{\dBm}$ |
| 1300 | $\qty{-39.69}{\dBm}$ | $\qty{-19.49}{\dBm}$ |
| 1400 | $\qty{-40.18}{\dBm}$ | $\qty{-19.79}{\dBm}$ |
| 1500 | $\qty{-40.13}{\dBm}$ | $\qty{-19.97}{\dBm}$ |
| 1600 | $\qty{-40.95}{\dBm}$ | $\qty{-20.62}{\dBm}$ |
| 1700 | $\qty{-41.55}{\dBm}$ | $\qty{-21.64}{\dBm}$ |
| 1800 | $\qty{-41.47}{\dBm}$ | $\qty{-20.92}{\dBm}$ |
| 1900 | $\qty{-43.1}{\dBm}$  | $\qty{-23.27}{\dBm}$ |
| 2000 | $\qty{-42.34}{\dBm}$ | $\qty{-21.89}{\dBm}$ |
[table:a_frequenzgang_messwerte:Measured levels as a function of frequency for the RF probe by DL3JOP]
</margin>

[question:AI612]

Let us now look at the calculation for these circuits in detail. With RF probes that have only one diode, what can be measured at the measurement output is the peak voltage of the RF voltage applied, minus the forward voltage of the diode used and minus the effect of any potential divider ahead of it. An RF probe with simple rectification followed by smoothing is calculated as follows:

The RF input signal is terminated at the input with the correct impedance by the resistor provided (or a combination of individual resistors). In the circuit shown (see Figure [ref:hf_messkopf_0]) the RF voltage is halved by the potential divider that follows (which also has an effect on the impedance). It is then peak-rectified by a diode, whose output voltage is the peak value minus the forward voltage of the diode, and which is held in the capacitor that follows.

---

[question:AI610]

<tip>
For all circuits with RF measuring heads you can simply assume that the input resistance is $\qty{50}{\ohm}$. You do not need to calculate it again; you can skip this step for the examination questions.
</tip>

Conversely, the power fed to the circuit can be calculated from the DC voltage measured. See whether you can work out the solution!

[question:AI611]

Besides RF probes with only one diode, there are circuits with two diodes. Their advantage is that both the positive and the negative peak of the RF signal are captured. As a result, a measuring voltage about twice as large as with simple peak rectification is available at the output. This is particularly helpful when small RF voltages are to be measured with a DC voltmeter connected after the probe.

[question:AI605]
[question:AI604]

The positive and the negative peak of the RF signal are captured separately and stored in capacitors. The two voltages add at the output. Ideally, the output voltage therefore corresponds to the peak-to-peak voltage of the RF signal:

$U_\mathrm{A} \approx U_\mathrm{SS} = 2\hat U$

In the real circuit, the forward voltages of the two diodes must also be taken into account. Approximately, therefore:

$U_\mathrm{A} \approx 2\hat U - 2U_\mathrm{F}$

If the RF voltage is to be worked out back from the output voltage measured, this gives:

$\hat{U} \approx \frac{U_\mathrm{A}+2U_\mathrm{F}}{2}$

From the peak value, the RMS value can then be calculated, and from that, with the resistance known, the RF power.

[question:AI607]
[question:AI606]

To show that a transmitter is radiating power through its antenna, a field-strength meter can be used. Here the RF received by a measuring antenna is fed to the diode and rectified by it. The rectified voltage is then fed through RF chokes to a capacitor, which holds the rectified voltage. The reading is given by a sensitive ammeter. The larger the needle deflection of the meter, the higher the RF field strength measured at the antenna. For exact measurements, both the measuring antenna and the field-strength meter must be calibrated.

[question:AI613]