In Class E we have already met the superheterodyne receiver. In this class we now want to look at the double-conversion superheterodyne receiver. Unlike the single-conversion superhet, the double-conversion superhet uses 2 intermediate frequencies, as shown in Figure [ref:doppelsuper_blockschaltbild].

<margin>
[picture:810:doppelsuper_blockschaltbild:Block diagram of a double-conversion superhet]
</margin>

Using a high first IF makes good image rejection possible, as described in the previous section. The two possible receive frequencies are then very far apart, and the unwanted receive frequency (image frequency) can easily be suppressed by input filters ahead of the first mixer. 

Using a low 2nd IF, a high selectivity of the receiver can be achieved in the 2nd step, since filters with a high Q and steep skirts are technically very easy to make for low frequencies.

In an HF receiver, depending on the receiver concept, the first IF and the highest wanted receive frequency should also be as far apart as possible, to avoid direct reception of the IF via the antenna. The 1st IF should therefore be twice the maximum receive frequency.

<tip>
An extension of the double-conversion concept would be the triple-conversion superhet, in which a low 3rd IF is formed. This can be useful for special demodulation methods or for implementing interference-suppression methods (notch filters). The intermediate frequencies and oscillator frequencies are then calculated in the same way as for the double-conversion superhet.
</tip>

[question:AF112]
[question:AF113]

After the first mixer, a very narrow filter tuned to the 1st IF can be used to improve the strong-signal performance. This filter is called a *roofing filter*. The bandwidth of the roofing filter must be at least as large as the largest bandwidth required by the intended modes.

[question:AF114]
[question:AF116]

The double-conversion superhet is made up of the following functional blocks:

1. RF section with preselection
2. First mixer with VFO to form the first IF. The frequency of the VFO can be either above or below the wanted receive frequency (offset from it by the 1st IF in each case)
3. First IF amplifier with filter (roofing filter)
4. Second mixer with CO (crystal oscillator) to form the second IF. The frequency of the CO can be either above or below the 1st IF (offset from it by the 2nd IF in each case)
5. Second IF amplifier with filter (IF filter depending on the type of modulation/mode, usually switchable).
6. Product detector or demodulator (depending on the mode), with a BFO where necessary. This stage also generates a control voltage for controlling the input sensitivity of the receive path (AGC)
7. AF amplifier with loudspeaker output or headphone socket

[question:AF209]
[question:AF117]
[question:AF210]

To calculate the oscillator frequencies required for a wanted receive frequency, you have to bear in mind that the oscillator frequencies can each lie above or below the wanted input frequency of the mixer. There are therefore two possible solutions for each mixer stage.

1. Oscillator frequency = input frequency + output frequency
2. Oscillator frequency = input frequency - output frequency

With this knowledge, the following questions can be answered.

[question:AF120]
[question:AF118]
[question:AF119]