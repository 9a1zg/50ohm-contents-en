An old radio operators' saying has it that the best RF amplifier is the antenna. In the first years of radio it was the only "amplifier": there were no amplifying electronics. Then, in 1907, came the thermionic valve – a very successful component, but rather large and not very efficient. From the twenties onwards, scientists dreamt of components with a similar function in which everything happens inside a solid (a semiconductor) rather than in a vacuum. The first component with which this was achieved in practice was the *bipolar transistor*, in 1947/1948, which is also by far the main subject of the questions in the Class E examination.

[question:EC602]

<indepth>
The *bipolar transistor* is also called a BJT, short for bipolar junction transistor.
</indepth>

The ideal function of all types of transistor, and of the valve too, is that of a *voltage-controlled current source*: the smallest possible change in voltage at the input is to produce the largest possible change in current at the output.

The bipolar transistor has three terminals, called the emitter, base and collector. The emitter emits charge carriers into the base – in the NPN bipolar transistor these are *electrons*, in the PNP bipolar transistor electron vacancies, also called *holes*. We will not discuss the physics behind these terms until the Class A course. These charge carriers cross the base and are collected again by the collector. 

---

Figure [ref:e_npn_pnp_symbol] shows the circuit symbols of NPN and PNP transistors. We recognise the emitter electrode by an arrow, which points towards the base in the PNP transistor and away from the base in the NPN transistor. 

<margin>
[picture:864:e_npn_pnp_symbol:Symbols of NPN and PNP transistors]
</margin>

[question:EC605]
[question:EC606]
[question:EC607]
[question:EC608]
[question:EC609]

---

Bipolar transistors are made up of two diodes – the emitter-base diode and the base-collector diode.
In active operation, the emitter-base diode is always forward-biased. In the NPN transistor the potential at the base must be more positive than that of the emitter, in the PNP transistor more negative. The base-collector diode is reverse-biased. To achieve this, the collector potential is chosen more positive than the base in the NPN transistor, and more negative in the PNP transistor.

<tip>
However, the transistor only works if the base zone between emitter and collector is no more than a few micrometres wide. So we cannot make a transistor by soldering two separate diodes together.
</tip>

The minimum voltage at the emitter-base junction depends on the semiconductor used. In a silicon NPN transistor the base must be about $\qty{0.6}{\volt}$ more positive than the emitter, in a silicon PNP transistor about $\qty{0.6}{\volt}$ more negative. This voltage is called the base-emitter voltage $U_\mathrm{BE}$.

[question:EC610]
[question:EC612]
[question:EC613]
[question:EC614]
[question:EC615]

---

<margin>
[picture:863:e_npn_i_u:Currents and voltages in an NPN transistor]
</margin>

---

The currents and voltages in an NPN transistor are shown in Figure [ref:e_npn_i_u]. We already know the base-emitter voltage $U_\mathrm{BE}$. There are also the collector-base voltage $U_\mathrm{CB}$ and the collector-emitter voltage $U_\mathrm{CE}$. The collector current $I_\mathrm{C}$ depends exponentially on the base-emitter voltage:

$I_\mathrm{C} = I_\mathrm{S}\ e^{\frac{U_\mathrm{BE}}{U_\mathrm{T}}}$

At room temperature, $U_\mathrm{T}$ is about $\qty{26}{\milli\volt}$.

<indepth>
$I_\mathrm{S}$ is the so-called reverse saturation current of a bipolar transistor. It is a characteristic parameter of the component and is closely related to the emitter-base diode. It is a very small leakage current that flows through the transistor even when the base-emitter path is not conducting.
</indepth>

Over wide operating ranges, the base current $I_\mathrm{B}$ has the same voltage dependence as the collector current, so that the ratio of collector current to base current is constant:

$\frac{I_\mathrm{C}}{I_\mathrm{B}} = B$

*$B$* is the current gain (strictly speaking, the current gain in the common-emitter circuit). It is often more practical to think of the transistor as a current-controlled component, even though physically it is not. In practical transistors the current gain is $50 \dots 350$.

<tip>
There is an age-old analogy for the current control of the bipolar transistor, involving a large and a small water channel, a weir in the large channel and a control flap. Older readers may still remember it from the "Kleiner Radiomann" (little radio man) kit published by Kosmos ...
  
[picture:835:e_transistor_wehr_geschlossen:Control channel closes the weir completely]
  
At first, no water flows in the small channel. The weir in the large channel is closed, so no water flows there either.
  
[picture:837:e_transistor_wehr_halb_offen:Control channel opens the weir halfway]

Then water starts to flow in the small channel, the control channel. The water lifts the flap, which in turn operates the weir – water starts to flow in the main channel too.
  
[picture:836:e_transistor_wehr_geoeffnet:Control channel opens the weir completely]

Now more water flows in the control channel, the flap is lifted further, and the weir in the main channel opens completely.
</tip>

[question:EC603]

The emitter current $I_E$ is the sum of the collector current and the base current:

$I_\mathrm{E} = I_\mathrm{C} + I_\mathrm{B}$

[question:EC611]

The voltage at a transistor's operating point is usually given as the collector-emitter voltage:

$U_\mathrm{CE} = U_\mathrm{CB} + U_\mathrm{BE}$

Besides the bipolar transistors that we mainly cover here, there are above all *field-effect transistors*, which work differently physically but from the outside have the same basic function (voltage-controlled current source). In the form of MOSFETs they dominate our electronics, as the integrated circuits of digital electronics contain millions to billions of them.

<indepth>
MOSFET stands for *metal-oxide-semiconductor field-effect transistor*.
</indepth>

[question:EC604]

Transistors can be used not only as amplifiers, but also as (current) switches (current on/off) or, at low voltages at the output, as controllable resistors. The last function is implemented mainly with field-effect transistors.

[question:EC601]
