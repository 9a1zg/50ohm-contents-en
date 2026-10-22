In contrast to modulation, which takes place on the transmitting side, the demodulation of signals in the receiver converts a modulated signal back, e.g. into AF, so that it becomes audible, or produces a bit sequence in a digital transmission.

Depending on which type of modulation was used on the transmitting side, a corresponding demodulation must take place on the receiving side. There are various circuit concepts that make demodulation possible. We will look at how modulation works in the digital domain in a later chapter. In this chapter we will first deal with the demodulation of analogue signals.

Amplitude modulation (AM) offers the simplest form of demodulation of a radio-frequency signal.
AM signals can be demodulated by means of a so-called envelope detector, as in Figure [ref:demodulator_huellkurvendemodulator_am]. For this, the radio-frequency signal is first selected for the desired receive frequency, e.g. by means of a suitably tuned resonant circuit, and then rectified by a diode. A capacitor following the diode is charged to the instantaneous peak value of the signal and at the same time discharged, with a suitable time constant, through a resistor connected in parallel with it. This time constant is well above the period of the RF signal but well below the period of the AF signal.

<margin>
[picture:141:demodulator_huellkurvendemodulator_am:Envelope detector for demodulating AM signals]
</margin>

[question:AD501]

At terminal X in Figure [ref:demodulator_huellkurvendemodulator_am_2], the rectified peak voltage of the RF signal appears at each peak; between the peaks of the RF signal it falls slightly, according to the time constant of the resistor connected in parallel with the capacitor. The envelope of the signal thus corresponds to the AF modulated onto the carrier, overlaid, because of the time constant of the capacitor, with a sawtooth signal (carrier frequency), and corresponds to the signal in Figure [ref:demodulator_huellkurvendemodulator_am_abbx]. In the following AF processing stages (not shown), the remnants of this carrier frequency are then filtered out, so that the pure AF remains as the output signal (see Figure [ref:demodulator_huellkurvendemodulator_am_clean]).

<margin>
[picture:607:demodulator_huellkurvendemodulator_am_2:Envelope detector for demodulating AM signals, showing the IF input signal present at the input of the demodulator]
[picture:146:demodulator_huellkurvendemodulator_am_abbx:Demodulated signal at point X of the envelope detector]
[picture:147:demodulator_huellkurvendemodulator_am_clean:Filtered signal at the output of the envelope detector]
</margin>

[question:AD502]

---
<margin>
[picture:841:demodulator_flankendiskriminator:Tuned circuit used as a slope detector]

[picture:149:demodulator_flankendiskriminator_schaltung:FM slope detector]
</margin>

A circuit very similar to the envelope detector described above can be used to demodulate FM signals.
Starting from the intermediate frequency in the FM receiver, the signal passes, as in Figure [ref:demodulator_flankendiskriminator], into a tuned circuit whose resonant frequency $f_\text{res}$ is tuned slightly above or below the IF $f_\text{ZF}$. As a result, the FM signal to be demodulated lies on the slope of the tuned circuit's response, so that the frequency changes of the FM are converted into amplitude changes. The FM signal, now converted into an AM signal, is then demodulated by the following AM demodulator and made audible. This circuit, shown in Figure [ref:demodulator_flankendiskriminator_schaltung], is called a slope detector.

[question:AD504]

---

FM signals can also be demodulated by means of a PLL (phase-locked loop) (see Figure [ref:demodulator_pll]). In a PLL, a voltage-controlled oscillator (VCO) is locked to an input signal by a phase control loop so that it follows its frequency. When the frequency of the input signal changes (frequency modulation), the control voltage of the VCO follows the FM. This control voltage then corresponds exactly to the modulation of the FM signal, and thus to the AF modulated onto it, and can be taken from the PLL for further processing.

<margin>
[picture:77:demodulator_pll:PLL for demodulating FM signals]
</margin>

[question:AD505]

---

To demodulate SSB signals, a so-called product detector is used. This is essentially a ring mixer, which we have already met in the chapter on receivers, with the receiver's IF and a BFO (beat frequency oscillator) as its input signals. Mixing these two input signals (forming their product) produces, as one of the mixing products, the desired AF signal (SSB signal), which can be taken from the output for further processing. For the best possible intelligibility of the demodulated AF, the BFO must be tuned to the frequency of the suppressed carrier of the SSB signal.


<indepth>
[picture:153:demodulator_produktdetektor:Product detector for demodulating SSB signals]
[picture:1125:a_produktdetektor_spannung:Example of voltages at the product detector]

A so-called *product detector* is often used to demodulate an SSB signal. It can, for example, be built as a ring mixer. As its input signals it receives the SSB signal at the intermediate frequency (IF) and the signal of a *beat frequency oscillator (BFO)*.

How it works can be explained in simplified form with a switching mixer. The BFO signal switches the ring mixer alternately between two states. In simplified terms, the BFO can therefore be thought of as a signal that switches between the values $+1$ and $-1$, as shown in the upper trace of Figure [ref:a_produktdetektor_spannung].

As a result, the IF signal is alternately passed through unchanged or inverted in polarity. In the simplified representation, the IF signal can therefore be regarded as the product of the AF signal and the BFO switching signal:

$u_\mathrm{ZF}(t)=u_\mathrm{NF}(t)\cdot s_\mathrm{BFO}(t)$

In the product detector, this signal is multiplied by the BFO signal once again:

$u_\mathrm{ZF}(t)\cdot s_\mathrm{BFO}(t)=u_\mathrm{NF}(t)\cdot s_\mathrm{BFO}(t)\cdot s_\mathrm{BFO}(t)$

Since the simplified BFO switching signal only takes the values $+1$ and $-1$, the following holds:

$s_\mathrm{BFO}^2(t)=1$

So the original AF signal remains as the low-frequency component:

$u_\mathrm{NF}(t)=u_\mathrm{ZF}(t)\cdot s_\mathrm{BFO}(t)$

Besides the desired AF signal, the mixing process produces further high-frequency mixing products. These are suppressed at the output of the product detector by a low-pass filter.

For the original AF signal to be recovered at the correct pitch, the frequency of the BFO must be set to match the frequency of the suppressed carrier of the SSB signal.
</indepth>

[question:AD506]

