* Antennas have a feed-point impedance that depends on the exact arrangement of the antenna elements
* If it does not match the characteristic impedance of the feeder, *reflection* occurs
* Transmit power is reflected back to the radio $\rightarrow$ cannot be radiated by the antenna
* If the feed-point impedance of the antenna and the characteristic impedance of the feeder are the same, the antenna is *matched*

---

## Standing wave ratio (SWR)

* A measure of how good the antenna match is
* Put simply, states how much transmit power is reflected by the antenna
* Abbreviated to SWR
* Measured with an *SWR meter*

<note>
Exact calculation: $\text{SWR} = \frac {\sqrt{P_\text{V}}+\sqrt{P_\text{R}}} { \sqrt{P_\text{V}}-\sqrt{P_\text{R}}}$ with $P_\text{V}$ the forward and $P_\text{R}$ the reflected power -- not needed for the Class N examination
</note>

---

## SWR meter

Measures at the same time the transmit power going to the antenna and the reflected power coming back

<left>
[photo:144:swr_meter:A simple SWR meter for determining the standing wave ratio]
</left>
<right>
[photo:143:swr_meter_kreuzzeiger:SWR meter with cross-needle display, left needle for the forward and right needle for the reflected power; to read the SWR, follow the green line downwards from the point where the two needles cross]
</right>
---
Inserted in the line between transceiver and antenna, or already built into the transceiver

<left>
[picture:670:n_trx_kabel_swr_antenne:Schematic of an SWR meter between transceiver  and antenna]
</left>
<right>
[photo:67:n_swr_display:Display of a transceiver]
</right>
<note>
SWR meter and S meter sound similar but are different: the SWR meter measures the standing wave ratio when transmitting, the S meter the signal strength when receiving
</note>

---
[question:NI201]

---

[question:NF101]

---
[question:NI202]

---
## Good match

* With a perfect match, the value $\num{1}$ is shown
* The best value that can be achieved
* All the power is taken up by the antenna
* No power is reflected back into the transmitter

---
[question:NG301]

---
[question:NI203]

---
## Poor match

* With a poor match, close to infinity ($\infty$) is shown
* No antenna connected, transmission line broken or short-circuited
* Poor match of the antenna or damaged transmission line
* In the worst case, can destroy the transmitter

---

* With an SWR of $\num{2}$, $\qty{11}{\percent}$ of the transmit power is reflected
* With an SWR of $\num{3}$, $\qty{25}{\percent}$ of the transmit power is reflected
* Modern transceivers reduce the transmit power automatically to protect the transmitter

---
[question:NG302]

---

[question:NG303]

---
## High cable loss

* Reduces the reflected signal
* Falsifies the measurement
* For example with a long cable
* Signal is reduced on the way there and on the way back

---
[question:NG208]

<note>
* SWR appears to get better, but only the reflected power is attenuated
</note>
