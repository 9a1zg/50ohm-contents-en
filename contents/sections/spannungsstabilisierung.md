Every radio contains one or more voltage stabilisers, because the input voltage can fluctuate, above all in battery-powered equipment, and sensitive circuits such as oscillators would then change their frequency.

Voltage stabilisers come in 3 variants:
1. *Zener diode circuit* 
2. *Linear voltage regulators* 
3. *Fixed voltage regulators* in an integrated circuit

The *Zener diode circuit* (see Figure [ref:a_stab_z_diode]) is a very simple circuit for stabilising the output voltage, since the Zener diode can keep the output voltage stable within limits.

The Zener diode is always operated with a series resistor and in the reverse direction ($-U_Z$). Zener diodes with breakdown voltages $U_Z$ from $\qty{5}{\volt}$ upwards have a very steep characteristic (see Figure [ref:a_z_diode_kennlinie]) and are therefore very well suited to voltage stabilisation. The efficiency of the circuit is very low, because the losses in the series resistor $R_V$ and in the Zener diode have to be taken into account. 

<margin>
[picture:323:a_stab_z_diode:Voltage stabilisation with a Zener diode]
[picture:862:a_z_diode_kennlinie:Characteristic of a Zener diode]
</margin>

The solution to the following question takes a little more work. First, the output power is found from the load resistance and the load current. Then the input power drawn is calculated from the supply voltage and the sum of the load current and the Zener diode current. The efficiency is then the ratio of the power delivered to the power drawn.

[question:AD321]

---

*Linear voltage regulators* stabilise the output voltage by operating a power transistor as a variable resistor, which forms a potential divider together with the load resistance.

<margin>
[picture:1079:a_diskrete_pannungsstabilisierung:Voltage stabiliser built from discrete components]
</margin>

The following question shows a discrete voltage stabiliser with a series pass transistor. A Zener diode produces a reference voltage of $\qty{5.6}{\volt}$ at the base of the transistor. When a silicon transistor is operating, the emitter potential is about $\qty{0.6}{\volt}$ lower than the base potential. The regulated output voltage is then about $\qty{5}{\volt}$.

The load current also flows through the transistor, so the transistor gets very warm when the load current is high. In linear regulated voltage stabilisers, these series pass transistors are therefore always mounted on a heatsink. 

<margin>
[photo:246:a_Längstransistor 2N3055 auf Kühlkörper:The series pass transistor in a linear regulated power supply has to withstand a high power dissipation and is therefore mounted on a heatsink.]
</margin>

[question:AD315]

The power dissipation $P_V$ is the difference $P_{\mathrm{in}} - P_{\mathrm{out}}$. Together with the power formula $P = U \cdot I$, the power dissipation can be calculated.

[question:AD319]

The efficiency of linear voltage regulators is, by their very nature, often very low. There is a question on this efficiency, which can be solved with the familiar formula from above, $\eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}}$. 

[question:AD320]

---

Besides the Zener diode and the linear voltage regulator, there are also *fixed voltage regulators* in an integrated circuit. Fixed voltage regulators work like linear voltage regulators with a series pass transistor and contain a very accurate voltage reference together with optimised electronic control. Even if the input voltage fluctuates considerably (e.g. $\qty{\pm 2}{\volt}$), the change in voltage on the load side can only be measured in the millivolt range. The capacitors on both sides of the fixed voltage regulator must be chosen as the manufacturer specifies; otherwise the regulation of the circuit can break into unwanted oscillation.

<margin>
[picture:200:a_Festspannungsregler:Fixed voltage regulator]
</margin>

---

A fixed voltage regulator keeps its output voltage largely constant as long as the input voltage is sufficiently above the output voltage. The output voltage therefore stays almost unchanged, even if the input voltage fluctuates.

[question:AD316]
[question:AD317]

<tip>
For the internal control circuit to work properly, the input voltage of standard fixed voltage regulators (e.g. type 7812 for a fixed voltage of $\qty{12}{\volt}$) must be about $\qty{3}{\volt}$ higher than the output voltage, i.e. at least $\qty{15}{\volt}$. There are fixed voltage regulators whose input voltage need only be $\qty{1}{\volt}$ higher than the output voltage. These regulators are called low-dropout (LDO) regulators.
</tip>

---

To solve the following question we again use the familiar relationship: the power dissipation $P_V$ of the fixed voltage regulator is the difference between $P_{\mathrm{in}}$ and $P_{\mathrm{out}}$.

[question:AD318]

<tip>
The solution starts by calculating the load current: $I_L$. Note: the current in the chassis lead of the fixed voltage regulator is negligibly small and is therefore not taken into account.
</tip>

<margin>
[photo:245:a_Festspannungsregler:Fixed voltage regulators for $\qty{5}{\volt}$, $\qty{12}{\volt}$ and $\qty{9}{\volt}$ on a heatsink]
</margin>
  