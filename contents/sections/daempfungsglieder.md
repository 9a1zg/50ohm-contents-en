Attenuators are often needed in RF engineering to reduce signal levels by a defined amount. A power attenuator, for example, can reduce the output power of a transmitter far enough that its output signal does not damage or overload the measuring instruments connected to it. Attenuators are also used to reduce input levels for amplifiers and receivers to a defined level.

An attenuator must always be designed for a defined system impedance at its input and output. In symmetrical attenuators, the input and output impedances are identical. Often this is the $\qty{50}{\ohm}$ usual in RF engineering. For an attenuator to present the required impedances at its input and output, a termination with the correct impedance is needed on both sides. This is achieved by a suitable resistor network. 

There are various circuit variants, which differ in the arrangement of the resistors. The two commonest are the T attenuator (see Figure [ref:a_daempfungsglied_t]) and the $\pi$ attenuator (see Figure [ref:a_daempfungsglied_pi]). In both variants the attenuation is achieved by a resistor network that converts the power fed in into heat.

<margin>
[picture:342:a_daempfungsglied_pi:Attenuator in pi configuration with source and load resistor]
</margin>

<margin>
[picture:341:a_daempfungsglied_t:Attenuator in T configuration with source and load resistor]
</margin>

[question:AD801]
[question:AD802]

---

The attenuation of an attenuator is usually given in dB (decibels) and refers to the power. For example, $\qty{20}{\dB}$ means attenuating the input power by a factor of $\num{100}$. The output power after this attenuator is then only $\frac{1}{100}$ of the input power, which, with an input power of $\qty{100}{\watt}$, corresponds to an output power of $\qty{1}{\watt}$.

In resistive attenuators, the attenuation takes place by converting the power fed in into heat. If, for example, a $\qty{100}{\watt}$ signal is attenuated by $\qty{20}{\dB}$ as described above, $\qty{99}{\watt}$ is converted into heat in the attenuator. The remaining power of $\qty{1}{\watt}$ is then still available at the output of the attenuator.

[question:AD806]
[question:AD803]
[question:AD804]
[question:AD805]

A symmetrical attenuator can be built, for example, as a T or $\pi$ network of resistors. The names come from how the arrangement of the resistors looks in the circuit.

<indepth>
The resistor values for a $\pi$ attenuator for an impedance of $\qty{50}{\ohm}$ can be calculated with the following formulas:

$R_1 = R_3 = \qty{50}{\ohm} \cdot \left( \frac{10^{\frac{a}{20}}+1}{10^{\frac{a}{20}}-1}\right)$

Here $a$ is the required attenuation in $\unit{\dB}$.

$R_2 = \frac{\qty{50}{\ohm}}{2} \cdot \left( 10^{\frac{a}{20}} - \frac{1}{10^{\frac{a}{20}}}\right)$

The resistor values for a T attenuator for an impedance of $\qty{50}{\ohm}$ can be calculated with the following formulas:

$R_1 = R_2 = \qty{50}{\ohm} \cdot \left( \frac{10^{\frac{a}{20}}-1}{10^{\frac{a}{20}}+1} \right)$

$R_3 = 2\cdot \qty{50}{\ohm} \cdot \left( \frac{10^{\frac{a}{20}}}{10^{\frac{a}{10}}-1} \right)$

<webonly>
[include:applet_daempfungsglied]
</webonly>

</indepth>


