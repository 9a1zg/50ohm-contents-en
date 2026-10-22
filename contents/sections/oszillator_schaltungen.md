Oscillators are among the most important circuit elements in amateur radio. They are, so to speak, the heart of every radio. Oscillators are used to generate RF oscillations in transmitters and receivers.

The core of an oscillator is an amplifying element whose *output signal is fed back to its input*.

For an oscillator to produce sustained (undamped) oscillations, *two basic conditions* must be met.
Firstly, the *output signal must be fed back in phase to the input point of the circuit*.
Secondly, the *amplitude of the fed-back signal must be at least as large* as that of the input signal. This is also expressed by saying that the so-called *loop gain must be greater than 1*, so that self-excitation is possible, which keeps the oscillation going.

[question:AD613]

<margin>
[picture:760:a_oszillator_schaltungen_oszillator:Circuit of a capacitive-feedback oscillator]  
</margin>

%TODO: Evtl. Bild 760 ableiten und noch um die 3 Punkte der Dreipunktschaltung ergänzen (am kapazitiven Spannungsteiler - oben, in der Mitte und unten)

The circuit shown in Figure [ref:a_oszillator_schaltungen_oszillator] is a capacitive-feedback three-point oscillator. The output signal is fed back from the emitter of the circuit to the base of the transistor through a capacitive potential divider. The frequency of the oscillator is determined mainly by the tuned circuit at the base (consisting of an inductor and a trimmer capacitor) and by the capacitive potential divider connected in parallel with the tuned circuit.
The circuit is a common-collector oscillator, since the collector is connected to chassis as far as AC is concerned.

[question:AD614]
[question:AD616]

To increase the frequency stability of an oscillator, its frequency-determining component (the tuned circuit) can be replaced by a crystal. Crystals can be made to oscillate both at their fundamental frequency and at their harmonic frequencies (overtones). For a crystal to be operated on an overtone, however, the amplifier must be designed to be frequency-selective (e.g. by using a tuned circuit). If there is no such tuned circuit, this shows that the crystal is operated at its fundamental frequency (see Figure [ref:a_oszillator_schaltungen_quarzoszillator] ).

<margin>
[picture:497:a_oszillator_schaltungen_quarzoszillator:Circuit of a crystal oscillator in common-collector configuration with the crystal operated at its fundamental frequency]  
</margin>

[question:AD617]

The oscillator signal should always be coupled out at the lowest-impedance point of an oscillator, so as to load the oscillator as little as possible. In a common-collector circuit, this is the emitter of the transistor.

[question:AD610]

An oscillator should always be followed by a so-called buffer stage, which decouples the oscillator from further parts of the circuit, so that its frequency is not affected by loading of the output. A buffer stage is usually designed as a common-collector circuit (emitter follower) and has a high input impedance, which loads the oscillator only minimally. At the buffer's output, the oscillator signal can then be processed further at low impedance.

Measurements on oscillators should always be made after the buffer stage, since otherwise the oscillator is loaded by parasitic capacitances and its frequency is affected as a result.

[question:AD615]
[question:AD619]
[question:AD618]










