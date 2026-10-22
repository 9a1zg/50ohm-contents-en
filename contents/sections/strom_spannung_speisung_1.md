An antenna is always fed with a voltage and a current that stand in a particular ratio to each other. This ratio is called the feed-point impedance.

For power to be delivered, there must always be voltage *and* current, because power is the product of voltage and current. If either the voltage or the current were zero, no power would be delivered or taken up.

Even so, we speak of *current-fed* antennas in some cases and of *voltage-fed* antennas in others. What is meant is that with some antennas there is a high current at a comparatively low voltage at the feed point, and with others a high voltage at a comparatively low current.


---

In a half-wave dipole, the feed-point impedance depends on where the antenna is fed. This is because in a dipole the charge carriers oscillate back and forth: in the middle, a particularly large number of charge carriers move, which we call a current antinode, and at the ends particularly high voltages arise, which we call a voltage antinode. Where no charges move, we speak of a current node, and where the voltage is zero, of a voltage node. Figure [ref:e_strom_spannung_speisung_dipol] shows the current and voltage distribution on the dipole. 

[question:EG203]

<margin>
[picture:787:e_strom_spannung_speisung_dipol:Half-wave dipole with voltage and current distribution]
</margin>

---

So if we feed a half-wave dipole in the middle, a large number of charges have to be moved, and we speak of a current-fed antenna (low feed-point impedance). An end-fed half-wave dipole, on the other hand, is a voltage-fed antenna (high feed-point impedance). Feeding at the end, as shown in Figure [ref:e_strom_spannung_speisung_dipol_ende], requires a matching network. We will only discuss this in more detail in Class A. 

<margin>
[picture:851:e_strom_spannung_speisung_dipol_ende:End-fed half-wave dipole]
</margin>

---

Accordingly, current-fed antennas have a low impedance and voltage-fed antennas a high impedance.

This is easy to illustrate with Ohm's law:

$ R = \frac{U}{I} $

If a dipole is fed in the middle, there is a comparatively low voltage there together with a high current. The quotient of voltage and current is therefore small, and the resulting resistance correspondingly low. If, on the other hand, it is fed at the end of the dipole, there is a high voltage there, while the current tends towards zero. This makes the quotient very large, and the resulting resistance takes on correspondingly high values.

With low resistances we also speak of *low-impedance* behaviour ($\downarrow\unit{\ohm}$), and with high resistances, accordingly, of *high-impedance* behaviour  ($\uparrow\unit{\ohm}$).

<indepth>
A typical order of magnitude for the *feed-point impedance* of a current-fed antenna is, for example, $\qty{36}{\ohm}$ to $\qty{100}{\ohm}$, and for voltage-fed antennas $\qty{1500}{\ohm}$ to $\qty{4000}{\ohm}$.
</indepth>

---

<indepth>
The current distribution on a dipole depends on the frequency at which the antenna is operated. Figure [ref:e_stromverteilungen] shows the current distribution for integer multiples of the fundamental frequency $f$ on a centre-fed dipole. It can be seen that at even multiples of the fundamental frequency there is a current node at the feed point. In this case the current there is very small, but the voltage is high, and the antenna appears as a high impedance at the feed point. For this reason, a centre-fed dipole is only resonant at odd integer multiples of the fundamental frequency. Use on several bands can be achieved by moving the feed point, for example to one of the current antinodes, as in Figure [ref:e_stromverteilungen]b (e.g. in the Windom antenna), or to the end of the antenna (e.g. the EFHW or Fuchs antenna). In these cases, however, antenna tuning units are needed, which we will only go into in more detail in Class A.
  
[picture:1050:e_stromverteilungen:Current distributions at different fundamental frequencies]
</indepth>

[question:EG204]
[question:EG205]
[question:EG206]