In A/D and D/A conversion, analogue and digital signal processing are joined together. Analogue filters are needed both before the A/D converter and after the D/A converter. Figure [ref:a_adc_dac_filter] shows the whole signal chain. On the input side, before the A/D converter, there is an *anti-aliasing filter*. It limits the frequency range of the analogue input signal before the signal is sampled. After the digital signal processing, the D/A converter produces an analogue signal again. A *reconstruction filter* following it removes unwanted high-frequency signal components. We look at why both filters are needed in the following section.

<margin>
[picture:1131:a_adc_dac_filter:A/D and D/A conversion with anti-aliasing and reconstruction filters]
</margin>

---

From the lesson on the sampling theorem we know that a signal must be sampled at a sufficiently high sampling rate. For a signal whose highest frequency to be captured is $f_\mathrm{max}$, the sampling rate must be greater than $2\cdot f_\mathrm{max}$.

Via an antenna, however, we usually receive many different signals – including some with frequencies above the frequency range that we actually want to process. If such signal components reach the A/D converter although its sampling rate is not sufficient for these frequencies, they can appear in the digital signal as other frequencies that are not actually present. These are called *aliases*.

To prevent this, an *anti-aliasing filter* is used ahead of the input of the A/D converter. Depending on the application, this is, for example, a low-pass or band-pass filter. A band-pass filter could be used for speech, for example. The filter must sufficiently suppress unwanted signal components that could lead to aliasing in sampling. In particular, frequency components above half the sampling frequency must not reach the A/D converter unhindered.

[question:AF622]
[question:AF623]

<indepth>
A vivid example of *aliasing* is also met in everyday life with digital pictures. If you photograph very fine, regularly repeating structures with a camera, for example a close-meshed grid, a fabric with fine stripes or a fly screen, larger patterns that are not present in the original at all can suddenly appear in the picture. These are called *moiré patterns*.

The cause is similar to that in sampling an electrical signal. A camera sensor cannot capture a picture at any number of points, but has only a finite number of pixels. If a structure is finer than the spatial resolution of the sensor, it is no longer sampled unambiguously. As a result, the fine structure that is actually present can apparently turn into a different, coarser structure.

In the A/D converter the same principle acts on the time axis: if too high a signal frequency is sampled at too low a sampling rate, a different, lower frequency appears in the digitised signal that was not originally present at all.

A moiré pattern can therefore be regarded as a visible example of how inadequate sampling gives rise to new, apparent structures.

% TODO: Bild besorgen
%<margin>
%[picture:XXXX:a_moire:Moiré-Muster als Beispiel für räumliches Aliasing]
%</margin>
</indepth>

---

The A/D converter also needs a clock generator, which is also called the sampling clock generator. This determines the moments at which the input signal is sampled and so determines the sampling rate. The sampling rate can be fixed or can be controlled, for example, by a microcontroller.

<margin>
[picture:1132:a_anit_alias:Anti-aliasing filter, A/D converter and clock generator]
</margin>

[question:AF620]

---

On the other side of the digital signal processing, the D/A converter carries out the reverse process. It converts the digital samples back into analogue voltage values. Since the individual values are output only at fixed intervals of time, the output of the D/A converter at first does not give an ideally smooth waveform.

The discrete-time output gives rise not only to the wanted signal but also to unwanted higher-frequency signal components (e.g. in Figure [ref:a_adc_4bit], where the fast transitions between the discrete values of the output signal contain the high-frequency components). To suppress these, a *reconstruction filter* is used after the D/A converter. Here, too, a low-pass or band-pass filter, for example, can be used, depending on the application.

The reconstruction filter passes the wanted frequency range and suppresses the unwanted higher-frequency signal components of the D/A converter. As a result, the output again carries an analogue signal that is as clean as possible (see Figure [ref:a_adc_12bit]; the reconstruction filter smooths the signal).

[question:AF624]
[question:AF625]

<margin>
[picture:300:a_adc_4bit:Signal before the reconstruction filter]
[picture:299:a_adc_12bit:Signal after the reconstruction filter]
</margin>
