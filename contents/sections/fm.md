In frequency modulation (FM), a modulating signal is modulated onto the carrier by changing its frequency. The amplitude of the carrier, on the other hand, is not changed and ideally remains constant. 

<margin>
[picture:711:n_fm_wasserfall:Signal of an FM amateur radio transmission (speech)]
</margin>

<margin>
[picture:357:n_fm_frequenzmodulation:Frequency modulation]
</margin>

[question:NE301]
[question:NE302]
[question:NE303]

The louder you speak into the microphone, i.e. the larger the amplitude of the modulating signal, the greater the change in the carrier frequency upwards and downwards. As a result, the occupied bandwidth of the emission also increases.

---

The maximum change in the carrier frequency is called the *frequency deviation*, or *deviation* for short. On some radios it can be set, but on others it cannot. Often it is also possible to switch between two fixed values: "normal" FM and narrowband FM (NFM), which occupies only about half the bandwidth.

<indepth>
The *frequency deviation* is given in Hz, just like the bandwidth, but must not be confused with it. The frequency deviation is the maximum change in the carrier frequency. The bandwidth is approximately twice the sum of the deviation and the bandwidth of the AF signal. Example: an AF signal with a bandwidth of $\qty{3}{\kilo\hertz}$ is modulated with a deviation of $\qty{3}{\kilo\hertz}$. This gives a bandwidth of:
$2 \cdot (\qty{3}{\kilo\hertz} + \qty{3}{\kilo\hertz}) = \qty{12}{\kilo\hertz}$
</indepth>

In this connection the IARU band plan should also be taken into account, since it gives the maximum recommended bandwidth of an emission in the various frequency ranges. For example, in the FM telephony segment of the $\qty{2}{\meter}$ band, no more than $\qty{12}{\kilo\hertz}$ of bandwidth should be occupied. This corresponds to NFM. The following question can easily be solved with this knowledge and the IARU band plan, which is available as an aid in the examination.

[question:BC216]

If the deviation cannot be set, or cannot be set small enough, this can in practice mean that an emission occupies more bandwidth than is intended for the frequency range. Many older handhelds and mobile transceivers in particular have a fixed deviation that results in up to $\qty{25}{\kilo\hertz}$ of bandwidth being occupied.

In such situations, it helps to speak more quietly into the microphone. Then the amplitude of the modulating signal, and so the change in the carrier frequency, is not as large, and as a result the emission occupies less bandwidth.

[question:NE306]

Since the amplitude of the carrier is not changed, the modulation does not change the transmit power either. As long as you press the PTT button, the transmit power is at its maximum, regardless of whether you speak into the microphone not at all, quietly or loudly. This has the advantage that interference does not make the volume of the speech signal fluctuate.

[question:NE304]

