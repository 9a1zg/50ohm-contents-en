With antennas, we have to distinguish between the *mechanical* and the *electrical length*. The mechanical length is simply the actual, measurable length of the antenna wire or radiator. The electrical length, on the other hand, describes how long the antenna behaves electrically at the frequency in question. It can be changed by coils and capacitors, among other things, without the mechanical length of the radiator having to be changed.

Let us first look at antennas close to their fundamental resonance. A half-wave dipole is resonant at a total length of roughly $\lambda/2$, a ground plane with a single vertical radiator at a radiator length of roughly $\lambda/4$. If such an antenna is too short for the wanted frequency, its feed-point impedance has a *capacitive* reactive part. A coil can compensate for this capacitive reactive part. This is called *electrical lengthening* of the antenna. If, on the other hand, the antenna is too long for the wanted frequency, its feed-point impedance has an *inductive* reactive part. This can be compensated for with a capacitor. This is called *electrical shortening*. So a coil lengthens an antenna electrically, and a capacitor shortens it electrically. The mechanical length of the radiator stays the same.

<margin>
[picture:1134:a_5_8_lambda_strahlung:Radiation patterns and current distribution of vertical antennas over perfect earth]
</margin>

---

An interesting example is the $\frac{5}{8}\lambda$ vertical antenna, with a length of $\qty{0.625}{\lambda}$ (see Figure [ref:a_5_8_lambda]). Mechanically, its radiator is therefore about 2.5 times as long as that of an ordinary $\frac{\lambda}{4}$ ground plane ($\qty{0.25}{\lambda}$). The greater radiator length changes the vertical radiation pattern to advantage, as shown in Figure [ref:a_5_8_lambda_strahlung]: more of the radiated power is concentrated towards the horizon, and less is radiated upwards or downwards. For terrestrial contacts this usually gives a greater range for the same power. A radiator length of about $\frac{5}{8} \lambda$ is optimal for this effect: if the radiator is made longer still, more power is again lost upwards and downwards.

However, with a radiator length of $\frac{5}{8}\lambda=\qty{0.625}{\lambda}$ this antenna is not resonant. For resonance, the radiator would have to be shortened to $\frac{\lambda}{2}=\qty{0.5}{\lambda}$ or lengthened to $\frac{3}{4}\lambda=\qty{0.75}{\lambda}$. Either would lead to less power at the horizon. Because of the better concentration, it is advisable to leave the radiator length at $\frac{5}{8}\lambda$ and to establish resonance electrically, that is, to lengthen the antenna electrically. One of several ways of doing this is a base loading coil. The coil provides an inductive reactive part that compensates for the capacitive reactive part of the $\frac{5}{8}\lambda$ radiator. The impedance obtained in this way is very similar to the impedance of an antenna with a radiator length of $\frac{3}{4}\lambda=\qty{0.75}{\lambda}$. 

<margin>
[picture:650:a_5_8_lambda:$\qty{5}{8}\lambda$ vertical antenna]
</margin>

[question:AG106]

---

Conversely, an antenna that is mechanically somewhat too long close to its fundamental resonance can be shortened electrically by a capacitor (see Figure [ref:a_verkuerzung]). The capacitor provides a capacitive reactive part and so compensates for the inductive reactive part of the radiator that is too long.

[question:AG107]

<margin>
[picture:563:a_verkuerzung:Vertical antenna with shortening capacitor]
</margin>

---

For a dipole, too, its mechanical length can first be used to estimate whether electrical lengthening or shortening is needed for the wanted fundamental resonance.

[question:AG108]