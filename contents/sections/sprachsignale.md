From here on, we will deal mainly with the modulation of speech. To do so, we first have to understand what speech actually consists of. When we speak, many different low and high, quiet and loud tones arise as sound waves. We call this a *speech signal*.

When we speak into a microphone, it converts the speech signal. The low and high, quiet and loud tones become slow and fast electrical oscillations with small and large amplitudes. The speech signal is no longer present as a sound wave but as an electrical oscillation, and can be processed in the radio.

<webmargin>
[picture:742:n_sprachspektrum:Human speech in the amplitude spectrum, the low tones on the left and the high tones on the right]
</webmargin>

In Figure [ref:n_sprachspektrum] we see a typical speech signal as an amplitude spectrum. The frequency range from $\qtyrange{0}{20}{\kilo\hertz}$ is shown. The curve represents the amplitude at each frequency. It is easy to see that speech does not contain arbitrarily high frequencies. For radio transmission, an even narrower frequency range is often used.

[include:spektrum_sprachsignale]

---

<margin>
[picture:730:n_sprachspektrum_symbolisch:Symbolic representation of the audio spectrum]
[picture:475:n_sprachspektrum_beispiel:Example of an audio spectrum]
</margin>

In Figure [ref:n_sprachspektrum_symbolisch] we see the symbolic representation of a speech spectrum. On the X axis, different frequencies are shown from left to right. Low tones with lower frequencies are further to the left than high tones with higher frequencies, which are further to the right. On the Y axis, the volume of each frequency is shown from bottom to top; in technical language we call this the amplitude. The higher up, the louder the tone.

Figure [ref:n_sprachspektrum_beispiel] gives a concrete example. It can be read from it that the frequency range used is $\qtyrange{300}{2700}{\hertz}$. The "width" of the signal, by the way, is called the bandwidth and is given in hertz ($\unit{\hertz}$). In this case the bandwidth is $\qty{2700}{\hertz}$ – $\qty{300}{\hertz}$ = $\qty{2400}{\hertz}$.

We will use this example speech signal to modulate carriers. A signal with which a carrier is modulated is called the *modulating signal*.