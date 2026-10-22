To reduce the maximum bandwidth of a transmitted SSB signal and to use the available frequency spectrum efficiently, the maximum AF modulation bandwidth of an SSB signal should not exceed $\qty{2.7}{\kilo\hertz}$. This allows a minimum spacing of $\qty{3}{\kilo\hertz}$ between SSB signals, for interference-free operation.

[question:AE208]
[question:AE209]

If an SSB signal is overdriven in the transmitter's modulator, this produces distortion that leads to spurious emissions. These spurious emissions are also known informally as "splatter" and can cause interference to neighbouring emissions, since the bandwidth of the transmitted signal then exceeds the required $\qty{2.7}{\kilo\hertz}$.
[question:AE205]

Every person's speech has an individual frequency spectrum. For the best possible intelligibility in SSB transmissions, speech frequencies in the higher range should be boosted and those in the lower frequency ranges attenuated. This is the job of an equaliser in the transmitter's microphone amplifier, which allows the frequency response of the modulating signal to be set individually. In this way, the frequency response of the microphone is matched optimally to the operator.
[question:AE213]

---

To assess the envelope shape of an SSB transmitter for quality and linearity, a two-tone signal can be used to modulate the SSB transmitter. The SSB transmitter is then modulated with an AF signal that consists of two superimposed audio frequencies. These audio frequencies must not be in an integer ratio to each other. The superposition produces maxima and minima (zero crossings) in the transmitted RF signal. For modulation, for example, a $\qty{700}{\hertz}$ and a $\qty{1200}{\hertz}$ tone can be used. When the RF signal is measured with an oscilloscope (across a load resistor), this gives an RF beat of $\qty{500}{\hertz}$, which should ideally be sinusoidal. The two-tone signal also allows the peak envelope power (PEP) of an SSB transmitter to be measured by displaying the waveform on the oscilloscope.

[question:AI304]

<margin>
[picture:1092:a_ssb_zweiton:Two-tone signal for assessing the envelope shape of an SSB transmitter]
</margin>

Figure [ref:a_ssb_zweiton] shows in 1. a single-tone signal, i.e. a simple sinusoidal AF tone. 2. and 3. show how this single-tone signal is converted to RF in AM and in SSB respectively. The SSB signal in 3. consists of a single RF component of constant amplitude, and so looks like an unmodulated RF carrier at a frequency shifted from that of the suppressed carrier. With such a single-tone signal, however, the quality and linearity of an SSB transmitter can be assessed only to a limited extent; in particular, no meaningful intermodulation products between several wanted signals occur.

4. shows a two-tone wanted signal, made up of two superimposed sine-wave tones of $\qty{700}{\hertz}$ and $\qty{1200}{\hertz}$. 5. and 6. show how this two-tone signal is converted to RF in AM and in SSB respectively. The SSB two-tone signal in 6. produces two RF components $\qty{500}{\hertz}$ apart. Their superposition produces a periodic beat in the RF envelope at the difference frequency of $\qty{500}{\hertz}$. This envelope allows the peak envelope power (PEP) to be measured and at the same time serves to assess the linearity of the transmitter, since non-linearities lead to additional intermodulation products in the spectrum.

[question:AE207]

For the following questions, the transmitter output power has to be determined as peak envelope power (PEP). The PEP is the RMS power that the transmitter delivers at the peak of the modulation envelope. So it does not refer to the mean power over the whole modulation, but to the power at the maximum of the envelope, as shown in Figure [ref:a_pep_hüllkurve]. The peak voltage for calculating the RMS power can be read from the oscillogram. Mind the probe's division ratio when doing so.

<margin>
[picture:875:a_pep_hüllkurve:Modulation envelope for calculating the power]
</margin>

% Tastkopf 1:1 PEP
[question:AI305]

% Tastkopf 10:1 PEP
[question:AI306]