We have already met diodes in various circuits. Now we look at how their non-linear characteristic can be used to modulate a radio-frequency carrier signal with an audio-frequency information signal.

If an RF signal and an AF signal are fed to a diode together, as shown in Figure [ref:a_am_modulator], the AF voltage affects the conductivity of the diode. As a result, the RF signal is passed on more or less strongly, depending on the instantaneous value of the AF. Its amplitude therefore varies in step with the AF signal.

As a result, two sidebands, above and below the carrier frequency, appear at the output besides the original RF carrier. A tuned circuit resonant at the carrier frequency suppresses further, unwanted frequency components. The output is then an amplitude-modulated (AM) signal.

<margin>
[picture:772:a_am_modulator:Simple AM modulator with diode and tuned circuit]
</margin>

<webonly>
The following simulation shows how the AM modulator works; the values have been chosen so that the RF and the AF can be seen clearly. The AF is at $\qty{500}{\hertz}$, the RF at $\qty{10}{\kilo\hertz}$. The amplitude of the RF signal is varied in step with the AF. The tuned circuit is tuned to the carrier frequency and suppresses unwanted frequency components. If you remove the tuned circuit, you will see a large number of mixing products. You can also try changing the AF frequency to $\qty{1}{\kilo\hertz}$ to see how the sidebands shift.

[include:applet_am_modulator]
</webonly>

<indepth>
An AM signal can also be described mathematically. To do this, we first consider a normalised sinusoidal AF signal

$m(t)=\cos(\omega t)$

with the angular frequency $\omega=2\pi f_\mathrm{m}$. With its amplitude $\hat U_\mathrm{m}$ and an additional DC component $U_\mathrm{G}$ this gives

$U_\mathrm{m}(t)=U_\mathrm{G}+\hat U_\mathrm{m}\cdot\cos(\omega t)$

This signal is now multiplied by the radio-frequency carrier signal

$U_\mathrm{T}(t)=\cos(\Omega t)$

with $\Omega=2\pi f_\mathrm{T}$. For the AM signal this gives:

$U_\mathrm{AM}(t)=\left(U_\mathrm{G}+\hat U_\mathrm{m}\cdot\cos(\omega t)\right)\cdot\cos(\Omega t)$

Multiplying out gives:

$U_\mathrm{AM}(t)=U_\mathrm{G}\cdot\cos(\Omega t)+\hat U_\mathrm{m}\cdot\cos(\omega t)\cdot\cos(\Omega t)$

With the relationship

$\cos(a)\cdot\cos(b)=\frac{1}{2}\left(\cos(a+b)+\cos(a-b)\right)$

the second term can be broken down further:

$U_\mathrm{AM}(t)=U_\mathrm{G}\cdot\cos(\Omega t)+\frac{\hat U_\mathrm{m}}{2}\left(\cos((\Omega+\omega)t)+\cos((\Omega-\omega)t)\right)$

This shows at once the three components of an AM signal: the first term describes the *carrier* at the frequency $\Omega$. The two other terms form the *upper and lower sidebands* at the frequencies $\Omega+\omega$ and $\Omega-\omega$.

The DC component $U_\mathrm{G}$ is what keeps the carrier present. Even when the information signal is momentarily zero, a carrier signal is still generated.

[picture:1127:a_am_modulation:Spectrum of an AM signal with carrier and two sidebands]

</indepth>

This principle becomes clear in the following question: a diode is fed with an AF signal and an RF signal at the same time, and the output signal is filtered with an LC tuned circuit.

[question:AD507]

---

With four diodes in a ring arrangement, a modulator can be built in such a way that the carrier is suppressed at the output. We have already met such a circuit as the *balanced mixer* in the second chapter on mixers. There it was used to convert an RF signal to an intermediate frequency. In the transmitter we now use the same basic principle to generate a modulated signal.

<margin>
[picture:759:a_balancemodulator:Balanced modulator with diode ring]
</margin>

A balanced mixer or balanced modulator can typically be recognised by the diode ring, as shown in Figure [ref:a_balancemodulator]. The diode ring is driven by the oscillator signal $f_\mathrm{OSZ}$. Depending on the polarity of the oscillator signal, one or the other of the two opposite pairs of diodes conducts.

As a result, the AF signal is passed to the output alternately with the same and with reversed polarity. In simplified terms, the AF signal is therefore multiplied by the oscillator signal.

The decisive advantage of the balanced circuit is *carrier suppression*: ideally, the components of the oscillator signal cancel each other out at the output. Without an AF signal there is therefore no output signal. When an AF signal is applied, on the other hand, the upper and the lower sideband are produced, while the carrier remains suppressed.

The output signal is called a *double-sideband suppressed-carrier signal* (DSB).

[question:AE206]
[question:AF302]
[question:AF308]
[question:AD510]

<indepth>
The carrier suppression of a balanced modulator can be described, in simplified form, by two symmetrical branches:

$u_1(t)=\left(U_G+\hat U_\mathrm{m}\cos(\omega t)\right)\cos(\Omega t)$

$u_2(t)=\left(U_G-\hat U_\mathrm{m}\cos(\omega t)\right)\cos(\Omega t)$

