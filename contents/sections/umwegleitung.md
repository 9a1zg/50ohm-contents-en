Another way of suppressing common-mode currents is to use a $\lambda / 2$ delay line.

[question:AG420]

<margin>
[picture:562:e_umwegleitung:Delay line]
</margin>

How such a delay line works is explained below.

A balanced antenna needs an RF voltage to earth at both of its terminals. The voltages must be equal in magnitude but of opposite sign, i.e. $\qty{180}{\degree}$ out of phase.

Such a phase shift can be obtained with a $\lambda / 2$ delay line. For example, *both* terminals of a folded dipole can be connected to the inner conductor, one of them being connected via a delay line that produces a $\qty{180}{\degree}$ phase shift.

The screen of the coaxial cable is then at earth potential, and no common-mode currents arise.

You do, however, have to be careful with the impedances. Although the delay line does not itself transform the impedance, connecting an antenna in this way still results in an impedance transformation. The antenna must have four times the impedance of the coaxial cable for it to be matched. The reason for this is that each terminal of the antenna has only half the resistance to earth, but both terminals are connected in parallel, i.e. both to the inner conductor.

---

<tip>
For the two following questions on the delay line it is enough to *remember* that the antenna shown is a folded dipole and that a $\lambda/2$ delay line produces a $\qty{180}{\degree}$ phase shift.
</tip>

[question:AG423]

<indepth>
*Connecting the coax screen* to the centre of the folded dipole is optional and often has mechanical reasons (e.g. it allows the folded dipole to be connected conductively to an earthed metal support).
</indepth>

---

[question:AG424]

<attention>
Although the circuit as a whole results in a 1:4 impedance transformation, no impedance transformation takes place in the delay line itself.
</attention>