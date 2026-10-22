Let us first look at how a receiver is constructed. To keep things simple, in Figure [ref:aufbau_empfaenger_blockdiagramm] we do not go down to the level of individual components, but look at blocks that each have a particular function. This kind of diagram is called a block diagram. In electrical engineering it is used to show complex equipment in a simplified overview. To do this, details that are not needed to understand the equipment as a whole are left out.

<margin>
[picture:736:aufbau_empfaenger_blockdiagramm:Block diagram of a simple receiver]
</margin>

<indepth>
The receiver shown here is called a tuned radio frequency (TRF) receiver (in German *Geradeausempfänger*, literally "straight-through receiver"). The German name comes from the fact that the frequency of the signal picked up by the antenna is not changed on its way to the demodulator.
</indepth>

---

Let us look at the individual blocks of the receiver in detail, one after the other from left to right:

1. Antenna: The antenna picks up a large number of radio waves and passes them on as electrical oscillations.
2. Band-pass filter: To filter out the wanted signal, a band-pass filter follows. It lets only the wanted frequency range through and blocks all other, unwanted frequencies.
3. RF amplifier: Next comes an amplifier that amplifies the signal that has been filtered out. This is a radio-frequency amplifier (RF amplifier), because the signal is at a high frequency, for example $\qty{144.3}{\mega\hertz}$.
4. Demodulator: The amplified signal is processed further by the demodulator. Demodulation is the counterpart of modulation. Whereas in modulation a signal (e.g. a speech signal) is modulated onto a radio-frequency carrier, demodulation does the opposite: the original signal is recovered from the modulated radio-frequency carrier. We then have, for example, the speech signal again that was spoken into the microphone at the transmitter. It is also called the audio-frequency signal, or AF signal for short, because it has comparatively low frequencies – for a speech signal, for example, frequencies below $\qty{20}{\kilo\hertz}$.
5. AF amplifier: The demodulated signal is then amplified. This time it is an audio-frequency amplifier (AF amplifier), which amplifies the signal for the loudspeaker. The symbol for the AF amplifier is the same as for the radio-frequency amplifier.
6. Loudspeaker: The loudspeaker now converts the signal from an electrical oscillation into a sound wave and so makes it audible again.

<indepth>
In the *band-pass filter* symbol, the two crossed-out waves indicate that frequencies above and below the wanted frequency range are blocked. The middle wave stands for the wanted frequency range being let through.
</indepth>

<indepth>
The *demodulator* is represented by the circuit symbol of the diode, which is the most important part of many demodulators. How a diode works is explained later, in the chapter on components and circuits.
</indepth>

[question:NF201]

Depending on exactly how a receiver is built, it has different properties. One important property is its sensitivity. This is the ability of the receiver to receive weak signals. The more sensitive a receiver is, the weaker the signals it can receive.

[question:NF303]
