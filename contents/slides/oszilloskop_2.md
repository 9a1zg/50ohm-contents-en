<left>
[photo:212:a_oszilloskop:Digital oscilloscope]
</left>
<right>
* Displays how voltages vary over time
* Measures the waveform
</right>
---
[question:AI301]
---
[question:AI304]
---
### Pulse width

<left>
[picture:1005:a_impulsbreite:Determining the pulse width of a non-ideal square-wave signal]
</left>
<right>
Definition: the pulse width is taken at 50% of the peak value
</right>
---
[question:AI303]
---
### Trigger

<left>
[photo:219:a_oszilloskop_x-ablenkung:With no input voltage, only a dot moves from left to right across the screen of an analogue oscilloscope, here at a speed of one division per second.]
</left>
<right>
* The trigger evaluates the applied signal
* E.g. the voltage passing through 0 from negative to positive
* This allows a stationary picture of a wave to be shown
</right>
---
[question:AI302]
---
### Probes

<left>
[photo:223:a_oszilloskop_tastkoepfe:Probes with various probe tips. The crocodile clips were removed for this photograph.]
</left>
<right>
* For measuring the voltage
* Tip made as a hook or needle
* Earth reference usually via a separate crocodile clip
* 10:1 probes divide the voltage to one tenth
</right>
---
### Measuring with an oscilloscope

[photo:224:a_oszilloskop_messung:Measuring with a probe. The probe tip can be seen between diodes D1 and D2, and further to the left the crocodile clip for the earth connection.]
---
[question:AI305]
---
### Solution
* given: $R=50\Omega$
* given: (from the diagram) $\hat{U} = 100V$
* required: $P_{\textrm{PEP}}$

<fragment>
$\begin{split} P_{\textrm{PEP}} &= \frac{U_{\textrm{eff}}^2}{R} = \frac{\left(\frac{\qty{100}{\volt}}{\sqrt{2}}\right)^2}{\qty{50}{\ohm}}\\ &=\frac{\frac{(\qty{100}{\volt})^2}{2}}{\qty{50}{\ohm}} = \frac{\qty{5000}{\volt}^2}{\qty{50}{\ohm}} = \qty{100}{\watt} \end{split}$
</fragment>
---
[question:AI306]
---
### Solution
* given: $R=\qty{50}{\ohm}$
* given: (from the diagram, with a 10:1 probe) $\hat{U} = \qty{6}{\volt}\cdot 10$
* required: $P_{\textrm{PEP}}$

<fragment>
$\begin{split} P_{\textrm{PEP}} &= \frac{U_{\textrm{eff}}^2}{R} = \frac{\left(\frac{\qty{6}{\volt}\cdot 10}{\sqrt{2}}\right)^2}{\qty{50}{\ohm}}\\ &=\frac{\frac{(\qty{60}{\volt})^2}{2}}{\qty{50}{\ohm}} = \qty{36}{\watt} \end{split}$
</fragment>

---
## Pulse

<left>
* A signal jumps from one value to a higher one and, at a later time, back again
* The duration of the pulse is measured from the middle of the rising edge to the middle of the falling edge
</left>
<right>
[picture:57:e_impuls:Pulse on an oscilloscope] 
</right>
---
[question:EI303]