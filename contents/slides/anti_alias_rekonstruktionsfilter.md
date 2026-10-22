--- style="font-size: smaller;"

## Filters in A/D and D/A conversion

[picture:1131:a_adc_dac_filter:A/D and D/A conversion with anti-aliasing and reconstruction filters]

* Before the A/D converter: *anti-aliasing filter*
* After the D/A converter: *reconstruction filter*
* Both filters suppress unwanted frequency components

<note>
The figure shows the whole signal chain from an analogue input signal, through the digital signal processing, back to an analogue output signal.

The anti-aliasing filter is located before the A/D converter. The reconstruction filter is located after the D/A converter.

We now look in more detail at why both filters are needed.
</note>

---

## Aliasing at the A/D converter

* For sampling: $f_\mathrm{S}>2\cdot f_\mathrm{max}$
* Unwanted higher frequencies can also be present at the input
* If the sampling rate is too low for them, apparent frequencies arise
* These are called *aliases*

<note>
Via an antenna we usually receive not only the wanted signal but many other frequency components as well.

If the sampling rate is too low for one of these frequency components, it can appear after digitisation as a different frequency that was not present in the original signal at all.

We have already met this effect with the sampling theorem.
</note>

--- style="font-size: smaller;"

## Anti-aliasing filter

[picture:1131:a_adc_dac_filter_aa:A/D and D/A conversion with anti-aliasing and reconstruction filters]

* The filter is located *before* the A/D converter
* It limits the frequency range of the input signal
* Low-pass or band-pass filters can be used
* Critical frequency components must be suppressed sufficiently

<fragment>
In particular, frequencies above $\frac{f_\mathrm{S}}{2}$ must not reach the A/D converter unhindered.
</fragment>

<note>
The anti-aliasing filter prevents frequencies for which the sampling rate is not high enough from reaching the A/D converter.

Depending on the application, a low-pass or band-pass filter, for example, can be used for this. For speech signals, for example, a band-pass filter can make sense.

What matters is that frequency components that could lead to aliasing are sufficiently suppressed before digitisation.
</note>

---

[question:AF622]

---

[question:AF623]

---
## Sampling clock generator

<left>
[picture:1132:a_anit_alias:Anti-aliasing filter, A/D converter and clock generator]
</left>
<right>
* The A/D converter needs a clock for sampling
* The clock determines the moments at which the individual samples are taken
* Its frequency determines the sampling rate
* The clock rate can be fixed or controllable
</right>

<note>
The sampling clock generator dictates when the A/D converter takes each new sample.

Its frequency therefore directly determines the sampling rate. The clock rate can be fixed or can be controlled, for example, by a microcontroller.
</note>

---

[question:AF620]

---

## Back to the analogue signal

* The D/A converter produces analogue voltage values again from digital samples
* The values are output at fixed intervals of time
* At first, the output does not give an ideally smooth waveform
* Sharp transitions contain high-frequency components

<note>
On the output side, the reverse process takes place.

The D/A converter outputs the individual digital values as analogue voltage values. Because the output is discrete-time, the waveform is at first not ideally smooth.

Sharp edges and transitions in particular contain additional high-frequency signal components.
</note>

--- style="font-size: smaller;"

## Reconstruction filter

<left>
[picture:300:a_adc_4bit:Signal before the reconstruction filter]
</left>
<right>
[picture:299:a_adc_12bit:Signal after the reconstruction filter]
</right>

* The reconstruction filter is located *after* the D/A converter
* It passes the wanted frequency range
* Unwanted higher-frequency signal components are suppressed
* Low-pass or band-pass filters can be used

<fragment>
The result is again an analogue output signal that is as clean as possible.
</fragment>

<note>
The reconstruction filter removes unwanted higher-frequency signal components at the output of the D/A converter.

On the left, a signal before filtering is shown. The clearly visible edges contain high-frequency components.

After filtering, the waveform is smoother and comes closer to the wanted analogue signal.

Depending on the application, a low-pass or band-pass filter, for example, can be used for this.
</note>

---

[question:AF624]

---

[question:AF625]