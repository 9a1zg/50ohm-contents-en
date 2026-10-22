In the past, so as not to have to build and tune separate oscillators for each frequency range in multiband amateur transmitters, the principle of frequency multiplication was used. A stable oscillator was operated on the frequency of the lowest band (e.g. $\qty{3.5}{\mega\hertz}$), and its output signal was then converted to each of the desired amateur bands by means of frequency multipliers. It is an advantage here that the individual bands are in fixed ratios to one another (e.g. $\qty{3.5}{\mega\hertz}$, $\qty{7}{\mega\hertz}$, $\qty{14}{\mega\hertz}$ etc.) and are mostly integer multiples of the lowest band. As a result, harmonics also fall into an amateur band again, which the regulatory authorities are quite happy with, as it avoids interference to other services from harmonics. In general, oscillators with high stability are easier to design and build at low frequencies than at high frequencies. 

---

Figure [ref:n_f_vervielfacher] shows the block diagram of a frequency multiplier with a factor of $2$, in which the input frequency of $\qty{3.5}{\mega\hertz}$ is raised to $\qty{7}{\mega\hertz}$. A frequency multiplier is typically based on a non-linearity (e.g. a diode), which deliberately produces harmonics of the input signal; the desired multiple of the frequency is then selected from these with a band-pass filter.

<margin>
[picture:1042:n_f_vervielfacher:Block diagram of a frequency multiplier]
</margin>

A chain of frequency multipliers is often used to obtain the desired multiplication factors. When multipliers are connected in series, the individual factors are multiplied together.
Conversely, such a circuit can of course also be worked backwards. You then have to divide by the corresponding individual factors.

[question:EF303]
[question:EF302]
[question:EF301]