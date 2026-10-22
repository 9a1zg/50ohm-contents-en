<left>
[picture:35:e_schaltnetzteil:Basic circuit diagram of a switch-mode power supply]
</left>
<right>
* Electronic switch E regulates to a constant output voltage
* Switching time is varied
* Switch stays closed for longer $\rightarrow$ more energy to the load side $\rightarrow$ output voltage rises
* This is the *pulse-width modulator*
</right>
<note>
The simplified diagram lacks the feedback of the output voltage to control block E that completes the control loop.
</note>
---
[question:AD311]
---
### Galvanic isolation

<left>
* Isolation of the input side from the output side
* Keeps the circuit's interference signals away from the mains side
* Otherwise the mains acts like an antenna
</left>
<right>
<fragment>
[photo:277:a_störspektrum:Interference spectrum of a switch-mode power supply]
</fragment>
</right>

---
[question:AD312]
---
[question:AD313]
---
<left>
[picture:367:a-schaltnetzteilfilter:Filter at the 230 V input of a switch-mode power supply]
Low-pass filter on the input side
</left>
<right>
[photo:243:a_EMV Filter2: Filter directly at the 230 V AC voltage input]
</right>
<note>
- PE must not be connected to L1 or N.
- Choke T must not act as a transformer.
</note>
---
[question:AD314]
