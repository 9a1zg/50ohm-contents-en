## Bipolar transistor


[picture:864:a_bauelemente_bipolartransistor:Circuit diagram of an npn and a pnp bipolar transistor with collector (C), base (B) and emitter (E)]

* Three semiconductor zones
* Alternately n- and p-doped
* npn transistor and pnp transistor

---
[question:AC503]
---
[question:AC504]
---
### Current control and factor

* Base-emitter voltage $U_{\textrm{BE}}$ controls collector current $I_{\textrm{C}}$ exponentially
* In the bipolar transistor a base current $I_{\textrm{B}}$ always flows, depending exponentially on $U_{\textrm{BE}}$
* Factor $B$ is the *current gain factor* of the transistor
* Approx. 20 to 500

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}}$
</fragment>

<note>
A higher factor needs a smaller base current to control a larger collector current
</note>
---
[question:AC501]
---
### Conducting bipolar transistor

* A significant collector current flows
* Base-emitter diode forward-biased
* Collector-base diode blocks, so that no charge carriers get from the collector into the base

---
[question:AC505]
---
[question:AC515]
---
#### Solution
* The value of $R_1$ sets the base current $I_B$
* $I_B$ is smaller than $I_C$ by a factor of 298
* For the voltage across $R_1$, the voltage lost in the transistor must be subtracted

---
* given: $U = \qty{12}{\volt}$
* given: $I_{\textrm{C}} = \qty{5}{\milli\ampere}$
* given: $B = 298$
* given: $U_{\textrm{BE}} = \qty{0.6}{\volt}$
* required: $R_1$

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}} \Rightarrow I_{\textrm{B}} = \frac{I_{\textrm{C}}}{B} = \frac{\qty{5}{\milli\ampere}}{298} = \qty{16.779}{\micro\ampere}$
</fragment>
<fragment>
$R_1 = \frac{U-U_{\textrm{BE}}}{I_{\textrm{B}}} = \frac{\qty{12}{\volt} - \qty{0.6}{\volt}}{\qty{16.779}{\micro\ampere}} \approx \qty{680}{\kilo\ohm}$
</fragment>

<note>
The disadvantage of the circuit is its poorly controlled current gain
</note>
---
[question:AC518]
---
### Stabilising the operating point

<left>
[picture:361:a_bauteile_arbeitspunkteinstellung:Transistor circuit with base potential divider]
</left>
<right>
* The operating point is set by the potential divider
* The divider current through $R_2$ should be high enough that the base current has little influence on the operating point
</right>
<note>
The collector current depends exponentially on the base-emitter voltage; the tolerance of the resistors can have a large effect on the collector current. The strong temperature dependence in the transistor can affect the collector current.
</note>

---
[question:AC516]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $U = \qty{10}{\volt}$
* given: $I_{\textrm{C}} = \qty{2}{\milli\ampere}$
* given: $B = 200$
</left>
<right>
* given: $U_{\textrm{R2}} = \qty{0.6}{\volt}$
* given: $I_{\textrm{R2}} = 10 \cdot I_{\textrm{B}}$
* required: $R_1$
</right>

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}} \Rightarrow I_{\textrm{B}} = \frac{I_{\textrm{C}}}{B} = \frac{\qty{2}{\milli\ampere}}{200} = \qty{10}{\micro\ampere}$
</fragment>
<fragment>
$U_{\textrm{R1}} = U - U_{\textrm{R2}} = \qty{10}{\volt} - \qty{0.6}{\volt} = \qty{9.4}{\volt}$
</fragment>
<fragment>
$I_{\textrm{R1}} = I_{\textrm{B}} + I_{\textrm{R2}} = I_{\textrm{B}} + 10 \cdot I_{\textrm{B}} = \qty{110}{\micro\ampere}$
</fragment>
<fragment>
$R_1 = \frac{U_{\textrm{R1}}}{I_{\textrm{R1}}} = \frac{\qty{9.4}{\volt}}{\qty{110}{\micro\ampere}} \approx \qty{85.5}{\kilo\ohm}$
</fragment>

