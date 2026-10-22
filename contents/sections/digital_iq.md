In one of the previous chapters we met the I/Q representation and the I/Q modulator. In a digital system, the two components I and Q are processed as two separate digital data streams. These can be generated, modified and evaluated by digital signal processing.

On the receiving side, the input signal is mixed for this purpose with two signals of the same frequency that are phase-shifted by $\qty{90}{\degree}$ relative to each other. This produces an I signal and a Q signal. Each of the two signals is then digitised by an A/D converter and can afterwards be processed further digitally. On the transmitting side the process works in reverse: digital I and Q data streams are converted into analogue signals by two D/A converters and then fed to an I/Q modulator.

A digital I/Q data stream can represent a frequency range around a particular centre frequency. Frequencies below the centre frequency are described by negative frequency offsets, and frequencies above the centre frequency by positive ones.

If, for example, an input signal is mixed with two signals of $\qty{435}{\mega\hertz}$ each, phase-shifted by $\qty{90}{\degree}$ relative to each other, the resulting I/Q data stream represents a frequency range around the centre frequency of $\qty{435}{\mega\hertz}$.

How wide this frequency range is depends on the sampling rate. If both I and Q are sampled at a sampling rate of $f_\mathrm{S}$, a frequency range of, ideally,

$-\frac{f_\mathrm{S}}{2}\text{ to }+\frac{f_\mathrm{S}}{2}$

around the centre frequency can be represented. The total bandwidth that can be represented is thus equal to the sampling rate $f_\mathrm{S}$.

If, for example, I and Q are each sampled at $\qty{10}{\mega\sample\per\second}$, the I/Q data stream can represent a frequency range from $\qty{-5}{\mega\hertz}$ to $\qty{+5}{\mega\hertz}$ around the centre frequency. With a centre frequency of $\qty{435}{\mega\hertz}$ this corresponds to a frequency range from $\qty{430}{\mega\hertz}$ to $\qty{440}{\mega\hertz}$.

[question:AF634]
[question:AF635]
[question:AF636]