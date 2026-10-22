In Class E we have already met the SWR meter and how it is used. In Class A we want to understand how an SWR meter works inside. An SWR meter usually consists of two directional couplers. First, let us become familiar with how they work. 

A *directional coupler* serves to couple a small part of an RF signal out of a feeder. Its special feature is that it can tell in which direction the wave is travelling on the line. To do this, the signal is picked up in two different ways. Capacitive coupling gives a voltage $U_C$ that depends on the voltage on the feeder. At the same time, inductive coupling produces a voltage $U_I$ that depends on the current on the feeder. The directional coupler is dimensioned so that the capacitively and inductively derived signal components at its outputs are equal in size. At the two outputs, however, these components are combined with opposite signs.

For a wave travelling in a particular direction on the line, e.g. from left to right as shown in Figure [ref:a_richtkoppler_rechts_links], the capacitively and inductively derived voltages add at one output. At the other output they are in opposition and, ideally, cancel each other out. The signal therefore appears mainly at only one of the two outputs.

<margin>
[picture:1109:a_richtkoppler_rechts_links:Directional coupler, the wave travelling from left to right]
</margin>

---

If the direction of travel of the wave is reversed, e.g. from right to left as shown in Figure [ref:a_richtkoppler_rechts_links], the direction of the current relative to the voltage is also reversed. As a result, the inductively coupled voltage $U_I$ changes its sign, while the capacitively coupled voltage $U_C$ follows the line voltage.

<margin>
[picture:1110:a_richtkoppler_rechts_links:Directional coupler, the wave travelling from right to left]
</margin>

The two outputs of the directional coupler are thus also swapped: the output at which the two components added before is now largely cancelled, while they add at the other output.

In this way a directional coupler can distinguish between a *forward wave* towards the antenna and a *reflected wave* towards the transmitter.

---

This property of directional couplers is used in an *SWR meter*: for this, the output voltages of two directional couplers inserted in the line and operated in opposite directions are measured. The RF voltages at the outputs of the directional couplers are rectified with diodes and smoothed. This produces DC voltages that can be shown on a meter.

[question:AI401]

Figure [ref:a_rswr_meter] shows the basic design of an SWR meter with two directional couplers. We assume that the transmitter is on the left and the antenna on the right.

[question:AI402]

The upper conductor is part of the feeder between transmitter and antenna. Two quantities are picked up from it: capacitive coupling takes off a small part of the RF voltage. At the same time, inductive coupling derives a component that depends on the current on the feeder.

The end of the coupling line that is not used for the measurement is terminated with a *terminating resistor*. This resistor corresponds approximately to the characteristic impedance $Z_0$ of the coupling line. As a result, the RF power arriving there is absorbed and not reflected back into the coupling line. Such reflections would impair the separation between the forward and reflected waves.

These two signal components are combined with each other in the directional coupler. For a wave travelling from the transmitter to the antenna they add in one of the two couplers, while in the other they largely cancel each other out. For a wave in the opposite direction it is exactly the other way round.

The two almost mirror-image halves of the circuit can therefore pick up different directions of travel:

* One directional coupler delivers a signal proportional to the *forward wave* from the transmitter to the antenna.
* The other directional coupler delivers a signal proportional to the *reflected wave* from the antenna to the transmitter.

The signals coupled out are at first RF alternating voltages. The diodes rectify these voltages, and the capacitors smooth them. This produces DC voltages that can be shown by the two meter movements of a cross-needle meter, or measured by a microcontroller with an A/D converter. The variable resistors are used to adjust or calibrate the reading. They are not to be confused with the terminating resistors of the coupling lines, which provide a low-reflection termination with $Z_0$.

<margin>
[picture:499:a_rswr_meter:SWR meter with two directional couplers]
</margin>