---
[question:AC517]
---
#### Solution

* $U_{\textrm{R2}}$ is equal to $U_{\textrm{BE}} + U_{\textrm{RE}}$
* The collector current is determined mainly by $R_{\textrm{E}}$
* Very stable circuit

--- style="font-size: smaller;"
<left>
* given: $U = \qty{10}{\volt}$
* given: $I_{\textrm{C}} = \qty{2}{\milli\ampere}$
* given: $B = 200$
</left>
<right>
* given: $U_{\textrm{BE}} = \qty{0.6}{\volt}$
* given: $U_{\textrm{RE}} = \qty{1}{\volt}$
* given: $I_{\textrm{R2}} = 10 \cdot I_{\textrm{B}}$
</right>
* required: $R_1$

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}} \Rightarrow I_{\textrm{B}} = \frac{I_{\textrm{C}}}{B} = \frac{\qty{2}{\milli\ampere}}{200} = \qty{10}{\micro\ampere}$
</fragment>
<fragment>
$U_{\textrm{R2}} = U_{\textrm{BE}} + U_{R_{\textrm{E}}} = \qty{0.6}{\volt} + \qty{1}{\volt} = \qty{1.6}{\volt}$
</fragment>
<fragment>
$U_{\textrm{R1}} = U - U_{\textrm{R2}} = \qty{10}{\volt} - \qty{1.6}{\volt} = \qty{8.4}{\volt}$
</fragment>
<fragment>
$I_{\textrm{R1}} = I_{\textrm{B}} + I_{\textrm{R2}} = I_{\textrm{B}} + 10 \cdot I_{\textrm{B}} = \qty{110}{\micro\ampere}$
</fragment>
<fragment>
$R_1 = \frac{U_{\textrm{R1}}}{I_{\textrm{R1}}} = \frac{\qty{8.4}{\volt}}{\qty{110}{\micro\ampere}} \approx \qty{76.4}{\kilo\ohm}$
</fragment>

---
[question:AC519]
---
#### Solution

* No current through $R_1 \rightarrow$ no voltage across $R_2$
* Base is at chassis potential $\rightarrow$ no current flows through the transistor
* No voltage drop across $R_{\textrm{C}} \rightarrow$ collector potential rises to the operating voltage

---
[question:AC520]
---
#### Solution

* $R_2$ carries no current $\rightarrow$ the base is connected to the operating voltage through $R_1$
* Because of the way the divider is designed, the base current is now 11 times higher than intended
* The collector current will rise sharply $\rightarrow$ the voltage drop across $R_{\textrm{C}}$ rises sharply
* $U_{\textrm{CE}}$ falls to the saturation value of approx. $\qty{0.1}{\volt}$

---
## Field-effect transistor (FET)

[picture:271:a_bauelemente_fet:Circuit diagrams of field-effect transistors]

* Different construction
* There is a semiconductor channel
* The current flow is controlled by an electric field
* Hence voltage-controlled

<note>
The vertical line represents the channel, contacted by the drain (top) and the source (bottom); the gate is on the left, and the arrow is reminiscent of a diode
</note>
---
[question:AC502]
---
[question:AC506]
---
### Terminals of the FET

* *Source*: source of the charge carriers in the channel
* *Drain*: outflow of the charge carriers in the channel
* *Gate*: controls the flow of charge carriers in the channel

---
[question:AC513]
---
[question:AC512]
---
[question:AC514]

<note>
Better: controls the channel current rather than the resistance, as this resistive behaviour only occurs at small drain-source voltages
</note>
---
### Types of FET

* *depletion-mode*: with no gate-source voltage the FET conducts
* *enhancement-mode*: with no gate-source voltage the FET is off
* *n-channel FET*: the current in the channel is carried by electrons
* *p-channel FET*: the current in the channel is carried by holes
* *junction FET*: the gate is a diode
* *insulated-gate FET*: the gate is a capacitor structure (e.g. MOSFET)

