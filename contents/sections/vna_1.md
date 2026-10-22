A simple multimeter is not suitable for measuring frequency-dependent resistances. Instead, a vector network analyser (VNA) can be used. This is an active measuring instrument that determines, for a large number of frequencies (an adjustable frequency range), how current and voltage relate to each other (the ratio of their amplitudes and the phase shift between voltage and current).

<margin>
[photo:201:e_vna_tiefpassmessung:Measurement from $\qty{0}{\mega\hertz}$ to $\qty{100}{\mega\hertz}$ of a low-pass filter with its cut-off frequency at $\qty{30}{\mega\hertz}$]
</margin>

---

This makes it possible, for example, to determine the frequency at which a tuned circuit or filter has a particularly high or particularly low resistance (or impedance) (see Figure [ref:e_vna_tiefpassmessung]). It is also possible to find the frequency at which an antenna is resonant, by looking at the SWR over a range of frequencies, as shown in Figure [ref:e_vna_swr].

<margin>
[photo:323:e_vna_swr:SWR measurement of an end-fed wire antenna. The SWR is close to $1$ at $\qty{14}{\mega\hertz}$]
</margin>

[question:EI201]
[question:EI202]
[question:EI203]
[question:EI204]

Many VNAs should be calibrated before use in order to obtain as accurate a measurement as possible.

[question:EI205]

---

For calibration, and also as a functional check, the "open-circuit" (infinite resistance), "short-circuit" (resistance close to zero) and "matched" (load resistance equal to the output resistance of the instrument) conditions are often measured.

<margin>
[photo:327:e_vna_solt:SOL(T) calibration kit. From left to right - Load, Open, Closed]
</margin>

With a line termination connected (e.g. a $\qty{50}{\ohm}$ terminating resistor), the VNA should display an SWR close to $\num{1}$, since no power is reflected. If nothing is connected to the test port, or if it is short-circuited, the result is an SWR close to infinity (total reflection).

[question:EI206]