In Class N we have already come across some types of antenna. In Class E we now want to discuss the properties of the various antennas in more detail. Centre-fed dipoles are *balanced antennas*. By a balanced antenna we mean an antenna that, ideally, has in operation the same voltage with respect to earth at both poles (e.g. the feed points of each leg of a dipole), apart from the sign. This is the case with dipoles, including the folded dipole, and also with the Yagi-Uda antennas based on them. A ground-plane antenna, on the other hand, ideally has earth potential at the point where the radials are connected (i.e. a voltage of zero with respect to earth) and is therefore not one of the balanced antennas.

<indepth>
Cables for signal transmission, e.g. the feeder of an antenna, are also divided into *balanced and unbalanced cables*. Here too, balance refers to the voltages with respect to earth that are present in the ideal case. In a coaxial cable, the currents should indeed be balanced, but only the inner conductor should carry a voltage with respect to earth. Coaxial cables are therefore unbalanced feeders. As we will learn later, these unbalanced feeders should only be connected to a balanced antenna by means of what is known as a balun.
</indepth>

[question:EG213]

---

A popular type of antenna is a wire about one wavelength long in total, in the shape of a circle, a square, a triangle or a similar shape. These are known as full-wave *loop antennas*. Because it is so simple to build, the delta loop antenna is very popular; like the capital delta (Δ) of the Greek alphabet, it has the shape of a triangle.

<margin>
[picture:311:e_delta_loop:Example of a delta loop antenna]
</margin>

[question:EG101]

<indepth>
The exact *shape* of a full-wave loop antenna does not matter, as long as the length of the wire is about one wavelength. Depending on the shape, however, different feed-point impedances or slightly higher or lower antenna gains can result.
</indepth>

---

Full-wave loop antennas must be distinguished from the *magnetic loop antennas*, which are much smaller in relation to the wavelength and produce a magnetic near field (see Figure [ref:e_mag_loop]).

<margin>
[picture:977:e_mag_loop:Example of a magnetic loop antenna]
</margin>

[question:EG105]

<indepth>
Although such magnetic loop antennas are in principle also suitable for transmitting, it is difficult to achieve a high *efficiency*. Efficiencies between $\qty{1}{\percent}$ and $\qty{10}{\percent}$ are usual for magnetic antennas used for transmitting. Nevertheless, these magnetic loops can offer advantages over other antennas: apart from their compact construction, they are often less affected by electrically conductive or attenuating objects in the near field, e.g. walls or roof tiles when mounted indoors or under a roof. 
</indepth>

---

*End-fed antennas* are fed from one end. Their length is usually half a wavelength. They are then also called end-fed half-wave dipoles (EFHW). Such an antenna needs a voltage that is considerably higher in relation to the current, and this can be produced by a suitable matching network, e.g. a Fuchs matching circuit. End-fed half-wave dipoles matched with a Fuchs circuit are accordingly called Fuchs antennas.

[question:EG104]
[question:EG103]

<margin>
[picture:310:e_fuchsantenne:Example of a Fuchs antenna]
</margin>

<person>
The Fuchs circuit and the Fuchs antenna are named after *Dr Josef Fuchs* (amateur call signs OE1JF, UO1JF and EAAA), who also patented them in 1927.
</person>

<indepth>
An end-fed antenna also needs a *counterpoise*, e.g. in the form of a $\lambda / 4$ wire or some other form of RF earth. However, the currents at the feed point of EFHWs are considerably smaller, which is why a poorer earth can be enough, e.g. a short piece of wire only a tenth or even a twentieth of the wavelength long. Sometimes even just the screen of the feeder or other metal parts (actually intended for other purposes) serve as the earth.
  
End-fed *long-wire antennas*, whose length is well over one wavelength, must not be confused with end-fed half-wave dipoles. The confusion arises because end-fed half-wave dipoles are often also operated on higher frequencies, where they are then de facto long-wire antennas for those frequencies.
</indepth>

---

The directional properties of an antenna can be shown in what is known as a radiation pattern. For one plane, the gain, or the field strength or radiated power, is plotted for each direction. The farther the curve is from the centre, the greater the gain, or the higher the field strength and radiated power in the far field. If no angle scale is used, the mechanical arrangement of the antenna is often shown in the same diagram as well, to make clear which direction in the diagram corresponds to which direction relative to the antenna.

