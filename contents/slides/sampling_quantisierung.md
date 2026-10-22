## Sampling and quantisation

When an analogue signal is digitised, two properties have to be considered:

* **When** is the signal measured?
  * Sampling
  * continuous-time → discrete-time
* **How precisely** is the measured value represented?
  * Quantisation
  * continuous-value → discrete-value

<note>
Sampling and quantisation are two different steps.

In sampling, the time axis is made discrete: we look at the signal only at particular sampling instants.

In quantisation, by contrast, the value axis is made discrete: a measured value is assigned to one of a finite number of possible levels.
</note>

---

## Analogue signal

[picture:408:a_wertkont_zeitkont:Continuous-value and continuous-time signal]

* A signal value exists at every moment in time
* The signal value can take any intermediate value
* An ideal analogue signal is therefore *continuous-time* and *continuous-value*

--- style="font-size: smaller;"

## Sampling

<left>
[picture:408:a_wertkont_zeitkont:Continuous-value and continuous-time signal]
</left>
<right>
[picture:409:a_wertkont_zeitdisk:Continuous-value and discrete-time signal]
</right>

<fragment>
* The signal is sampled only at particular moments
* The individual sampled values are called *samples*
* A continuous-time signal becomes a *discrete-time* signal
* At first, the values themselves can still take any value
</fragment>

<note>
In idealised sampling, at first only the time axis changes.

Before sampling, the signal is defined at every moment. Afterwards, values exist only at particular sampling instants.

At this point the individual sample values do not yet have to be quantised. That is why the signal on the right is discrete-time but still continuous-value.
</note>

---

[question:AF601]

---

[question:AF603]

---

## Sampling

* The process of taking values at particular moments in time is called *sampling*
* The individual sampled values are called *samples*
* Between two samples the analogue signal can go on changing

<fragment>
Sampling therefore means:

**continuous-time → discrete-time**
</fragment>

---

[question:AF606]

---

## Sampling rate

* The *sampling rate* or *sample rate* states how many samples are taken per unit of time
* Unit: samples per second

<fragment>
Example, audio CD:

$\num{44100}$ samples per second

correspond to

$\qty{44.1}{\kilo\sps}$
</fragment>

<note>
The higher the sampling rate, the shorter the time between two successive samples.

What sampling rate is needed as a minimum is dealt with next, under the sampling theorem.
</note>

---

[question:AF615]

---

## Quantisation

* Analogue signal values can take any intermediate value: *continuous-value*
* Digitally, only a finite number of possible values is available: *discrete-value*
* A measured value has to be assigned to one of the available levels

<fragment>
This process is called *quantisation*.
</fragment>

<note>
After sampling, we know at which moments we look at the signal.

Now we still have to decide which digital numerical value is to represent each measured analogue value.

If the actual value lies between two possible levels, it is assigned to a suitable level.
</note>

--- style="font-size: smaller;"

## Continuous-value and discrete-value

<left>
[picture:410:a_wertdisk_zeitkont:Discrete-value and continuous-time signal]
</left>
<right>
[picture:411:a_wertdisk_zeitdisk:Discrete-value and discrete-time signal]
</right>

* Left: the values are already discrete, time is still continuous
* Right: values and time are discrete

<fragment>
Combining **sampling and quantisation** gives the digital representation of an analogue signal.
</fragment>

<note>
The left-hand diagram serves mainly to show that discrete time and discrete values are two independent properties.

The right-hand diagram is the one that matters most for digitisation: after sampling and quantisation there are only individual samples, which in addition can take only a finite number of possible values.
</note>

---

[question:AF602]

---

[question:AF604]

---

[question:AF605]

---

## Practical example: dimmer vs. step switch

* An analogue dimmer allows fine, continuous brightness settings  
* A step switch (e.g. $\num{5}$ steps) allows only fixed brightness values – intermediate steps are not possible
* Quantisation: choosing the step that fits best to represent the analogue value

---
## Summary

<left>
[include:quantisierung_und_sampling]
</left>
<right>
* Sampling determines **when** a value is looked at
* Quantisation determines **which digital value** it becomes
* Only both steps together give a discrete-time and discrete-value signal
</right>

<note>
With the applet, sampling and quantisation can be looked at together.

The sampling rate affects the time between the samples. Quantisation, on the other hand, determines which possible values the samples can take.

This lets you follow the two steps, which are independent at first, together once more.
</note>