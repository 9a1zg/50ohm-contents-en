In Class E we have already met the *dummy load*. A dummy load is a load resistor that converts the RF power delivered by the transmitter into heat. It makes it possible, for example, to test a transmitter or to determine its output power without a signal being radiated from an antenna. In Class A we now look more closely at how such a dummy load can be built.

A dummy load for radio frequencies is often made up of several individual resistors. This spreads the power dissipated over several components and gives a correspondingly high total power rating. The resistors can be connected in parallel, in series or in a combination of series and parallel connections. If identical resistors with the same power rating are used and the circuit is built symmetrically, the power dissipated is shared equally between the individual resistors. The number of resistors needed and the way they are connected can be worked out with the familiar rules for series and parallel connections. With an RF dummy load it is also important that the circuit behaves as closely as possible like a purely resistive $\qty{50}{\ohm}$, even at high frequencies. For this reason suitable resistors with as little inductance as possible are used, and the connecting leads are kept as short as possible.

Figure [ref:dummy_load_aufbau1] shows a finished dummy load from 50ohm.de. Here, for example, $\num{20}$ resistors of $\qty{1}{\kilo\ohm}$ each are connected in parallel. For $n$ identical resistors in parallel:

$R_\mathrm{ges} = \frac{R}{n}$

This gives:

$R_\mathrm{ges} = \frac{\qty{1}{\kilo\ohm}}{20} = \qty{50}{\ohm}$

<warning>
The maximum possible power dissipation of the whole dummy load is approximately the sum of the power ratings of all the resistors, provided the power is shared equally between them. Since the 50ohm.de dummy load has no cooling and is not screened, it should only be used for QRP transmitters with a low output power. Higher powers call for a dummy load with cooling and screening that is also suitable for continuous operation!
</warning>

The 50ohm.de dummy load also has a peak rectifier made of a diode and a capacitor. With it, the RF voltage present can be turned into a DC voltage that can be measured with a multimeter, for example. Taking into account the potential divider and the forward voltage of the diode, the RF output power of the transmitter can be determined from this.

[question:AI602]

<margin>
[photo:340:dummy_load_aufbau1:The finished 50ohm.de dummy load]
[photo:341:dummy_load_aufbau2:Construction of the 50ohm.de dummy load]

*Advertisement:* Would you like to build a cool 50ohm.de QRP dummy load too? You can order it as a kit from [DARC-Verlag](https://darcverlag.de/50Ohm-Dummy-Load-DIY-Kit-Bausatz).
</margin>

In the following examination question, the dummy load consists of a combination of series and parallel connections. If $N_\mathrm{S}$ identical resistors are connected in series in each branch and $N_\mathrm{P}$ such branches are then connected in parallel, the total resistance is:

$R_\mathrm{ges} = \frac{N_\mathrm{S}}{N_\mathrm{P}} \cdot R$

The total number of resistors used is then:

$n = N_\mathrm{S} \cdot N_\mathrm{P}$

If all the resistors carry the same load, their permitted power dissipations add up. In this way a dummy load can be built with the desired resistance and, at the same time, a high power rating.

[question:AI601]

Another way of determining the RF output power is to give the dummy load a tap on its resistor network. If this tap is, for example, close to the chassis connection, only part of the total RF voltage is present there.

The resistors then form a potential divider. If its divider ratio is known, the total voltage across the dummy load can be calculated back from the RF voltage measured at the tap. The partial voltage can be measured, for example, with an RF probe and a digital multimeter. The RF power can then be calculated from the total voltage found in this way.

[question:AI603]