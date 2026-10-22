As we have already learnt, a half-wave dipole can also be fed at one end. With a wire length of $\lambda / 2$ or multiples of it, the feed-point impedance is high (approx. $\qtyrange{2000}{2500}{\ohm}$).

There are various ways of matching such an end-fed antenna. Below we look at three typical variants:

* Fuchs circuit
* Transformer for impedance matching
* Zepp antenna

One way of matching is the Fuchs circuit already discussed (see Figure [ref:a_fuchskreis]). It is a parallel tuned circuit tuned to the operating frequency. It transforms the low impedance of the feeder to the high feed-point impedance of the end-fed half-wave antenna and at the same time compensates for any reactive components.

<margin>
[picture:310:a_fuchskreis:Fuchs circuit for matching an end-fed half-wave antenna]
</margin>

[question:AG419]

---

Another possibility is a transformer (see Figure [ref:a_unun_1_49]) with a transformation ratio of $ü = 1:7$. Since voltage and current are multiplied and divided respectively by a factor of $\num{7}$, the resistance is transformed by $1:7^2 = 1:49$, corresponding to $(1 \cdot \qty{50}{\ohm}) : (49 \cdot \qty{50}{\ohm}) = \qty{50}{\ohm} : \qty{2450}{\ohm}$.

<margin>
[photo:332:a_unun_1_49:1 to 49 unun for matching an end-fed half-wave antenna]
[picture:315:a_endspeisung_1:End-fed half-wave dipole with pigtail]
[picture:260:a_endspeisung_2:End-fed half-wave dipole with coaxial cable as counterpoise]
</margin>

<attention>
For *impedance transformation* (the transformation of the resistance), the turns ratio of a transformer enters squared, i.e. a transformer with a turns ratio of 1:7 gives a 1:49 impedance transformation. With baluns and ununs it is often not stated whether the turns ratio or the impedance ratio is meant, so the two can be confused. It is usual to give the impedance ratio. A transformer with a turns ratio ($ü$) of 1:7 is then called, for example, a 1:49 unun.
</attention>

A short piece of wire (at least a twentieth of the wavelength), see Figure [ref:a_endspeisung_1], or part of the coaxial feed cable (at least $\qty{0.05}{\lambda}$), see Figure [ref:a_endspeisung_2], is often used as the counterpoise. A common-mode choke (in German *Mantelwellensperre*, abbreviated MWS) prevents the rest of the feed cable from becoming part of the antenna.

[question:AG123]
[question:AG124]

---

Instead of a Fuchs circuit or a transformer, a $\lambda / 4$ length of twin feeder can also be used. This is then called a *Zepp antenna*, short for Zeppelin antenna (see Figure [ref:a_zeppelinantenn]). How a line transforms an impedance will be looked at more closely in a later section.

The name goes back to the use of these antennas on airships. Because of the $\lambda / 4$ long twin feeder, the high voltage only occurs at its end, and therefore far away from the gas-filled airship (see Figure [ref:a_zeppelinantenne_foto]).

<margin>
[picture:314:a_zeppelinantenne:Construction of a Zepp antenna]
[photo:336:a_zeppelinantenne_foto:Zepp antenna (illustrative photo)]
</margin>

[question:AG120]

---

Just as with an end-fed half-wave dipole, a feeder with a different characteristic impedance can also be used for matching with other types of antenna. For Class E we have already met the full-wave loop antennas, among them the delta loop and the quad antenna. A delta loop antenna (see Figure [ref:a_delta_loop]) with sides of equal length has a feed-point impedance of about $\qty{100}{\ohm}$. Inserting a $\lambda / 4$ line with a characteristic impedance of $\qty{75}{\ohm}$ transforms this to the $\qty{50}{\ohm}$ usual in amateur radio.

<margin>
[picture:311:a_delta_loop:Delta loop antenna]
</margin>

[question:AG117]

<indepth>
The optimum value for the characteristic impedance of a $\lambda / 4$ feeder used for matching is the *geometric mean* of the two impedances, e.g. of $\qty{50}{\ohm}$ and $\qty{100}{\ohm}$, giving $\sqrt{\qty{50}{\ohm} \cdot \qty{100}{\ohm}} \approx \qty{70.7}{\ohm}$.
</indepth>

If the full-wave loop is made as a square, each side must accordingly be a quarter of the wavelength long.

[question:AG119]

<attention>
As with the dipole, the mechanical length of a full-wave loop antenna differs from its electrical length. Unlike the shortening factor of dipoles, however, full-wave loops surprisingly have a *lengthening factor*, i.e. the antenna must be a few per cent longer than one wavelength in free space would be.
</attention>

---

Since frequency bands have different propagation conditions at different times of day, seasons and phases of the solar cycle, radio amateurs like to be able to operate on as many frequency bands as possible. Two examples of multiband antennas are the *G5RV antenna with two legs of equal length* (see Figure [ref:a_g5rv]) and a twin feeder, and the *off-centre-fed Windom antenna* (see Figure [ref:a_windom]); in both, clever dimensions give many resonances and thus use on as many amateur bands as possible.

<margin>
[picture:313:a_g5rv:G5RV antenna]
[picture:309:a_windom:Windom antenna]
</margin>

[question:AG121]
[question:AG122]

---

% TODO: Darstellung von $5/8 \lambda$ prüfen

That an antenna is resonant does not yet mean that it also has a good radiation pattern. The lowest possible angle of radiation is often wanted. For vertical antennas fed against earth, a length of approx. $5/8 \lambda$ turns out to be the optimum.

<indepth>
A simple wire with earth as the other pole is not resonant at a length of $5/8 \lambda$. Resonances only occur at $1/4$, $3/4$, $5/4$ and so on. Matching is therefore necessary. This is usually achieved by inserting a coil that lengthens the electrical length from $5/8$ to $6/8$ (i.e. $3/4$). Such coils are often seen on vehicle antennas.
% TODO: Bild VHF oder CB-KFZ-Antenne
</indepth>

<attention>
The optimum of $5/8 \lambda$ only applies to antennas fed against earth. If, for example, centre-fed dipoles are considered that are either in free space or vertical, just above the ground, the optimum is $5/4 \lambda$.
% TODO: Frage ist falsch, siehe 2. Review von DL9JBE.
</attention>

[question:AG223]