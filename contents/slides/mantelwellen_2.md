## Differential-mode signal and common-mode currents

* Ideally, equal and opposite currents flow in the inner and outer conductors of a coaxial cable
* Their sum is zero – a pure differential-mode signal
* A pure differential-mode signal prevents common-mode currents from occurring

---
### Common-mode signal and sheath current

* If the sum of the currents is not zero, a common-mode signal results
* The common-mode component flows on the outside of the outer conductor as a sheath current
* The sheath current produces a sheath wave around the cable

---
[question:AG425]

---
### Current-compensated choke

* Coaxial cable wound on a ferrite core suppresses common-mode currents
* This design is called a current-compensated choke

---
[question:AG426]

---
## RF isolating transformer to block common-mode currents

* Alternative: an RF isolating transformer, whose primary and secondary windings are not connected
* Current that flows in at one terminal flows out at the other with almost the same magnitude – no common-mode component

<note>
Capacitance forms between the turns of the windings, so that the common-mode component is not suppressed completely
</note>

---
[question:AJ115]

---
### RF voltages and common-mode currents

* No RF common-mode signals: the outer conductor shows no RF voltage to earth
* With differential-mode signals the electric field forms only between the inner and outer conductors
* Seen from outside: the currents cancel – no common-mode currents
* Common-mode currents are directly linked to RF voltages on the outer conductor

---
## Balanced antennas and outer-conductor voltage

* With a balanced antenna, each dipole leg has a voltage to earth
* Connecting the antenna legs to the conductors of the coaxial cable leads to an RF voltage on the outer conductor

---
### Effect of earthing on antennas

* Well-earthed antennas (e.g. a ground plane with tuned or buried radials) have almost $\qty{0}{\volt}$ at the feed point
* Poorly earthed ground-plane antennas can be prone to common-mode currents

---
## Contactless coupling into the coax screen

* Common-mode currents can arise through contactless coupling
* If a feeder is run parallel to a dipole leg, the near field of the antenna couples into the coax screen

---
[question:AG427]

---
### Voltage balun / autotransformer

<left>
[picture:447:a_mantelwellen_spannungsbalun:Construction of a voltage balun]
</left>
<right>
* With completely balanced antennas, a voltage balun can balance the currents in the coaxial cable
* Typical autotransformer: coaxial cable connected to the centre and one end of a coil, antenna to both ends of the coil
</right>

---

<left>
[picture:447:a_mantelwellen_spannungsbalun:Construction of a voltage balun]
</left>
<right>
* Doubling the voltage ($ü = 2$) and halving the current give a 1:4 impedance transformation
* A $\qty{50}{\ohm}$ coaxial cable is ideally connected to an antenna of approx. $\qty{200}{\ohm}$
</right>

---
[question:AG421]

---
[question:AG422]

---
## Limitations of the common-mode choke


* A voltage balun only works if the connected antenna is actually balanced
* Uneven loading can encourage common-mode currents
* Contactless coupling via the electromagnetic near fields remains possible
* An additional common-mode choke some distance away can help

---
[question:AG428]

---
[question:AG429]
