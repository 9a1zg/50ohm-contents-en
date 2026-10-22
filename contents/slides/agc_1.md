* Automatic gain control (*AGC*) readjusts the AF output signal when the RF input signal fluctuates
* Used e.g. with fading
* Volume fluctuations are reduced

---
## How it works

* Measurement of the received level at the output of the receive path
* This is used to control the RF gain
* Influences the received volume after demodulation
* Response (attack time, decay time) can be adjusted
<note>
* Do not confuse with automatic level control (ALC) in the transmitter
</note>

---
## AGC modes

<left>
* AGC Slow
* AGC Normal
* AGC Fast
* AGC Off
</left>
<right>
* SSB: AGC Slow or Normal
* Morse: AGC Normal or Fast
* Data modes: AGC Fast or Off
</right>
<note>
* The faster response is there so that strong signals cannot mask weak signals and the control follows quickly
</note>

---
[question:EF211]
---
[question:EF212]