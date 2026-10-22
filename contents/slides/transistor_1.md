--- data-transition="none"
## From diode to transistor
<left>
You can picture how it works like this:
* A control channel regulates the flow through a weir
* If no water flows in the control channel, the weir is closed
</left>
<right>
[picture:835:e_transistor_wehr_geschlossen:Control channel closes the weir completely]
</right>

--- data-transition="none"

## From diode to transistor
<left>
You can picture how it works like this:
* If some water flows in the control channel, the weir opens halfway
</left>
<right>
[picture:837:e_transistor_wehr_halb_offen:Control channel opens the weir halfway]
</right>

--- data-transition="none"

## From diode to transistor
<left>
You can picture how it works like this:
* If more water flows in the control channel, the weir is fully open
</left>
<right>
[picture:836:e_transistor_wehr_geoeffnet:Control channel opens the weir completely]
</right>

---

[question:EC602]

---

[question:EC608]

---

### Bipolar transistor and circuit diagram

<left>
Mnemonic for PNP $\rightarrow$ Pfeil Nach Platte (arrow towards the plate)
</left>
<right>
[picture:374:e_schaltbild_npn_transistor:Circuit diagram of an NPN transistor]
[picture:375:e_schaltbild_pnp_transistor:Circuit diagram of a PNP transistor]
</right>

---

[question:EC607]

---

[question:EC606]

---

[question:EC605]

---

[question:EC609]

---

### Switch or amplifier?
* The drive can be set so that the transistor is either off or fully on; it is then called a switching transistor.
* The drive can be set so that the transistor is controlled continuously; it is then called an amplifier.

---

[question:EC601]

---
[question:EC603]

---

## Drive voltage and its polarity
Each type of bipolar transistor needs a different polarity.

* An NPN transistor needs a positive control voltage to switch on.
* A PNP transistor needs a negative control voltage to switch on.

As with a silicon diode, the control voltage is about $\qty{0.6}{\volt}$.

---

[question:EC610]

---

Since the base current flows through the transistor as well as the collector current, the largest current flows through the emitter terminal.

---

[question:EC611]

--- style="font-size: smaller;"

###  When does the NPN transistor switch on?
Is the base-emitter voltage high enough, and is it positive?
Watch the signs here, and think again when they are negative. Examples:

* Base $\qty{+2}{\volt}$ and emitter $\qty{+1.4}{\volt} \rightarrow$ the base-emitter voltage is positive and is $\qty{+0.6}{\volt}$
* Base $\qty{-5.6}{\volt}$ and emitter $\qty{-6.2}{\volt} \rightarrow$ the base-emitter voltage is positive and is $\qty{+0.6}{\volt}$

---

Either you see it intuitively or you work it out (paying attention to the signs).

$U_{ BE } = U_{ B } - U_{ E }$

---

[question:EC612]

---

[question:EC613]

--- style="font-size: smaller;"

### When does the PNP transistor switch on?
Is the base-emitter voltage high enough, and is it negative?
Watch the signs here, and think again when they are negative. Examples:

* Base $\qty{+5.6}{\volt}$ and emitter $\qty{+6.2}{\volt} \rightarrow$ the base-emitter voltage is negative and is $\qty{-0.6}{\volt}$
* Base $\qty{-2}{\volt}$ and emitter $\qty{-1.4}{\volt} \rightarrow$ the base-emitter voltage is negative and is $\qty{-0.6}{\volt}$

---

Either you see it intuitively or you work it out (paying attention to the signs).

$U_{ BE } = U_{ B } - U_{ E }$

---

[question:EC614]

---

[question:EC615]

---

## Types of transistor
The transistors covered so far are called *bipolar transistors*. They are the type of transistor that heralded a technical revolution in the '50s and replaced the thermionic valve. Unlike current-controlled bipolar transistors, *field-effect transistors (FETs)* are voltage-controlled, so no control current flows into them. We will look at them in more depth in the Class A course.

---

[question:EC604]