In Class E we have also already dealt with the inductor. With direct current, in the steady state, the inductor has a very small resistance. The inductor then acts like a piece of wire. With alternating current, however, the inductor, like a capacitor, has an AC resistance $X_{\textrm{L}}$: although the wire of the coil has only a very small ohmic resistance (conductor resistance), the current that flows becomes smaller as the frequency of the AC voltage rises:

$|X_{L}| = \omega \cdot L = 2\cdot\pi\cdot f \cdot L$

The formula shows that the AC resistance rises as the frequency increases and falls as the frequency decreases. Unlike that of the capacitor, the AC resistance of an inductor is positive. 

<indepth>
Why is the inductive reactance positive? The reason again lies in complex AC calculation, which is not strictly necessary for the amateur radio examination.

For readers who know complex numbers, however, it should be mentioned that the correct form of the inductive reactance is actually

$X_L = j\omega L$

Here $j$ again stands for the imaginary unit $\sqrt{-1}$.

This shows that the inductive reactance is not only positive but also complex. The positive sign describes the phase relationship between current and voltage in the inductor, which we will look at more closely in this chapter.
</indepth>

[question:AC202]

[question:AC203]

---

A vector network analyser (VNA) can display how the inductive reactance $X_L$ changes with frequency (see Figure [ref:a_XL_Verlauf]). 

<margin>
[photo:265:a_XL_Verlauf:Change in the inductive reactance $X_L$ of an inductor from $\qty{500}{\kilo\hertz}$ to $\qty{10}{\mega\hertz}$]
</margin>

Now try to answer the following question with the formula above. Pay particular attention to the units and the powers of ten so that you get the right results.

[question:AC204]

---

As with the capacitor, there is also a phase shift between voltage and current in the inductor. It is $\qty{+90}{\degree}$, with the current lagging the voltage, as shown in Figure [ref:a_Blindleistung_Spule]. The red line in Figure [ref:a_XL_Verlauf] shows the phase of the inductive reactance $X_L$ at approx. $\qty{+90}{\degree}$.

<tip>
Memory aid: Bei der Induktivit*äää*t kommt der Strom zu sp*äää*t! (in the inductance, the current comes too late)
</tip>

[question:AC201]

This gives a power curve that swings symmetrically about the zero line. The mean value of this power is zero, which means that – just as with the capacitor – no real power is absorbed. Instead, energy is periodically stored in the magnetic field of the inductor and returned to the source.

For an ideal, lossless inductor we therefore speak of reactive power and a reactance.

<margin>
[picture:944:a_Blindleistung_Spule:The product $U \cdot I$ gives the green power curve]
</margin>

If an inductor gets warm in radio-frequency applications, it has losses that cause this heating. The losses arise from the ohmic resistance of the wire, and in addition there is the skin effect, which effectively reduces the cross-sectional area of the wire. Here too, as with the capacitor, the Q factor $Q$ or the dissipation factor $\tan\delta$ is used to describe the losses.

[question:AC209]

---

We have now met the capacitive reactance $X_C$ of the capacitor and the inductive reactance $X_L$ of the inductor. Both quantities depend on frequency and, together with the ohmic resistance $R$, make up the so-called *impedance* $Z$ of a component.

The reactances $X_L$ and $X_C$ act in opposite directions and can partly or completely cancel each other. To combine the reactances with the ohmic resistance, however, simple algebraic addition is not possible; geometric addition is needed. This is done with Pythagoras' theorem (see Figure [ref:a_impedanzdreieck]).

The result is the impedance $Z$, which describes the complex total resistance of a component. The magnitude of the impedance, $|Z|$, is what German calls the *Scheinwiderstand* (in English usually also just called the impedance):

$Z = \sqrt{R^2 + (X_L - X_C)^2}$ 

or, simplified (see the formula sheet – keyword: impedance (*Scheinwiderstand*)):

$Z = \sqrt{R^2 + X^2}$ 

In radio-frequency engineering, impedance plays a central part, because it determines how components behave in circuits and is crucial in particular for matching lines, antennas and amplifiers. It is given in ohms ($\unit{\ohm}$) and describes the total resistance of a component when operated with alternating current. A series connection of reactance and resistance gives an impedance $Z$, which appears only when operated with AC voltage and cannot be measured with an ohmmeter. 

<margin>
[picture:1067:a_impedanzdreieck:Impedance $Z$ as the geometric sum of $R$ and $X$]
</margin>

<indepth>
The impedance $Z$ is a complex quantity that takes into account both the ohmic resistance $R$ and the reactances $X_L$ and $X_C$ ($Z = R + j\cdot X$).
</indepth>

[question:AA101]

<tip>
A resistance of $\qty{100}{\ohm}$ and a reactance of $\qty{100}{\ohm}$ in series give an impedance of $\qty{141}{\ohm}$.
The result comes from adding the two resistances geometrically, using a right-angled triangle and Pythagoras' theorem $a^2 + b^2 = c^2$.
For the resistances this means: $R^2 + X_L^2 = Z^2$
$Z = \sqrt{(\qty{100}{\ohm})^2 + (\qty{100}{\ohm})^2} = \qty{141}{\ohm}$
</tip>


---

We have also already met the inductance of an inductor in Class E. In principle, the inductance rises when the number of turns is increased, the length of the coil is shortened, the cross-sectional area of the coil is enlarged and a material that conducts magnetic flux better is used as the core. To increase the inductance without drastically increasing the number of turns, the winding is wound on a ferrite toroidal core. Chokes with a high inductance are used to reduce radio-frequency currents.

<indepth>
[photo:270:a_Pulvereisenringkern:Example of an iron-powder toroidal core]
[photo:271:a_Ferritringkern:Example of a ferrite core]
</indepth>

[question:AC211]

For toroidal inductors, a so-called $A_\text{L}$ value of the core material is given to make it easier to calculate the inductance.
The inductance is then calculated as:
$L = N^2 \cdot A_\text{L}$ (see the formula sheet – keyword: inductance of a toroidal coil (*Induktivität einer Ringkernspule*)). Now try to answer the following questions with it. 

<attention>
The $A_\text{L}$ value is given in nanohenries per turn squared.
</attention>


[question:AC205]
[question:AC206]
[question:AC207]
[question:AC208]

<indepth>
If there is a material inside the coil that conducts magnetic flux well (e.g. iron, ferrite), the magnetic field is strengthened. The resulting magnetic flux density $B$ can be calculated with the formula (see the formula sheet – keyword: magnetic flux density (*Magnetische Flussdichte*))
$B = \mu_0 \cdot \mu_r \cdot H$
Here $\mu_0$ is the magnetic constant, $\qty{1.2566e-6}{\volt\second\per\ampere\meter}$, and $\mu_r$ stands for the relative permeability of the core material in the coil. For air the factor $1$ is used (see the formula sheet – keywords: magnetic constant; relative permeability (*Magnetische Feldkonstante; relative Permeabilität*)).
</indepth>

To screen a magnetic field, a material that conducts magnetic flux well is needed, for example tinplate. Figure [ref:a_abschirmbecher] shows an example of inductors with screening cans. The metal screening cans contain inductors with an adjustable ferrite core, which is screwed in or out from above through the opening with a screwdriver. This changes the inductance of the inductor.

[question:AC210]

<margin>
[photo:333:a_abschirmbecher:Example of inductors with screening cans for screening magnetic fields]
</margin>
