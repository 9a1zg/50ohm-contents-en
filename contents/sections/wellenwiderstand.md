A feeder can be represented as a circuit of many small inductances and capacitances, as in Figure [ref:a_wellenwiderstand]. From this inductance per unit length $L'$ in $\unit{\henry\per\meter}$ and capacitance per unit length $C'$ in $\unit{\farad\per\meter}$, the characteristic impedance $Z$ of the line follows. In general:

$Z_0 = \sqrt{\frac{L'}{C'}}.$

<margin>
[picture:1108:a_wellenwiderstand:Characteristic impedance of a feeder]

| X: Property                  | l: Value                              |
| Impedance                    | $\qty{50}{\ohm}$                      |
| Frequency range              | $ < \qty{1}{\giga\hertz}$             |
| Capacitance per unit length  | $\qty{100}{\pico\farad\per\meter}$    |
| Inductance per unit length   | $\qty{0.25}{\micro\henry\per\meter}$  |
| Velocity of propagation      | $\qty{0.66}{\percent}$                |
[table:a_rg58:Technical data from a data sheet of an RG-58 coaxial cable]
</margin>

Table [ref:a_rg58] shows the technical data of an RG-58 coaxial cable. The characteristic impedance is $\qty{50}{\ohm}$, the capacitance per unit length $\qty{100}{\pico\farad\per\meter}$ and the inductance per unit length $\qty{0.25}{\micro\henry\per\meter}$. From these values the characteristic impedance can be calculated with the formula above:

$Z_0 = \sqrt{\frac{\qty{0.25}{\micro\henry\per\meter}}{\qty{100}{\pico\farad\per\meter}}} = \sqrt{2500} = \qty{50}{\ohm}$

If the capacitance and inductance per unit length are not known, the formula sheet has formulas based on the geometric dimensions of the line and the relative permittivity of the dielectric.

The characteristic impedance $Z_0$ of a balanced twin feeder depends, for example, on the centre-to-centre spacing of the conductors ($a$) and their diameter ($d$), and on the relative permittivity $\epsilon_\mathrm{r}$ of the dielectric between them. The equation given on the formula sheet applies for $a/d > 2.5$:

$Z_0 = \dfrac{\qty{120}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{2\cdot a}{d}\right)}$

Here $\ln$ is the natural logarithm.

[question:AG305]

The characteristic impedance $Z_0$ of a coaxial line depends on the ratio of the inside diameter of the outer conductor ($D$) to the diameter of the inner conductor ($d$), and on the dielectric between them. From the formula sheet we take:

$Z_0 = \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{D}{d}\right)}$

Here $\ln$ is the natural logarithm and $\epsilon_\mathrm{r}$ the relative permittivity of the dielectric.

[question:AG306]
[question:AG307]

If a line is terminated in its characteristic impedance, that is, if a component or an antenna whose resistance is exactly the same as the characteristic impedance of the line is connected at one end, the line is said to be matched. In this case, waves are not reflected at this end of the cable.

[question:AG304]
