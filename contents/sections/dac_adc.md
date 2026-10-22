This section shows how analogue signals are converted into digital values and digital values back into analogue signals. *A/D converters* (analogue-to-digital converters) and *D/A converters* (digital-to-analogue converters) are used for this. Figure [ref:a_adc_dac] shows the block diagrams of an A/D and a D/A converter.

<margin>
[picture:1130:a_adc_dac:A/D and D/A converters]
</margin>

An A/D converter samples an analogue input signal at particular moments and produces from it digital numerical values, which can then be processed digitally by other parts of a circuit.

Since an A/D converter works with only a limited number of possible digital values, it can capture the amplitude of an analogue input signal only in particular steps. Recall the example used earlier of the dimmer and the step switch. If the actual value lies between two possible levels, it has to be assigned to one of them. This gives rise to a *quantisation error*.

[question:AF607]

---

The number of possible levels of an A/D converter is called its *resolution*. It is often stated in bits (unit: $\unit{\bit}$). If a converter can distinguish $\num{256}$ different values, for example, it has a resolution of $\qty{8}{\bit}$, because $\num{256}$ different values can be represented with $\qty{8}{\bit}$. A $\qty{16}{\bit}$ converter can already distinguish $\num{65536}$ different values.

For signals that can take both positive and negative values, part of these values is typically used for the positive and part for the negative signal range.

Figure [ref:a_adc_4bit] shows a sine-wave signal that has been digitised by an A/D converter with a resolution of $\qty{4}{\bit}$ and then converted back into an analogue signal. Figure [ref:a_adc_12bit] shows the same sine-wave signal, but digitised by an A/D converter with a resolution of $\qty{12}{\bit}$ and then converted back into an analogue signal. It can be seen clearly that the additional $\qty{8}{\bit}$ lead to a much finer resolution (better by a factor of 256), so that the reconstructed signal already comes very close to the original sine-wave signal.

<margin>
[picture:300:a_adc_4bit:Sine-wave signal digitised by a 4-bit A/D converter, followed by D/A conversion]
[picture:299:a_adc_12bit:Sine-wave signal digitised by a 12-bit A/D converter, followed by D/A conversion]
</margin>

[question:AF608]

Another important property of an A/D converter is the timing accuracy of the sampling. The individual samples should be taken as exactly as possible at the intended intervals of time. This requires a sampling clock generator that is as stable as possible.

In practice, however, the actual sampling instants can deviate slightly from the ideal instants. These fluctuations in time are called *jitter*. Jitter can lead to additional errors and so to additional noise in the digitised signal. The same mechanism occurs on the side of the D/A converter. There, jitter leads to additional noise in the analogue signal.

[question:AF621]

---

The counterpart of the A/D converter is the *D/A converter*. It produces an analogue signal again from a digital data stream, or from digital samples.

A D/A converter, too, cannot produce any number of different output values. As with the A/D converter, it has a particular resolution in bits and so only a finite number of possible output values.

A D/A converter can, moreover, produce voltages only within a particular range of values, for example from $\qty{0}{\volt}$ to $\qty{1}{\volt}$ or from $\qty{-2}{\volt}$ to $\qty{2}{\volt}$.

In a linear D/A converter, the possible output values are spread evenly over this voltage range. If a D/A converter has a resolution of $\qty{4}{\bit}$, for example,

$\num{2^4}=\num{16}$

possible levels are available.

[question:AF609]

If these are spread over a voltage range from $\qty{0}{\volt}$ to $\qty{1}{\volt}$, there are $\num{15}$ steps in all between the $\num{16}$ levels. The step size is therefore

$\frac{\qty{1}{\volt}}{16-1}\approx\qty{67}{\milli\volt}.$

[question:AF611]
[question:AF610]

---

A/D and D/A converters are used, for example, in SDR receivers and transceivers. Analogue input signals are first digitised by an A/D converter and then processed digitally. If an analogue signal is to be produced from them again, the digital values are converted back into analogue voltage values by a D/A converter.

It can happen that an input signal uses only a small part of the available range of values of an A/D converter. In this case, correspondingly, only some of the available digital levels are used.

Conversely, an input signal can exceed the maximum range of values of an A/D converter. Values above the maximum input voltage that can be captured can then no longer be represented correctly and are represented only by the maximum possible value. This effect is called *clipping*. In the waveform, the affected parts therefore appear cut off.

A D/A converter, too, cannot produce an output voltage outside its intended range of values.

The higher the resolution of an A/D or D/A converter, the more finely different amplitude values can be represented digitally, or converted back into analogue voltage values. With a low resolution, on the other hand, only a few possible levels are available, so that the steps become more clearly visible.

[question:AF613]
[question:AF612]
[question:AF614]