<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* Bipolar transistor amplifier circuits are named after the terminal through which both the input and the output signal flow
* Or the other way round: the terminal to which neither the input nor the output is directly connected
</right>
---
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* Input signal: source $\rightarrow$ base $\rightarrow$ collector $\rightarrow$ supply voltage $\rightarrow$ source
* Output signal: collector $\rightarrow$ load $\rightarrow$ supply voltage $\rightarrow$ collector
</right>
---
[question:AD401]
---
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* The transistor needs a defined operating point (bias)
* This is set by the potential divider at the base
</right>
--- 
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* The emitter resistor produces a voltage when current flows through the transistor.
* The current flows from the emitter through the resistor to chassis.
* The more current flows, the higher the voltage at the emitter becomes.
</right>
---
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* The emitter voltage holds back the current and prevents large fluctuations.
* Changes in temperature affect the transistor less.
* $\rightarrow$ The transistor remains reliable and works steadily.
</right>
---
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* Signals are coupled in and out at the base and emitter through *coupling capacitors*
* They keep DC components away from the amplifier stage
* The operating point is stabilised
</right>
---
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* The decoupling capacitor on the supply voltage takes unwanted RF and AF signals to chassis
* Feedback effects within the stage and on the supply voltage are avoided
* The collector is connected to chassis $\rightarrow$ the output is at the same potential as the input
</right>
---
<left>
[picture:140:a_kollektorschaltung_schaltbild:Bipolar transistor amplifier in common-collector configuration]
</left>
<right>
* The phase shift is $\qty{0}{\degree}$
* Input impedance relatively high
* $\rightarrow$ Voltage gain approx. $\num{0.9}$ to $\num{0.98}$ (always slightly less than $1$)
* Output impedance very low compared with the input impedance
</right>

---
[question:AD405]
---
[question:AD402]
---
[question:AD403]
---
### Buffer stage

* Often used as a buffer stage between an oscillator and further parts of the circuit
* Presents a high-impedance load to the oscillator
* $\rightarrow$ Less current drawn from the oscillator
* $\rightarrow$ Decoupling
* $\rightarrow$ Better frequency stability of the oscillator

---
[question:AD404]