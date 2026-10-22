* One of the most important circuits in amateur radio
* Generation of RF oscillations in transmitters and receivers
* The heart of every radio

---
### Loop gain

* Amplifying element whose output signal is fed back to the input
* In phase
* Amplitude at least as large $\rightarrow$ *loop gain greater than $1$*
* Necessary for self-excitation, and keeps the oscillation going

---
[question:AD613]
---
<left>
[picture:760:a_oszillator_schaltungen_oszillator:Circuit of a capacitive-feedback three-point oscillator]
</left>
<right>
* The output signal is fed back from the emitter to the base through a capacitive potential divider
* The frequency is determined by the tuned circuit at the base and the capacitive potential divider connected in parallel with it
* Common-collector oscillator
</right>
<note>
Transistor circuits come a little later in the chapter
</note>

---
[question:AD614]
---
[question:AD616]
---
<left>
[picture:497:a_oszillator_schaltungen_quarzoszillator:Circuit of a crystal oscillator in common-collector configuration with the crystal operated at its fundamental frequency]  
</left>
<right>
* Tuned circuit replaced by a crystal
* The crystal can oscillate at its fundamental frequency or on harmonics $\rightarrow$ for this, the amplifier must be designed to be frequency-selective, e.g. with a tuned circuit
</right>
<note>
There is no other tuned circuit here, so the crystal is operated at its fundamental frequency
</note>

---
[question:AD617]
---
### Coupling out the signal

* Always at the lowest-impedance point of an oscillator
* This loads the oscillator only lightly
* In a common-collector circuit, at the emitter of the transistor

---
### Buffer stage

* Follow the oscillator with a buffer stage
* Decouples the oscillator from further parts of the circuit
* The frequency is not affected by loading of the output
* The buffer stage is often a common-collector circuit (an emitter follower) and has a high input impedance

---
[question:AD610]
---
[question:AD615]
---
### Measurement

* Measurements should be made after the buffer stage
* Otherwise the oscillator is loaded by the parasitic capacitances
* This affects the frequency

---
[question:AD619]
---
[question:AD618]
