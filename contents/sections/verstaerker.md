In the chapter on transistors we have already learnt that a small base current $I_\text{B}$ can be used to control a much larger collector current $I_\text{C}$. This principle can be used to build an amplifier for electrical signals. Depending on the type of circuit, transistors can amplify signals of all kinds – be they digital signals, audio-frequency (AF) or radio-frequency (RF) signals. Amplification means that the output power of a signal is greater than its input power, and this is the basic characteristic of an amplifier.

---

Figure [ref:e_nf_verstaerker] shows an audio-frequency amplifier (AF amplifier) intended to amplify audio signals from the radio for a loudspeaker. This is easy to see from the loudspeaker symbol in the circuit. RF power amplifiers are used, for example, to amplify the transmitted signal.

<margin>
[picture:763:e_nf_verstaerker:Circuit diagram of an AF amplifier]  
</margin>

[question:ED402]
[question:ED403]

Since the output power is greater than the input power, energy must always be supplied to an amplifier. A voltage source with a suitable rating is therefore required.

[question:ED401]

---

For an amplifier to be called *linear*, it must have the property that when the input signal doubles, the output signal of the amplifier doubles too.
Departures from linearity are as a rule unwanted, and can only be tolerated with modes such as FM (in which the information in the signal is carried not by the amplitude but only by the frequency). If an amplifier does not work linearly, its output signal contains frequencies that are not present in the input signal (known as splatter). At AF this shows up as distortion. At RF, harmonics of the amplified signal are produced. Both are unwanted. Figure [ref:e_verstaerker_linearitaet] shows an example of how a sine-wave signal is deformed by non-linear behaviour. 

<margin>
[picture:828:e_verstaerker_linearitaet:The input signal is amplified. Where it is limited by a lack of linearity, the output signal is deformed.]
</margin>

[question:EF403]

The linearity of a transmitter likewise requires a power supply that is stabilised and decoupled from other stages, in order to avoid unwanted feedback.

[question:EF405]

AF amplifiers are found not only at the loudspeaker of a radio but also at the microphone. There they are used, for example, to amplify the microphone signal. Usually, the lower (below $\qty{300}{\hertz}$) and higher frequency components (above $\qty{3}{\kilo\hertz}$) of the microphone signal are already suppressed within the microphone amplifier by a band-pass response, in order to limit the bandwidth of the AF signal and to suppress lower frequency components such as mains hum (see Figure [ref:e_frequenzgang_mikrofonverstaerker]). For good speech intelligibility in voice communication, an audio bandwidth of approx. $\qtyrange{2.5}{3}{\kilo\hertz}$ is needed.

<margin>
[picture:246:e_frequenzgang_mikrofonverstaerker:Typical frequency response of an amateur radio microphone amplifier]
</margin>

[question:EF308]
[question:EF307]