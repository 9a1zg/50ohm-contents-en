As shown in Figure [ref:a_nahfernfeld], the electromagnetic field of an antenna can be divided into the *near field* in the immediate vicinity of the antenna and the more distant *far field*. The near field is further divided into the *reactive near field* and the *radiating near field*.

<tip>
In the [Explanations of the assessment procedures under the BEMFV](https://50ohm.de/bemfv), the Federal Network Agency (Bundesnetzagentur, BNetzA) has explained the terms and procedures for determining the safety distances.
[photo:80:n_Bewertungsverfahren:The assessment procedures are described in this document.]
</tip>

[picture:1113:a_nahfernfeld:Distance definitions for the near field and the far field according to the Federal Network Agency (BNetzA).]

---

According to the definition of the Federal Network Agency (BNetzA) used in the figure, the reactive near field extends to a distance of

$d \le \dfrac{\lambda}{2 \cdot \pi}$

from the antenna, where $\lambda$ is the wavelength. At greater distances the radiating near field begins. The distance of this boundary therefore depends on the wavelength. For a wavelength of $\qty{20}{\meter}$, for example, we get:

$d = \frac{\qty{20}{\meter}}{2 \cdot \pi} \approx \qty{3.18}{\meter}$

In this example the reactive near field therefore extends to a distance of about $\qty{3.18}{\meter}$ from the antenna.

In the reactive near field of an antenna, the electric field strength and the magnetic field strength have no constant phase relationship to each other. What exactly this means is explained in more detail in the in-depth box alongside. 

[question:AK101]

If you look at how the electric and magnetic fields of a dipole antenna vary across these regions in Figure [ref:a_dipol_feld_e_h], you can see that the two field quantities do not have the same magnitudes. The electric field is much stronger than the magnetic field. With a magnetic loop antenna, in Figure [ref:a_loop_feld_e_h], it is exactly the other way round: the magnetic field is much stronger than the electric field.

<margin>
[picture:1114:a_dipol_feld_e_h:Electric and magnetic field strength of a dipole antenna across the near-field and far-field regions (logarithmic).]
[picture:1115:a_loop_feld_e_h:Electric and magnetic field strength of a loop antenna across the near-field and far-field regions (logarithmic).]
</margin>

<indepth>
For the mathematically minded who are already familiar with complex numbers, here is a simplified explanation of why the electric and magnetic field strength in the reactive near field have no phase relationship to each other that is independent of position.
For an electrically short dipole, the fields are made up, in simplified form, of several components:

$ \underline{E}(r)~=~\left( \underbrace{\frac{A}{r^3}}_{\text{quasi-static}} + \underbrace{j\,\frac{B}{r^2}}_{\text{inductive}} + \underbrace{\frac{C}{r}}_{\text{radiation}} \right) e^{-jkr}$

$ \underline{H}(r)~=~\left( \underbrace{j\,\frac{D}{r^2}}_{\text{inductive}} + \underbrace{\frac{F}{r}}_{\text{radiation}} \right) e^{-jkr}. $

The underlined quantities are complex and describe not only the strength but also the phase of each field component. Factors such as $j$ or $-j$ in the complete field equations correspond to phase shifts of $\qty{90}{\degree}$ and $\qty{-90}{\degree}$ respectively.

Since the individual components decrease at different rates with the distance $r$, their ratio to each other changes. As a result, the phase difference between the electric and magnetic field strength in the near field also depends on the distance, the direction and the form of the antenna.

For a full understanding, the individual vector components of the field equations have to be considered. These relationships go well beyond the syllabus of Class A and are not relevant to the examination.
</indepth>

Especially in the reactive near field, high local field strengths can occur because of the strong electric or magnetic field components, which fall off rapidly with increasing distance. This region is called *reactive* because a large part of the field energy is not radiated but oscillates back and forth between the antenna and the field. Just as with a capacitor (electric field) or an inductor (magnetic field), the energy stored in the reactive near field is not consumed but returned to the antenna with a phase shift – this oscillation between field and antenna corresponds to the reactive part of the antenna impedance, while only the resistive part (radiation resistance) describes power actually radiated.

In the *radiating near field*, in the region

$\frac{\lambda}{2\pi} < d < 4\cdot\lambda$

the radiated field components increasingly come to the fore. The ratio of the electric and magnetic field strength comes closer and closer to that in the far field. The antenna does not, however, start radiating only in this region; it radiates in any case. It is merely that the reactive field components become less important with increasing distance. For many simplified considerations, the radiating near field can already be treated much like the far field. We will come back to this in more detail later.

According to the definition used here, the *far field* begins at a distance of

$d \ge 4\cdot\lambda$

from the antenna. In this region the electric and the magnetic field strength each decrease in proportion to $\frac{1}{d}$. In addition, the two field components are in a fixed ratio to each other and have a constant phase relationship.

---

The ratio of the magnitudes of the electric and magnetic field strength is called the *wave impedance*:

$Z_\mathrm{F}(d)=\left|\frac{E(d)}{H(d)}\right|$

Figure [ref:a_feldwellenwiderstand] shows how the wave impedance changes with increasing distance from the antenna. In the reactive near field it depends strongly on the form of the antenna, the direction under consideration and the distance. There it can be considerably greater or smaller than the impedance of free space.

In the radiating near field, the ratio of the electric and magnetic field strength comes closer and closer to the value for free space. In the far field it is finally constant and is approximately:

$Z_0 = \sqrt{\dfrac{\mu_0}{\varepsilon_0}} \approx \qty{120\pi}{\ohm} \approx \qty{377}{\ohm}$

The impedance of free space links the electric and magnetic field quantities. It is a measure of how strong the electric field strength is in relation to the magnetic field strength. 

[question:AK102]

We must remember this value, since we need it to derive the approximation formula. 

To sum up: 

* The far field of a source of radiation is the region in which the vectors of the electric field strength (E), the magnetic field strength (H) and the direction of propagation are at right angles to each other and have no phase differences. In addition, the wave impedance must be equal to that of free space. 
* The boundary between the far field and the near field depends primarily on the wavelength. However, the type of antenna used and its surroundings do play a part. With the wire antennas mostly used in amateur radio (e.g. dipoles), the far field forms at a distance of about $4\cdot\lambda$. 

<margin>
[picture:1116:a_feldwellenwiderstand:Wave impedance across the near-field and far-field regions (logarithmic).]
</margin>