## Converters

* Signals on one frequency band are converted to another frequency band
* E.g. a $\qty{2}{\meter}$ signal on receive is transmitted as a $\qty{70}{\centi\meter}$ signal
* The signal is converted in one direction only
* Basically a simple mixer

---
[question:EF504]

<note>
* TCXO and PLL come later
* But the mixing can be calculated
</note>

---
[question:EF505]
---
## Transverters

* In a transverter, the conversion works in both directions
* Here too, the conversion is done by mixing

---
[question:EF501]
---
[question:EF502]
---
[question:EF503]
<note>
* Solution on the next slide
</note>
---
### Solution

The frequency of the generator is multiplied by 3: $\qty{38.666}{\mega\hertz} \cdot 3 = \qty{116}{\mega\hertz}$

<left>
*TX path*
* The $\qtyrange{28}{30}{\mega\hertz}$ from the TRX are mixed with $\qty{116}{\mega\hertz}$
* The signal can be $\qtyrange{86}{88}{\mega\hertz}$ or $\qtyrange{144}{146}{\mega\hertz}$
</left>
<right>
[picture:843:e_transverter_tx:Transverter in the TX path]
</right>

---

<left>
*RX path*
* The antenna signal is mixed with $\qty{116}{\mega\hertz}$ and $\qtyrange{28}{30}{\mega\hertz}$ comes out
* So the antenna signal is at $\qtyrange{144}{146}{\mega\hertz}$, among other possibilities
* $\rightarrow$ Only the answer with $\qty{2}{\meter}$ and the transverter is correct
</left>
<right>
[picture:842:e_transverter_rx:Transverter in the RX path]
</right>

---
## Frequency stability

* Converters and transverters should be built with frequency-stable oscillators
* If the frequency is off, the output frequency is off too

---
<left>
* Diagram from the previous question
* $\qty{10}{\mega\hertz}$ becomes $\qty{2.256}{\giga\hertz}$, i.e. multiplication by $\num{225.6}$
* Because of an error, the oscillator produces $\qty{10.01}{\mega\hertz}$ instead of $\qty{10}{\mega\hertz}$
* $\qty{10.01}{\mega\hertz} \cdot 225.6 = \qty{2.258256}{\giga\hertz}$
* Mixer: $\qty{144}{\mega\hertz} + \qty{2.258256}{\giga\hertz} = \qty{2.402256}{\giga\hertz} \rightarrow \qty{2.256}{\mega\hertz}$ off
</left>
<right>
[picture:651:e_konverter_13cm:Converter for the $\qty{13}{\centi\meter}$ band]
</right>