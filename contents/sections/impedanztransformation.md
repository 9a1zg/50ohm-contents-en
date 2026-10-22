Not every antenna has, at its feed point, exactly the impedance needed for connection to a particular feeder or transmitter. If the impedance differs, for example, from the usual $\qty{50}{\ohm}$, it must be matched accordingly so that the RF power can be transferred with as little loss as possible. To do this, the existing impedance is *transformed* into another, desired impedance. This is called *impedance transformation* or *impedance matching*.

There are various ways of carrying out impedance matching or impedance transformation. Frequently used are, for example:

* transformers,
* $\frac{\lambda}{4}$ lines or
* matching networks made of inductors and capacitors.

We have already met transformers with the end-fed antenna and its 1:49 unun. Below, we therefore look more closely at two further possibilities: impedance transformation with $\frac{\lambda}{4}$ lines from the previous section, and matching with LC networks. Let us first look again at transformer sections; incidentally, it makes no difference here whether we use a balanced feeder or an unbalanced coaxial line, as the transformation works in both cases:

On a line whose electrical length is $\lambda/4$, resistances lower than the characteristic impedance of the line become resistances higher than the characteristic impedance of the line. Conversely, resistances higher than the characteristic impedance of the line become resistances lower than the characteristic impedance. This is used, for example, to match high-impedance antennas to a low-impedance system ($\qty{50}{\ohm}$).

[question:AG410]
[question:AG409]

With a line length of $\lambda/2$, however, the effect cancels out again, so that no impedance transformation takes place.

[question:AG412]
[question:AG416]

For the following questions, remember that a half-wave dipole is current-fed (low impedance) and a full-wave dipole is voltage-fed (high impedance).

[question:AG413]
[question:AG414]
[question:AG415]

To transform to a particular resistance value, the characteristic impedance needed is the geometric mean of the load resistance $Z_\mathrm{A}$ and the desired input impedance $Z_\mathrm{E}$ at the other end of the cable:

$Z = \sqrt{Z_\mathrm{E} \cdot Z_\mathrm{A}}$

[question:AG417]
[question:AG418]

---

Often, however, inductors and capacitors are also used for impedance matching. A circuit often found is what is called the pi filter, which as well as acting as a low-pass filter also brings about an impedance transformation. Such a pi filter can accordingly also be used as an antenna tuner.

<indepth>
*The name "pi filter"* comes from the arrangement of the components in the circuit diagram, which resembles the Greek letter $\pi$, and has nothing to do with the number $\pi$.
</indepth>

[question:AG406]