At the output, one signal is subtracted from the other:

$u_\mathrm{out}(t)=u_1(t)-u_2(t)$

This gives:

$u_\mathrm{out}(t)=U_G\cos(\Omega t)+\hat U_\mathrm{m}\cos(\omega t)\cos(\Omega t)-U_G\cos(\Omega t)+\hat U_\mathrm{m}\cos(\omega t)\cos(\Omega t)$

The two carrier components $U_G\cos(\Omega t)$ cancel. What remains is:

$u_\mathrm{out}(t)=2\hat U_\mathrm{m}\cos(\omega t)\cos(\Omega t)$

With $\cos(a)\cos(b)=\frac{1}{2}\left(\cos(a+b)+\cos(a-b)\right)$ it follows that:

$u_\mathrm{out}(t)=\hat U_\mathrm{m}\left(\cos((\Omega+\omega)t)+\cos((\Omega-\omega)t)\right)$

The output signal therefore contains only the upper and the lower sideband. The carrier at $\Omega$ is suppressed.
</indepth>

---

For the oscillator signal to cancel out as completely as possible at the output, the circuit must be symmetrical, that is, *balanced*. Even small differences in amplitude or phase between the two signal paths leave a remnant of the carrier at the output. The amplitude balance can be adjusted with a potentiometer, for example. For the phase adjustment, some circuits also use a trimmer capacitor. The aim of the adjustment is the highest possible carrier suppression, while the two modulation sidebands are retained.

<webonly>
The following applet shows the carrier balancing. When the slider on the right-hand side is moved, the carrier suddenly appears in the spectrum. 

[include:applet_dsp]
</webonly>

[question:AF309]

---

The balanced modulator forms the first stage of an SSB modulator and generates a DSB signal. It is followed, as the second stage, by a narrowband band-pass filter, as in Figure [ref:a_ssb_modulation]. This lets only one of the two sidebands through and suppresses the other. The result at the output is a single-sideband (SSB) signal.

<margin>
[picture:500:a_ssb_modulation:Block diagram of SSB modulation by the filter method]
</margin>

[question:AF306]
[question:AF304]
[question:AF303]
[question:AF305]

---

A good implementation for a radio that is to generate both USB and LSB is to design the band-pass filter for one fixed frequency range. Whether the upper or the lower sideband is filtered out is not decided by changing the filter but by the frequency of the oscillator in the balanced modulator. For this purpose, two different crystal oscillators are provided.

If, for example, the oscillator frequency $\qty{8998.5}{\kilo\hertz}$ is chosen for USB, the modulation produces two sidebands. The upper sideband is shifted exactly into the passband of the fixed filter, while the lower sideband lies outside the passband and is suppressed.

For LSB, the radio switches to the other crystal frequency, $\qty{9001.5}{\kilo\hertz}$. This shifts the whole DSB spectrum so that the lower sideband now falls into the passband of the same filter and the upper sideband is suppressed.

The decisive trick, then, is to leave the filter unchanged and instead to shift the position of the DSB signal by using different oscillator frequencies. As with the intermediate frequency of a receiver, this allows one high-quality filter, tuned to a fixed frequency, to be used for different frequency positions.

[question:AF307]

<margin>
<latexonly>
[picture:831:a_ssb_modulation_lsb:Frequencies with the filter method for LSB]
[picture:940:a_ssb_modulation_lsb:Spectrum with the filter method for LSB]
[picture:832:a_ssb_modulation_usb:Frequencies with the filter method for USB]
[picture:941:a_ssb_modulation_usb:Spectrum with the filter method for USB]
</latexonly>
<webonly>
[include:applet_dsp_filter]
</webonly>
</margin>

---

A *varactor diode* can be used to generate a frequency-modulated (FM) signal. In circuit diagrams it can be recognised by the small capacitor symbol next to the diode, as in Figure [ref:a_fm_modulator].

A varactor diode is operated in the reverse direction. Its capacitance depends on the reverse voltage applied. If it is used as part of the frequency-determining tuned circuit of an oscillator, a change in this voltage changes the resonant frequency of the tuned circuit and thus the frequency of the oscillator.

For frequency modulation, the AF signal is superimposed on the DC voltage across the varactor diode. Its capacitance then changes in step with the AF signal, and the oscillator frequency is shifted up and down accordingly. In this way a frequency-modulated signal is produced.

<margin>
[picture:155:a_fm_modulator:FM modulator with varactor diode]
</margin>

[question:AD508]
[question:AF310]

---

With large AF voltages it is easy to cause much larger changes in the oscillator frequency (FM "deviation") than are permitted. "Deviation" limiting, by setting and limiting the AF amplitude, is therefore necessary. Diodes connected in inverse parallel limit the voltage to about the knee voltage of the diodes. Figures [ref:a_fm_modulator_hub1] and [ref:a_fm_modulator_hub2] show an example.

<margin>
[picture:44:a_fm_modulator_hub1:Circuit for deviation limiting]
[picture:828:a_fm_modulator_hub2:Limiting of the signal]
</margin>

[question:AD509]