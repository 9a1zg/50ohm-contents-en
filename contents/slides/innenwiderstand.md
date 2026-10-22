<left>
[picture:1058:a_isource_schematic:Equivalent circuit of a current source, $R_i$ high]
</left>
<right>
* Delivers a constant current
* Regardless of the load connected
* Theory: infinitely large internal resistance
* Practice: very high internal resistance
</right>

---

### Uses of a current source

* Laboratory power supplies
* Charging rechargeable batteries

<note>
Laboratory power supplies are dealt with further in the next section
</note>

### Voltage source
<left>
[picture:1018:a_vsource_schematic:Equivalent circuit of a voltage source]
</left>
<right>
* Real voltage source loaded with $R_L$ $\rightarrow$ terminal voltage $U_k$ falls
* The reason is the internal resistance
* Without a load / at open circuit: $U_q = U_L$
</right>
<note>
</note>

---
### Internal resistance

<left>
* Cannot be measured with a multimeter
* Calculate it: <br/>$R_i = \frac{\Delta U}{\Delta I}$
</left>
<right>
* Open circuit: $I = \qty{0}{\ampere}$
* Loaded with $R_L$: <br/>$I_L = \frac{U_L}{R_L}$
</right>

---
### Internal resistance of a voltage source

$(\Delta U = \qty{0}{\volt})$;  $R_i = \frac{\Delta U}{\Delta I} = \frac{0}{x} = \qty{0}{\ohm}$

<fragment>
Ideal voltage sources should have a very low internal resistance $R_i \ll R_L$

Ideal case: $\qty{0}{\ohm}$; the output voltage then stays unchanged under load.
</fragment>

---

### Current limiting

* Built into laboratory power supplies
* Load current exceeds a maximum current
* $\rightarrow$ terminal voltage is lowered
* $\rightarrow$ load current stays constant
* Function of the constant-current source

---
### Internal resistance of a current source

$R_i = \frac{\Delta U}{\Delta I}$; $(\Delta I \to \qty{0}{\ampere})$;  $R_i = \frac{\Delta U}{\Delta I} \to \qty{\infty}{\ohm}$

<fragment>
Ideal current sources should have a very high internal resistance $R_i \gg R_L$.

Ideal case: $\qty{\infty}{\ohm}$; the load current then stays constant when the  load resistance changes, which is why this is also called current matching.
</fragment>

---
[question:AB201]
---
### Power matching

* Optimum power delivery from transmitter to antenna
* $R_i = R_L$

--- style="font-size: 0.7em;"

|c: Internal resistance: summary | c: Internal resistance |
| Voltage matching with a constant-voltage source| $R_i$ is very low; theoretically $\qty{0}{\ohm}$; $R_i \ll R_L$ is the same as $R_L \gg R_i$|
|Current matching with a constant-current source|$R_i$ is very high; $R_i \gg R_L$ is the same as $R_L \ll R_i$ |
| Power matching with amplifiers| $R_L = R_i$|
[table:a_Innenwiderstand Zusammenfassung:Summary of internal resistance]

---
[question:AG401]
---
[question:AB202]
---
[question:AB203]
---
[question:AB204]
---
[question:AB207]
---
#### Solution
* given: $U_0 = \qty{13.5}{\volt}$
* given: $U_{Kl} = \qty{13}{\volt}$
* given: $I = \qty{2}{\ampere}$
* required: $R_i$

<fragment>
$R_i = \frac{U_i}{I} = \frac{U_0-U_{Kl}}{I} = \frac{\qty{13.5}{\volt} - \qty{13}{\volt}}{\qty{2}{\ampere}} = \qty{0.25}{\ohm}$
</fragment>
---
[question:AB208]
---
#### Solution
* given: $U_0 = \qty{13.8}{\volt}$
* given: $U_{Kl} = \qty{13.6}{\volt}$
* given: $I = \qty{20}{\ampere}$
* required: $R_i$

<fragment>
$R_i = \frac{U_i}{I} = \frac{U_0-U_{Kl}}{I} = \frac{\qty{13.8}{\volt} - \qty{13.6}{\volt}}{\qty{20}{\ampere}} = \qty{10}{\milli\ohm}$
</fragment>
---
[question:AB206]
---
#### Solution
* given: $U_0 = \qty{13.5}{\volt}$
* given: $U_{Kl} = \qty{12.4}{\volt}$
* given: $I = \qty{0.9}{\ampere}$
* required: $R_i$

<fragment>
$R_i = \frac{U_i}{I} = \frac{U_0-U_{Kl}}{I} = \frac{\qty{13.5}{\volt} - \qty{12.4}{\volt}}{\qty{0.9}{\ampere}} = \qty{1.22}{\ohm}$
</fragment>
---
[question:AB205]
---
#### Solution
* given: $U_0 = \qty{5.0}{\volt}$
* given: $U_{Kl} = \qty{4.8}{\volt}$
* given: $R_L = \qty{1.2}{\ohm}$
* required: $R_i$

<fragment>
$I = \frac{U_{Kl}}{R_L} = \frac{\qty{4.8}{\volt}}{\qty{1.2}{\ohm}} = \qty{4}{\ampere}$
</fragment>
<fragment>
$R_i = \frac{U_i}{I} = \frac{U_0 - U_{Kl}}{I} = \frac{\qty{5.0}{\volt} - \qty{4.8}{\volt}}{\qty{4}{\ampere}} = \qty{0.05}{\ohm}$
</fragment>
