In Class E we have already met the open-wire feeder, also called ladder line (see Figure [ref:a_huenerleiter]). It consists of two conductors running in parallel. Provided twin feeders are fed and loaded in a balanced way, they also behave in a balanced way as regards their current and voltage distribution. This means that at any given point the current and the voltage on the two conductors have the same magnitude but opposite signs, as shown in Figure [ref:a_zweidrahtleitung].

<margin>
[photo:324:a_huenerleiter:Ladder line, also called twin feeder]
</margin>

The currents on the two conductors therefore flow in opposite directions at every instant. These are called *differential-mode currents*. As a result, the electromagnetic fields produced by the two conductors largely oppose each other at a greater distance and for the most part cancel out. A twin feeder operated in a balanced way therefore radiates only a little.

<margin>
[picture:1107:a_zweidrahtleitung:Current and voltage distribution on a twin feeder]
</margin>

If, on the other hand, the feeder is not completely balanced, *common-mode currents* can occur as well. Here part of the current flows in the same direction on both conductors. The fields produced by these currents do not cancel each other out. The feeder itself can then act like an antenna and radiate RF energy. Such common-mode components can arise, for example, if a dipole is not built exactly symmetrically, if an unbalanced antenna or load is connected, or if the transition between a balanced antenna and an unbalanced feeder is not decoupled by a suitable balun or common-mode choke.

[question:AG312]

In addition, stronger electromagnetic coupling can occur, especially in the near field of other lines or electrical equipment. For this reason feeders inside buildings are usually screened, for example in the form of coaxial cable. In a coaxial cable the electromagnetic fields of the differential mode lie largely between the inner conductor and the screen. This reduces both the radiation from the feeder and the coupling in of external interference.

[question:AG301]

A suitable screened cable is the coaxial cable, which we also met in Class E. Coaxial cables come in a wide variety of designs. The following question looks at the *RF properties* of coaxial cables, that is, their electrical properties at high frequencies. These are essentially:

* the characteristic impedance,
* the cable loss and the
* velocity factor,

which we look at more closely in a moment. The bending radius, on the other hand, is a mechanical property that states how tightly the cable may be bent where it is laid round a curve. The return loss states how much reflection there is, which depends on the load connected to a line and is therefore not a property of the cable.

[question:AG303]

The velocity factor results from the dielectric between the inner and outer conductors. Most of the electromagnetic wave carried by the cable is in this dielectric. The choice of dielectric determines how fast a wave can propagate through the cable. The velocity of propagation in a coaxial cable is lower than the speed of light in free space. Common materials for the dielectric are polyethylene (PE) and Teflon (PTFE). Foaming produces, in effect, a mixture with air, which gives a lower cable loss.

[question:AG314]
[question:AG302]

The velocity of propagation, reduced by the dielectric, is reflected in the velocity factor, which states the length to which a cable must be physically cut so that it has a particular electrical length (for example, so that it is a quarter of a wavelength long). For the velocity factor we find the following relationship on the formula sheet:

$k_\mathrm{v} = \frac{L_\mathrm{G}}{L_\mathrm{E}} = \frac{1}{\sqrt{\epsilon_\mathrm{r}}}$

Here $k_\mathrm{v}$ is the velocity factor, $L_\mathrm{G}$ the geometric ("mechanical") length and $L_\mathrm{E}$ the electrical length. The relative permittivity $\epsilon_\mathrm{r}$ depends on the dielectric used. For non-foamed polyethylene (PE), the formula sheet gives a relative permittivity of $\num{2.29}$.

[question:AG317]