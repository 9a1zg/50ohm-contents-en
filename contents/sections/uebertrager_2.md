In Class E we have already met the basics of the transformer. It consists of two coils that are magnetically coupled through an iron or ferrite core. To tell the two sides apart, we speak of the primary side, with the number of turns $N_P$, and the secondary side, with the number of turns $N_S$.

The transformer principle is based on a fundamental physical effect: electromagnetic induction. If the magnetic field in one coil changes – as it does when an AC voltage is applied – a voltage is induced in a neighbouring, magnetically coupled coil. According to the law of induction, this voltage is directed so that it opposes the cause that produced it. This is therefore also called *mutual induction*.

[question:AC301]

In Class E we have already met the formula for the transformation ratio $ü$:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S}$

For the currents, the reverse applies accordingly:

$ü = \frac{N_P}{N_S} = \frac{I_S}{I_P} = \frac{U_P}{U_S}$

With this formula, which can also be found on the formula sheet, the next question can be solved:

[question:AC302]

---

Since current-carrying wires must not get excessively hot, to avoid damage to the insulation or even the conductor glowing, a certain maximum current, depending on the cross-sectional area of the conductor, must not be exceeded. If the current is related to the cross-sectional area of the conductor in $\unit{\milli\meter\squared}$, we get the so-called current density $S$. For transformers, the relevant standards specify that a maximum current density of about $\qty{2.5}{\ampere\per\milli\meter\squared}$ should not be exceeded.

The formula is (see the formula sheet – keyword: current rating of windings (*Belastbarkeit von Wicklungen*)):

$I = S \cdot A_\mathrm{Dr}$

<unit>
Current density $S = \frac{I}{A} $ in  $\unit{\ampere\per\milli\meter\squared}$
</unit>

<indepth>
According to the VDE, the maximum permitted current for copper conductors installed in free air is set at $\qty{12}{\ampere}$ for a cross-sectional area of $\qty{0.75}{\milli\meter\squared}$. In fuses, the current density can reach as much as $\qty{3000}{\ampere\per\milli\meter\squared}$.
</indepth>

Now try to answer the following question. For it you need the formula for the cross-sectional area of a conductor and the formula for the current rating of windings. Make sure that the units are converted correctly.

[question:AC307]

---

One of the most important applications of transformers in radio-frequency engineering is **impedance matching**. Here transformers are used as so-called matching transformers.

Unlike mains transformers, the core of such transformers is usually not made of solid iron but of pressed iron powder or ferrite. These materials are better suited to high frequencies and reduce losses.

<indepth>
*Matching* means that the impedance of a source (e.g. a transmitter) is made to match the impedance of the load (e.g. an antenna) as closely as possible. Only with good matching can the power be transferred optimally, without part of the energy being reflected.
</indepth>

A matching transformer therefore has the job of converting a given impedance into another, so that source and load suit each other as well as possible.

---

On the formula sheet we find the formula for the transformation ratio $ü$:

$ü = \sqrt{\frac{Z_p}{Z_s}} = \frac{N_p}{N_s} = \frac{U_p}{U_s}$

Squaring both sides of the equation gives: 


$ü^2 = \frac {Z_p}{Z_s} = \left(\frac{N_p}{N_s}\right)^2 = \left(\frac{U_p}{U_s}\right)^2$

This shows that the impedance ratio is the square of the voltage ratio and so also the square of the turns ratio. Or, put the other way round, a given turns ratio leads to an impedance ratio that is its square.

<indepth>
Derivation of the formula for impedance transformation:
$ P_p = P_s$
$U_p \cdot I_p = U_s \cdot I_s$
Substitute Ohm's law for $U$: $U = I \cdot R$;
$R$ is replaced by $Z$
$(I_p \cdot Z_p) \cdot I_p = (I_s \cdot Z_s) \cdot I_s$
Form the impedance ratio on one side:
$ \frac{Z_p}{Z_s} = \frac{{I_s}^2}{{I_p}^2} = ü^2$
Alternatively, substitute Ohm's law for $I$:
$I = \frac{U}{R}$
$R$ is replaced by $Z$
$\frac{U_p}{Z_p} \cdot U_p  = \frac{U_s}{Z_s} \cdot U_s$
Form the impedance ratio on one side:
$ \frac{Z_p}{Z_s} = \frac{{U_p}^2}{{U_s}^2} = ü^2$
</indepth>

---

As an example, let us consider an end-fed antenna, which we will examine more closely in a later chapter. Its input impedance is about $\qty{2450}{\ohm}$, which is distinctly high. It is to be matched to a transmitter with a load impedance of $\qty{50}{\ohm}$.

<margin>
[picture:260:a_endgespeiste_antenne:End-fed antenna with impedance matching by a transformer]
</margin>

To transform the impedance from $\qty{50}{\ohm}$ to $\qty{2450}{\ohm}$, the ratio is $Z_p:Z_s = \qty{50}{\ohm}:\qty{2450}{\ohm} = 1:49$. This means $ü^2 = 1:49$ and so $ü=\sqrt{1}:\sqrt{49}=1:7$. This means that the primary side may have only one seventh of the turns of the secondary side for the impedance matching to work, e.g. $N_p=1$ and $N_s=7$. In practice, a turns ratio of $2:14$ is usually used (see Figure [ref:a_unun]).

<margin>
[photo:332:a_unun:Example of an unun transformer with a turns ratio of 2 to 14, with the primary and secondary wound together bifilar (twisted)]
</margin>

The following question corresponds essentially to the example above. Here an input impedance of about $\qty{2.5}{\kilo\ohm}$ is given for an end-fed dipole. In practice, however, this value varies with the surroundings and the construction, typically in the range of about $\qty{2}{\kilo\ohm}$ to $\qty{3}{\kilo\ohm}$. 
With a turns ratio of about $1:7$, a sufficiently good match to $\qty{50}{\ohm}$ can nevertheless usually be achieved.

[question:AC306]

Now try to solve the following questions on your own with what you know.

[question:AC305]
[question:AC303]
[question:AC304]