<note>
MOSFET: metal-oxide-semiconductor FET
</note>
---
### FET circuit symbols

<left>
[picture:273:a_bauelemente_selbstleitender_p_kanal_mosfet:Depletion-mode p-channel MOSFET]
[picture:276:a_bauelemente_selbstsperrender_n_kanal_mosfet:Enhancement-mode n-channel MOSFET]
</left>
<right>
* *depletion-mode*/*enhancement-mode*: gate continuous/dashed
* *p-*/*n-channel*: arrow points away from/towards the channel
* *insulated gate* (MOSFET): gate and channel as a capacitor
</right>

---
[question:AC507]
---
[question:AC508]
---
[question:AC509]
---
[question:AC510]
---
[question:AC511]
---
[question:AC521]
---
#### Solution

<left>
* given: $U_{\textrm{B}} = \qty{44}{\volt}$
* given: $R_1 = \qty{10}{\kilo\ohm}$
* given: $R_2 = \qty{1}{\kilo\ohm}$
* given: $R_3 = \qty{2.2}{\kilo\ohm}$
* required: $U_{\textrm{GS}}$
* Approach: unloaded potential divider across $R_1$ and $R_2$, with $U_{\textrm{GS}} = U_{\textrm{R2}}$
</left>
<right>
<fragment>
$\begin{split} \frac{U_{\textrm{R2}}}{U_{\textrm{B}}} &= \frac{R_2}{R_1+R_2}\\ \Rightarrow U_{\textrm{R2}} &= \frac{R_2}{R_1+R_2} \cdot U_{\textrm{B}}\\ &= \frac{\qty{1}{\kilo\ohm}}{\qty{10}{\kilo\ohm}+\qty{1}{\kilo\ohm}} \cdot \qty{44}{\volt}\\ &= \frac{1}{11} \cdot \qty{44}{\volt} = \qty{4}{\volt} \end{split}$
</fragment>
</right>

---
[question:AC522]
---
#### Solution

<left>
* given: $U_{\textrm{B}} = \qty{44}{\volt}$
* given: $R_1 = \qty{10}{\kilo\ohm}$
* given: $R_3 = \qty{2.2}{\kilo\ohm}$
* given: $U_{\textrm{GS}} = U_{\textrm{R2}} = \qty{2.8}{\volt}$
* given: $U_{\textrm{B}} = U_{\textrm{R1}} + U_{\textrm{R2}}$
* required: $R_2$
</left>
<right>
<fragment>
$\begin{split} \frac{U_{\textrm{R1}}}{U_{\textrm{R2}}} &= \frac{R_1}{R_2}\\ \Rightarrow R_2 &= R_1 \cdot \frac{U_{\textrm{R2}}}{U_{\textrm{R1}}}\\ &= R_1 \cdot \frac{U_{\textrm{R2}}}{U_{\textrm{B}}-U_{\textrm{GS}}}\\ &= \qty{10}{\kilo\ohm} \cdot \frac{\qty{2.8}{\volt}}{\qty{44}{\volt}-\qty{2.8}{\volt}}\\ &\approx \qty{680}{\ohm} \end{split}$
</fragment>
</right>
---
[question:AC523]
---
#### Solution

* given: $R_{\textrm{DSon}} = \qty{4}{\milli\ohm}$
* given: $I = \qty{25}{\ampere}$
* required: $P$

<fragment>
$P = I^2 \cdot R = (\qty{25}{\ampere})^2 \cdot \qty{4}{\milli\ohm} = \qty{2.5}{\watt}$
</fragment>

<note>
The MOSFET behaves like an ohmic resistance
</note>

---
### Freewheeling diode

* The relay is driven through a bipolar transistor connected in series
* Transistor switches on $\rightarrow$ current flows through the relay coil
* Transistor switches off $\rightarrow$ the current in the coil induces a negative voltage at the transistor
* This can destroy the transistor
* Prevention: fit a *freewheeling diode* in parallel with the relay, in the reverse direction
* The induced voltage is limited to the diode voltage

---
[question:AC524]