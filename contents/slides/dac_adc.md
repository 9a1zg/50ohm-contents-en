## A/D and D/A conversion

* *A/D converters* convert analogue signals into digital values
* *D/A converters* convert digital values back into analogue signals
* Both have only a finite number of possible values
* An important property is therefore their *resolution*

<note>
A/D and D/A converters form the interface between the analogue and the digital world.

The A/D converter produces digital samples from an analogue input signal. The D/A converter carries out the reverse process and produces analogue voltage values again from digital values.
</note>

---
## Quantisation in the A/D converter

* The A/D converter can produce only a limited number of digital values
* Analogue input values are therefore assigned to fixed levels
* Intermediate values cannot be represented exactly
* This gives rise to a *quantisation error*

<note>
We have already met quantisation.

An analogue value actually measured often lies between two possible digital levels. The A/D converter has to assign it to one of these levels.

The resulting difference between the actual value and the value represented is called the quantisation error.
</note>

---

[question:AF607]

---
## Resolution of an A/D converter

* The resolution states the number of digital values that can be distinguished
* It is usually stated in *bits*
* $\qty{8}{\bit}$ → $\num{256}$ possible values
* $\qty{16}{\bit}$ → $\num{65536}$ possible values
* More bits allow a finer representation of the signal amplitude

---
## Effect of the resolution

<left>
[picture:300:a_adc_4bit:Sine-wave signal digitised by a 4-bit A/D converter, followed by D/A conversion]
</left>
<right>
[picture:299:a_adc_12bit:Sine-wave signal digitised by a 12-bit A/D converter, followed by D/A conversion]
</right>

* $\qty{4}{\bit}$ → $\num{16}$ possible values
* $\qty{12}{\bit}$ → $\num{4096}$ possible values
* Higher resolution → smaller quantisation steps

<note>
Here the effect of the resolution can be compared directly.

With 4 bits, only 16 possible values are available. The steps can be seen clearly in the reconstructed signal.

With 12 bits, 4096 possible values are already available. The reconstructed signal therefore comes much closer to the original sine-wave signal.

The additional 8 bits increase the number of possible levels by a factor of 256.
</note>

---

[question:AF608]

---
## Jitter

* The samples should be taken at exactly defined moments
* In practice, the actual sampling instants can fluctuate slightly
* These deviations in time are called *jitter*
* Jitter can cause additional noise in the digitised signal

<note>
Not only the accuracy of the measured amplitude is important, but also the accuracy of the sampling instant.

For this, the A/D converter needs a clock that is as stable as possible. Small fluctuations of this clock in time mean that the samples are not taken at exactly the intended moments.

These fluctuations are called jitter.
</note>

---

[question:AF621]

---
## D/A converter

* The D/A converter is the counterpart of the A/D converter
* It produces analogue voltage values from digital samples
* A D/A converter, too, has only a finite number of possible output values
* Its resolution is likewise stated in bits

<note>
In the D/A converter, the process runs in the opposite direction.

A digital numerical value is assigned to a particular analogue output value. Here, too, the resolution determines how many different values can be produced.
</note>

---

[question:AF609]

---
## Voltage range and resolution

* A D/A converter has a fixed voltage range
* Example: $\qty{0}{\volt}$ to $\qty{1}{\volt}$
* With $\qty{4}{\bit}$, $\num{2^4}=\num{16}$ possible levels are available
* In a linear D/A converter, these are spread evenly over the voltage range

---
## Step size

With $\num{16}$ levels there are $\num{15}$ intervals between the levels.

For a voltage range from $\qty{0}{\volt}$ to $\qty{1}{\volt}$ this gives:

$\frac{\qty{1}{\volt}}{16-1}\approx\qty{67}{\milli\volt}$

<fragment>
The step size is therefore about $\qty{67}{\milli\volt}$.
</fragment>

<note>
Note here that there are only 15 intervals between 16 possible voltage values.

This is the well-known fencepost problem: between 10 fence posts there are only 9 gaps.

That is why, in this example, the voltage range is divided by 15 and not by 16.
</note>

---

[question:AF611]

---

[question:AF610]

---
## A/D and D/A converters in an SDR

* A/D converters digitise analogue input signals
* The samples can then be processed digitally
* D/A converters produce analogue signals from them again where needed
* This principle is used in many places in SDR receivers and transceivers

<note>
An SDR is a typical example of A/D conversion, digital signal processing and D/A conversion working together.

The analogue signal is first digitised. After that, filtering, demodulation or modulation, for example, can be done digitally. If an analogue signal is then to be produced again, a D/A converter is used.
</note>

---
## Using the range of values

* A small input signal uses only some of the available levels
* An input signal that is too large exceeds the range of values that can be represented
* Values above the maximum can no longer be represented correctly
* At this point the signal is cut off

<fragment>
This effect is called *clipping*.
</fragment>

<note>
For the best possible digitisation, the available range of values should be used sensibly.

If the signal is very small, only a few of the available levels are used.

If, on the other hand, the signal is too large, the A/D converter reaches its maximum value that can be represented. Even larger input values can no longer be distinguished. The peaks of the signal therefore appear cut off.

A D/A converter, too, cannot produce an output voltage outside its intended range of values.
</note>

---
## Effect of the resolution

* High resolution → many possible amplitude values
* Low resolution → few possible amplitude values
* More levels allow more accurate digitisation and reconstruction
* The available range of values should be used as fully as possible

---

[question:AF613]

---

[question:AF612]

---

[question:AF614]