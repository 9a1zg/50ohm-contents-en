* Stabilising a variable, potentially unstable oscillator (e.g. a VCO) by means of a stable reference oscillator
* Phase comparison between the two signals
* The output frequency corresponds to the reference frequency or a multiple of it, and remains stable

--- style="font-size: smaller;"
[picture:45:a_oszillator_pll_pll:Diagram of a phase-locked loop (PLL)]

* *Phase detector* compares the phases of the VCO and the reference oscillator
* *Low-pass filter* converts the pulses from the phase detector into a DC voltage
* *VCO* generates the output frequency according to the DC voltage from the low-pass filter
* *Frequency divider* (optional) synchronises the VCO frequency to a multiple of the reference frequency

<note>
When there are phase errors, the phase detector outputs pulses, which the low-pass filter smooths into a DC voltage. The change in frequency at the VCO gradually reduces the phase difference.
</note>

---
[question:AD701]
---
[question:AD702]
---
### Accuracy and stability

* Depend on the quality of the reference oscillator
* Often a crystal oscillator

---
[question:AD705]
---
### Frequency division and tuning

* The frequency divider allows the PLL to be set to different frequencies
* The output frequency is an integer multiple of the reference frequency
* The smallest selectable frequency corresponds to the reference oscillator

---
[question:AD703]
---
[question:AD704]
--- style="font-size: 0.7em;"
#### Solution
* given: $f_\text{Osc} = \qty{12.5}{\kilo\hertz}$
* given: $f_\text{Out,low} = \qty{12.000}{\mega\hertz}$
* given: $f_\text{Out,high} = \qty{14.000}{\mega\hertz}$
* required: $n$

<fragment>
For $f_{Out,low} = \qty{12.000}{\mega\hertz}$:
$n = \frac{f_\text{Out,low}}{f_\text{Osc}} = \frac{\qty{12.000}{\mega\hertz}}{\qty{12.5}{\kilo\hertz}} = 960$
</fragment>
<fragment>
For $f_\text{Out,high} = \qty{14.000}{\mega\hertz}$:
$n = \frac{f_\text{Out,high}}{f_\text{Osc}} = \frac{\qty{14.000}{\mega\hertz}}{\qty{12.5}{\kilo\hertz}} = 1120$
</fragment>