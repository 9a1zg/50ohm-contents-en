Remotely mounted preamplifiers or receive converters fitted at the antennas need a DC supply. To save running an additional DC supply line, the supply voltage can also be carried over the coaxial cable, alongside the RF signal, without the two signals interfering with each other. A bias tee (remote DC feed) is therefore used to feed the DC voltage into the coaxial cable. Figure [ref:a_qo100_bias_t] shows a QO-100 station with a bias tee for supplying power to the preamplifier (LNB).

<margin>
[picture:1080:a_qo100_bias_t:QO-100 station with a bias tee for supplying power to the LNB]
</margin>

[question:AD322]

Technically, this arrangement can be put into practice with a very simple circuit, as shown in Figure [ref:a_bias_t]. Apart from the connectors, the bias tee consists of only two capacitors and one inductor. We have already met this circuit with the MMIC, whose supply voltage is fed in through the output with a bias tee.

<margin>
[picture:399:a_bias_t:Bias tee (remote DC feed)]
</margin>

[question:AD323]

A bias tee can be recognised by the fact that on one side the RF signal is taken to the receiver (RX), while on the other side a preamplifier or receive converter (LNA) is connected. In addition, a DC supply voltage is fed in through the DC connection. This DC voltage passes through the inductor onto the inner conductor of the coaxial cable and so supplies the connected LNA. The inductor presents a high impedance at RF, so that the RF signal does not leak away into the power supply.

The coupling capacitor $C_1$ prevents the DC voltage fed in from reaching the receiver input. Without the capacitor $C_1$, the supply voltage could therefore be short-circuited to chassis.

[question:AD324]

---

The inductor serves to feed the DC supply voltage into the line, while presenting a high impedance at RF. This allows the DC voltage to reach the LNA without the RF signal leaking away into the power supply. The capacitor $C_2$ shunts any remaining RF components to chassis. This prevents RF signals from coupling into the power supply.

<indepth>
[photo:288:a_Bias T Platine:Bias tee circuit board – designed with KiCad]
This is what a practical circuit board for the circuit diagram shown might look like. $C_2$ and $C_3$ are decoupling capacitors for different frequency ranges, so that the circuit works over a wide frequency range. $L_1$ feeds in the DC voltage and must be dimensioned specifically for the load current. The decoupling capacitor $C_2$ on the DC side is meant to suppress RF voltage. It must be chosen so that at the wanted RF frequency its reactance is less than 1 Ω.
</indepth>

The inductor between the DC side (e.g. $\qty{12}{\volt}$) and the RF side (e.g. a $\qty{10}{\giga\hertz}$ received signal) is meant to stop RF components from getting through to the DC side. It is therefore a choke, which must present a high impedance at the wanted frequency (e.g. $X_L = \qty{10}{\kilo\ohm}$). The supply current for the preamplifier or converter (LNA) flows through this choke. The wire diameter of the choke must be large enough that the DC supply current does not make the choke heat up. In other words: the inductor must have an adequate current rating. 

[question:AD325]