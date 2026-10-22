* *Integrated circuit (IC)*
* Complex circuit on a semiconductor substrate
* Makes it easier to build electronic circuits

---
[question:AC601]
---
## Monolithic microwave integrated circuit (MMIC)

* Wideband amplifier with few components
* Typically $\qty{50}{\ohm}$ input and output impedance
* Combines active and passive components

---
[question:AC602]
---
[question:AC603]
---
[question:AC604]
---
### MMIC external circuitry

<left>
[picture:773:a_mmic:MMIC circuit]
</left>
<right>
* The operating point is set by $R_{\textrm{BIAS}}$
* Capacitors block DC voltage
* Terminals 2 and 4 are at chassis potential with respect to $U_{\textrm{CC}}$
* Terminal 1 is open
* $U_{\textrm{CC}}$ is dropped across $R_{\textrm{BIAS}}$ and the MMIC
</right>
<note>
</note>

---
[question:AF425]
---
#### Solution
* given: $U_{\textrm{D}} = \qty{4}{\volt}$
* given: $U_{\textrm{CC}} = \qty{13.5}{\volt}$
* given: $I_{\textrm{D}} = \qty{10}{\milli\ampere}$
* required: $R_{\textrm{BIAS}}$

<fragment>
$R_{\textrm{BIAS}} = \frac{U_{\textrm{CC}} - U_{\textrm{D}}}{I_{\textrm{D}}} = \frac{\qty{13.5}{\volt} - \qty{4}{\volt}}{\qty{10}{\milli\ampere}} = \qty{950}{\ohm}$
</fragment>

---
[question:AF426]
---
#### Solution
* given: $U_{\textrm{D}} = \qty{4}{\volt}$
* given: $U_{\textrm{CC}} = \qty{13.8}{\volt}$
* given: $I_{\textrm{D}} = \qty{15}{\milli\ampere}$
* required: $R_{\textrm{BIAS}}$

<fragment>
$R_{\textrm{BIAS}} = \frac{U_{\textrm{CC}} - U_{\textrm{D}}}{I_{\textrm{D}}} = \frac{\qty{13.8}{\volt} - \qty{4}{\volt}}{\qty{15}{\milli\ampere}} = \qty{653.3}{\ohm} \rightarrow \qty{680}{\ohm}$
</fragment>

---
[question:AF427]
---
#### Solution
* given: $U = \qty{9}{\volt}$
* given: $R_{\textrm{BIAS}} = \qty{470}{\ohm}$
* given: $U_{\textrm{D}} = \qty{4}{\volt}$
* required: $P$
* Approach: the current through $R_{\textrm{BIAS}}$ is the same everywhere, because there is no other ohmic load in the circuit

<fragment>
$I_{\textrm{D}} = \frac{U_{\textrm{BIAS}}}{R_{\textrm{BIAS}}} = \frac{U-U_{\textrm{D}}}{R_{\textrm{BIAS}}} = \frac{\qty{9}{\volt}-\qty{4}{\volt}}{\qty{470}{\ohm}} = \qty{10.64}{\milli\ampere}$
</fragment>
<fragment>
$P = U_{\textrm{D}} \cdot I_{\textrm{D}} = \qty{4}{\volt} \cdot \qty{10.64}{\milli\ampere} \approx \qty{43}{\milli\watt}$
</fragment>
