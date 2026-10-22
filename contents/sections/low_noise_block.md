A low-noise block converter (LNB) is often used for processing high frequencies in the $\unit{\giga\hertz}$ range in amateur radio communication via satellite. Figure [ref:a_lnb] shows a possible implementation of a QO-100 station. Here the very high receive frequency, which is typically received with a satellite dish, is already mixed down directly in the LNB to a much lower frequency, to avoid the high cable losses that would occur at high frequencies.

<margin>
[picture:1094:a_lnb:LNB (blue) and bias tee (red) in a QO-100 transceiver]
</margin>

[question:AF230]

An LNB is an active component that needs a power supply. This is usually provided directly via the coaxial cable leading to the LNB. For this, a so-called bias tee is fitted into the coaxial cable at the receiving station. Its job is to supply DC to the LNB and to separate the DC from the RF signal in the further signal path to the receiver.
An LNB can receive either horizontally or vertically polarised signals. Switching between the two polarisations is done by means of the level of the operating voltage supplied to the LNB. Usual values here are, for example, $\qty{12}{\volt}$ and $\qty{18}{\volt}$.

[question:AF231]