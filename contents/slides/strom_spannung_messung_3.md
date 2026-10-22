## Current and voltage measurement

<left>
* Voltage is measured in parallel with the component
* Current is measured in series with the component
</left>
<right>
[picture:1003:a_strom_spannung_messung:Measuring the power of an amplifier (PA)]
</right>

---
[question:AI101]
---
[question:AI102]
---
## Accuracy

The displayed value usually differs from the true value
* Internal resistance of the meter
* Resolving power $\rightarrow$ *finest resolution*
* The reading only changes when the value changes by the finest resolution
* The manufacturer determines the deviation
* The deviation is stated in the data sheet

---

<left>
[picture:1004:a_reale_spannungsmessung:Equivalent circuit of a real voltmeter]
</left>

<right>
[picture:1007:a_reale_strommessung:Equivalent circuit of a real ammeter]
</right>

---
[question:AI103]
--- style="font-size: smaller;"
### Solution

* Percentage calculation – the absolute values are not relevant
* given: $U_{\mathrm{Abw}}$ at $\qty{95}{\percent}$ of the true value
* given: $I_{\mathrm{Abw}}$ at $\qty{95}{\percent}$ of the true value
* required: deviation of the power $P = U \cdot I$

<fragment>
$\begin{split} P_{\textrm{Abw}} &= 100\% - (U_{\mathrm{Abw}} \cdot I_{\mathrm{Abw}})\\ &= 100\% - (95\% \cdot 95\%)\\ &= 100\% - 90.25\%\\ &= 9.75\% \end{split}$
</fragment>

---
## Current through the multimeter

* A current flows through a meter even when it measures voltage
* The current divides
* Because of the high internal resistance, the current drawn off is relatively small

---
[question:AI104]
---
### Solution
* given: $U = \qty{0.5}{\volt}$
* given: $R = \qty{10}{\mega\ohm}$
* required: $I$

<fragment>
$$I = \frac{U}{R} = \frac{\qty{0.5}{\volt}}{\qty{10}{\mega\ohm}} = \qty{50}{\nano\ampere}$$
</fragment>

