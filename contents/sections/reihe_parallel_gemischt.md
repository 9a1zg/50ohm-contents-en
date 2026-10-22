In Class E we have already learnt how capacitors behave in series and in parallel. The previous chapter also covered inductors in series. In this chapter we now look at the parallel connection of inductors and capacitors. First, however, we go over the basic relationships for capacitances in parallel and in series once more.

In parallel tuned circuits, inductors and capacitors are combined. A real inductor also has a certain self-capacitance. This arises, for example, from the windings of the coil and the resulting electric-field coupling between the turns.

To calculate the resonant frequency as accurately as possible, these "invisible" capacitances must be taken into account. In the following question, the capacitances of the capacitors and the self-capacitance of the inductor can be added directly, as they are in parallel with each other.

It is particularly important here to watch out for the different units. Before calculating, all the values should therefore be converted to the same unit, so that the capacitances can be added correctly.

[question:AD103]

In the following question, three capacitors are connected in series. In Class E we learnt that for capacitors in series, the reciprocals of the capacitances add up:

$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{C_{1}} + \frac{1}{C_{2}} + \frac{1}{C_{3}}$

Here too, the capacitances must be converted to the same unit before calculating, so that the reciprocals can be added correctly.

[question:AD101]

---

In AC circuits, besides the familiar ohmic resistances, there are also reactances, which we have already met with capacitors and inductors. The ordinary ohmic resistance is called the resistive part, or simply the resistance $R$. Reactances are denoted by $X$. Both kinds of resistance affect the current flowing in the circuit at the same time.

Since resistance and reactance act differently, they cannot simply be added. Instead, they are combined geometrically. You can picture this as a right-angled triangle, as in Figure [ref:a_dreieck]:

---

- The resistance $R$ forms the horizontal side.
- The reactance $X$ forms the vertical side.
- The resulting total resistance is the magnitude of the impedance, $|Z|$, which German calls the *Scheinwiderstand*.

<margin>
[picture:1067:a_dreieck:Right-angled triangle illustrating how the magnitude of the impedance $|Z|$ is calculated from the resistance $R$ and the reactance $X$]
</margin>

The magnitude of the impedance can be calculated with Pythagoras' theorem (see the formula sheet):

$ |Z| = \sqrt{R^2 + X^2} $

The letter $Z$ is used for what is called the impedance. For the calculations in this chapter, however, it is enough to regard its magnitude $|Z|$ as the total AC resistance of the circuit.

<indepth>
For the mathematically minded: the impedance $Z$ is a complex quantity with the resistance $R$ as its real part and the reactance $X$ as its imaginary part:

$Z = R + jX$

The magnitude $|Z|$ is then the length of the vector in the complex plane that results from combining $R$ and $X$.
</indepth>

For the next question, before we can apply Pythagoras' theorem, the reactance $X_C$ of the capacitor at $\qty{1}{\mega\hertz}$ has to be calculated. For this we use the formula for the reactance of a capacitor.

[question:AD104]

The next question deals with calculating the magnitude of the impedance of a series circuit of a resistor and an inductor. First we calculate $X_L$, then we again apply Pythagoras' theorem. Here too, the powers of ten must be taken into account so that the calculation can be carried out correctly.

[question:AD105]