A dipole does not radiate in the direction of the wire, as one might mistakenly assume, but at right angles to it. Viewed in one plane and plotted as a radiation pattern, this gives corresponding lobes (e.g. left and right) beside the dipole (see Figure [ref:e_dipol_strahlungsdiagramm]). A vertically suspended dipole therefore radiates, for example, to the left and right as well as to the front and back. Since the radiation pattern only looks at one plane, you only see, for example, one lobe for the radiation to the left and one lobe for the radiation to the right. Depending on the scale, these lobes may look circular.

<margin>
[picture:1045:e_dipol_strahlungsdiagramm:Example of the radiation from a dipole]
</margin>

<indepth>
A lobe with a *circular* cross-section results, on a scale linear in field strength, when a very short dipole (Hertzian dipole) is considered. A half-wave dipole actually has a slightly higher gain, corresponding to a slightly narrower lobe. Nevertheless, the examination questions show a circular pattern, which is only approximately correct. On a scale linear in the radiated power in each direction, the lobe would have to be narrower still.
% TODO: ggf. Fragenbild korrigieren
</indepth>

[question:EG215]
[question:EG214]

---

Because a dipole radiates at right angles to itself, a vertically mounted half-wave dipole can accordingly give a low angle of radiation, which may be desirable, e.g., in DX operation, but also for contacts via the direct wave or ground wave.

[question:EG219]

<margin>
[photo:316:e_vertikaldipol:Vertical $\frac{\lambda}{2}$ dipole]
</margin>

---

A special case of a vertical antenna is the $\frac{5}{8}\lambda$ antenna fed against earth (or a vehicle body) (see Figure [ref:e_fuenf_achtel]). Here the length, which works out at $\qty{0.625}{\lambda}$, is chosen for a particular reason. The radiator is thus mechanically about 2.5 times as long as that of a normal $\frac{\lambda}{4}$ ground plane ($\qty{0.25}{\lambda}$). The greater radiator length changes the vertical radiation pattern favourably, as shown in Figure [ref:a_5_8_lambda_strahlung]: more of the radiated power is concentrated towards the horizon, and less is radiated upwards or downwards. For terrestrial contacts, this generally gives a greater range for the same power. A radiator length of about $\frac{5}{8} \lambda$ is optimum for this effect: if the radiator is lengthened further, more power is again lost upwards and downwards.

[question:EG108]

<margin>
[picture:1134:a_5_8_lambda_strahlung:Radiation patterns and current distribution of vertical antennas over perfect earth]
[picture:650:e_fuenf_achtel:$5/8 \lambda$ antenna]
</margin>

---

A ground-plane antenna also radiates at right angles to the radiator (not to the radials). Since the radiation pattern often shows the ground-plane antenna viewed from above, the result is almost an omnidirectional antenna, with almost the same gain in all directions (see Figure [ref:e_ground_plane_abstrahlung]). The radials have only a small influence and can "dent" the radiation pattern slightly, which corresponds to a slightly different gain in certain directions.

<margin>
[picture:1046:e_ground_plane_abstrahlung:Radiation from a ground-plane antenna]
</margin>

[question:EG216]

<indepth>
Even if the radiation pattern of a ground-plane antenna with radials is slightly *"dented"*, in theory this deviation is much smaller than is often shown. A ground-plane antenna is therefore in fact an almost ideal omnidirectional antenna in the plane.
</indepth>

---

Directional antennas (e.g. the Yagi-Uda antenna) are characterised by a gain that is considerably higher in one direction than in other directions, as shown in Figure [ref:e_richtantenne_abstrahlung].

[question:EG217]

<margin>
[picture:1047:e_richtantenne_abstrahlung:Radiation from a directional antenna]
</margin>

---

At higher frequencies, e.g. in the UHF range or above, horn antennas or parabolic antennas (see [ref:e_parabolantenne]) are also used. Patch antennas are likewise found on the circuit boards of smaller devices. All these types of antenna are unusual in the HF range, as they would become unwieldy in size. That leaves only the long-wire antenna, Yagi-Uda antenna, dipole antenna, Windom antenna and delta loop antenna for the following questions.

[question:EG106]

<margin>
[picture:850:e_parabolantenne:Parabolic antenna]
</margin>

The sleeve dipole consists of a $\lambda / 4$ long sleeve that acts as a balun or common-mode choke. With this knowledge the following question can be answered, because a sleeve dipole and a crossed Yagi-Uda, just like a parabolic dish, would be unwieldy in size on the $\qty{80}{\meter}$ band.

[question:EG107]