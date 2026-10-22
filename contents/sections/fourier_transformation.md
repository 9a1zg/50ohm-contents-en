Signals can be represented in different ways. Up to now we have often looked at the *time domain*. This shows how, for example, the voltage of a signal changes with time. The same signal can, however, also be looked at in the *frequency domain*. This no longer shows the variation with time, but which frequency components the signal is made up of and how strongly each of them is present. This representation is also called the *frequency spectrum*. It is based on the fact that periodic signals can be described as a superposition of sine waves of different frequency, amplitude and phase. A pure sine-wave signal, for example, consists of only a single frequency and therefore appears in the frequency spectrum only at that frequency.

The *Fourier transform* makes it possible to change between the time and frequency domains. It breaks a signal down mathematically into its individual frequency components. For digital, discrete-time signals, the *discrete Fourier transform* (DFT) is used for this. Computing a DFT directly can be very laborious for a large number of samples. The *fast Fourier transform* (FFT) provides a much more efficient algorithm for computing the DFT. That is why the FFT is often used in software and digital hardware, for example to determine the frequency spectrum of a signal.

<indepth>
Non-sinusoidal waveforms consist of several frequency components. Sharp changes and edges in the waveform in particular require additional high-frequency components. The following applet can be used to investigate how different sine waves are superimposed and how different waveforms arise from them.

[include:fourier]
</indepth>

[question:AF630]

---

The relationship between the time and frequency domains becomes particularly clear with signals that have sharp edges. An ideal square-wave signal, for example, can be built up from a fundamental and several harmonics. Besides the fundamental frequency, the odd multiples of the fundamental frequency occur. Their amplitudes become smaller as the frequency increases.

These harmonics also matter in transmitters. If, for example, an ideal square-wave signal were fed directly to an antenna, its harmonics would be radiated as well as the wanted fundamental frequency. A low-pass filter can suppress the unwanted higher frequency components, so that mainly the wanted fundamental reaches the antenna.

For some typical periodic waveforms the frequency spectrum can be described particularly simply. We consider idealised waveforms without a DC component:

* A *sine-wave signal* consists of only a single frequency. Only the fundamental frequency $f$ therefore appears in the frequency spectrum.
* A *square-wave signal* consists of the fundamental frequency and the *odd multiples* of the fundamental frequency. It therefore contains the frequencies $f$, $3\cdot f$, $5\cdot f$, $7\cdot f$ and so on. The amplitudes of the harmonics become smaller as the frequency increases.
* A *sawtooth signal* contains both the even and the odd multiples of the fundamental frequency. It therefore contains $f$, $2\cdot f$, $3\cdot f$, $4\cdot f$, $5\cdot f$ and so on. Here, too, the amplitudes become smaller as the frequency increases.
* A *triangular-wave signal*, like the square-wave signal, contains only the odd multiples of the fundamental frequency, i.e. $f$, $3\cdot f$, $5\cdot f$, $7\cdot f$ and so on. The amplitudes of the higher frequency components, however, fall off much faster than with the square-wave signal.

The waveforms can therefore also be told apart by their frequency spectrum. A single spectral component points to a sine wave. If odd multiples occur, then in the examination questions it is always a square-wave signal.

[question:AB404]
[question:AB405]
[question:AB406]
[question:AB407]