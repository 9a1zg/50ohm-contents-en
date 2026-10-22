A phase-locked loop (PLL) can, for example, synchronise a variable and potentially unstable VCO with a stable reference oscillator (G). To do this, it compares the phases of the two signals and corrects the VCO so that a stable output frequency results. In amateur radio, PLLs are used above all for stable and precise frequency generation in transmitters and receivers, for instance for channel selection, for generating mixing frequencies and for synchronising oscillators.

A PLL consists essentially of the following components:

* *Phase detector*: compares the phases of the signals from the VCO and from the reference oscillator.
* *Low-pass filter*: converts the pulses produced by the phase detector into a DC voltage.
* *VCO*: generates the output signal, whose frequency is controlled by the DC voltage from the low-pass filter.

[question:AD701]

Optionally, the PLL can be supplemented by a *frequency divider* in order to synchronise the frequency of the VCO to multiples of the reference frequency.

<margin>
[picture:45:a_oszillator_pll:Diagram of a phase-locked loop (PLL)]  
</margin>

---

The phase detector measures the phase difference between the signals of the VCO ($f_\mathrm{out}$) and the reference oscillator ($f_\mathrm{ref}$). If there is a phase error, it outputs pulses that correspond to the error. These pulses are smoothed by the low-pass filter and converted into a proportional DC voltage. This DC voltage serves as the control signal for the VCO and corrects its frequency, so that the phase difference is gradually reduced to zero. When this state has been reached, the PLL is said to be "locked", i.e. in a *stable state*. In the stable state of the PLL, the frequencies and phases of the two signals are identical. The following applies:

$f_\mathrm{ref}=\frac{f_\mathrm{out}}{n}$

The output frequency is stable and corresponds essentially to the reference frequency or a multiple of it (depending on the division ratio selected on the frequency divider).

A simple example using Figure [ref:a_oszillator_pll] makes the principle clear: the reference oscillator supplies a frequency of $f_\mathrm{ref}=\qty{10}{\mega\hertz}$ at point A. The output frequency of the VCO is divided at point C by the frequency divider with the division ratio $n=100$. When the PLL is locked, i.e. in the *stable state*, the frequencies at points A and B are equal. This gives the output frequency:

$f_\mathrm{out}=n\cdot f_\mathrm{ref}=100\cdot\qty{10}{\mega\hertz}=\qty{1}{\giga\hertz}$

The VCO therefore generates a frequency of $\qty{1}{\giga\hertz}$, which is divided down to $\qty{10}{\mega\hertz}$ by the frequency divider and compared with the reference frequency.

<indepth>
A PLL can be built with analogue or digital techniques, or as a mixture of the two. Radios often combine digital phase detectors and frequency dividers with an analogue loop filter and VCO.
</indepth>

[question:AD702]

The accuracy and stability of the PLL output frequency depend primarily on the quality of the reference oscillator, which is usually a crystal oscillator.

[question:AD705]

A PLL can be set to different frequencies by means of the frequency divider. This makes it possible to generate the output frequency as an integer multiple of the reference frequency. The smallest selectable frequency step is equal to the frequency of the reference oscillator, since the division can only be done in whole-number steps. In an FM radio with a channel spacing of $\qty{12.5}{\kilo\hertz}$, a comparison frequency of $\qty{12.5}{\kilo\hertz}$ can therefore be used. If the division ratio $n$ is increased or decreased by one, the output frequency changes accordingly by $\qty{12.5}{\kilo\hertz}$. In this way the PLL can be set to the individual radio channels.

[question:AD703]

To reach a particular output frequency for a given reference frequency, the division ratio is chosen so that the same frequency is present at both inputs of the phase detector. This allows the division ratio needed for the desired output frequency to be calculated.

[question:AD704]