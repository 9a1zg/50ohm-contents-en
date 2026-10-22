We already discussed the bipolar transistor in the Class E course material. In Class A we will go into the topic in more depth and also look at another type of transistor.

The bipolar transistor consists of three semiconductor zones that are alternately n- and p-doped. The zones are called the emitter, base and collector. In the *npn transistor* the emitter is n-doped, the base p-doped and the collector n-doped. The pnp transistor accordingly has a p-emitter, an n-base and a p-collector. 

Figure [ref:a_bipolartransistor_aus] shows an npn transistor in the off state.
As soon as the base-emitter voltage $U_\mathrm{BE}$ is applied by closing the switch (typically $\approx \qtyrange{0.6}{0.7}{\volt}$ for silicon), the base-emitter diode starts to conduct. As a result, a small base current $I_\mathrm{B}$ flows (see Figure [ref:a_bipolartransistor_ein]).

This small base current causes many electrons to be injected from the emitter into the thin base. Since the base is very narrow, most of these charge carriers carry on to the collector. There they are "sucked away" by the applied collector-emitter voltage $U_\mathrm{CE}$, and the collector current $I_\mathrm{C}$ flows. It is larger than the base current by the factor $B$, where $B$ is the so-called current gain of the transistor. Typical values of $B$ are in the range $\num{20}$ to $\num{500}$.

<margin>
[picture:1071:a_bipolartransistor_aus:NPN bipolar transistor in the off state]
[picture:1072:a_bipolartransistor_ein:NPN bipolar transistor in the on state]
</margin>

[question:AC503]

It is a good idea to memorise the NPN transistor, for example. For PNP everything is then the other way round.

[question:AC504]

Physically, the base-emitter voltage $U_{BE}$ controls the collector current $I_C$, and it does so exponentially. For the npn transistor, for example:

$I_C = I_S \cdot e^{\frac{U_{BE}}{U_T}}$

$I_S$ is the saturation current, which depends strongly on the type of transistor. It can be found in the data sheet. $U_T$ is the so-called thermal voltage, which is about $\qty{26}{\milli\volt}$ at room temperature.

One difference from the field-effect transistor, which we look at later, is that in the bipolar transistor a current always flows at the input (the base) as well: the base current $I_B$. It too depends exponentially on $U_{BE}$, with $I_S$ smaller by a factor of $B$ than for the collector current.

$I_B = \frac{I_S}{B} \cdot e^{\frac{U_{BE}}{U_T}}$

So the factor $B$ is the quotient of collector current and base current:

$B = \frac{I_C}{I_B}$

Even though the bipolar transistor is physically controlled by $U_\mathrm{BE}$, it is described as *current-controlled*, because it only conducts when a base current flows.

[question:AC501]

A transistor is described as "conducting" in the "forward direction" when a significant collector current flows. For this, the base-emitter diode must always be forward-biased, i.e. $U_{BE}$ positive for npn and negative for pnp transistors. The collector-base diode, on the other hand, must block, because no charge carriers are to be injected from the collector into the base.

[question:AC505]

In what follows, we look at a few simple transistor circuits based on the bipolar transistor.

---

[question:AC515]

The desired operating point is set by feeding a base current in through $R_1$. The base current is smaller than the collector current by the given current gain of $\num{298}$. The difference between the operating voltage and the base potential is dropped across the resistor. The base potential is given as $\qty{0.6}{\volt}$. So we calculate:

$R_1 = 298 \cdot \frac{\qty{12}{\volt} - \qty{0.6}{\volt}}{\qty{0.005}{\ampere}} \approx \qty{680}{\kilo\ohm}$

<indepth>
In practice, however, the circuit has a huge disadvantage: the current gain of a bipolar transistor is not particularly well controlled. Take the popular BC547B as an example. According to its specification, its current gain can lie anywhere between $\num{200}$ and $\num{450}$. With this circuit, the collector current can therefore easily differ from the design value by more than a factor of $2$.
</indepth>

To make the operating point more stable, the operating point of the bipolar transistor is usually set with a potential divider. The so-called divider current is the current that flows through $R_2$ here. It should be at least ten times the base current, so that the base current has little influence on the operating point. 

---

[question:AC516]

<indepth>
From a practical point of view, this circuit is not very advisable either. For one thing, the collector current depends exponentially on the base-emitter voltage. The resistors have a tolerance, so the base potential may well differ somewhat from the intended value – with a large effect on the collector current. In addition, the threshold voltage of the base-emitter diode depends quite strongly on temperature, at about $\qty{-2}{\milli\volt\per\kelvin}$. So the collector current in this circuit will vary strongly with temperature. That can sometimes be desirable, but it has to be kept in mind. We will meet a circuit that contains negative feedback, which stabilises the operating point.
</indepth>

There is a calculation question on this circuit too:

[question:AC518]

The potential divider $R_1$ and $R_2$ sets the base potential, which must be about $\qty{0.6}{\volt}$ because the emitter is connected to chassis. With a collector current of $\qty{2}{\milli\ampere}$ and a current gain of $\num{200}$, the base current is $\qty{2}{\milli\ampere} / 200 = \qty{10}{\micro\ampere}$. The current through $R_2$ is to be ten times the base current, so $11 \cdot \qty{10}{\micro\ampere} = \qty{110}{\micro\ampere}$ flows through $R_1$. The resistor $R_1$ is then:

$R_1 = \frac{\qty{10}{\volt} - \qty{0.6}{\volt}}{\qty{110}{\micro\ampere}} = \qty{85.5}{\kilo\ohm}$

The next circuit shows a typical way of setting the operating point of the bipolar transistor, as also used in practice.

---

[question:AC517]

<indepth>
This is a good circuit, which is often used in practice too, because the collector current is determined mainly by the emitter resistor $R_E$, which provides series negative feedback:

If the collector current $I_C$ rises, the emitter current $I_E$ rises too. As a result, a larger voltage is dropped across the emitter resistor $R_E$. So the emitter becomes more positive. Since the base voltage stays almost constant because of the potential divider formed by $R_1$ and $R_2$, the base-emitter voltage $ U_{BE} = U_B - U_E $ becomes smaller.

A smaller base-emitter voltage means that the transistor conducts less. This reduces the current that had originally risen.

So the circuit automatically counteracts changes in the current. That is why it is called negative feedback. If the current rises, the transistor is "turned down" a little. If the current falls, the transistor conducts more again. This stabilises the operating point of the circuit.
</indepth>

The base potential is set by the potential divider $R_1$ and $R_2$. Since $\qty{1}{\volt}$ is to be dropped across the emitter resistor $R_E$, the base potential must be $\qty{1.6}{\volt}$. With a collector current of $\qty{2}{\milli\ampere}$ and a current gain of $\num{200}$, the base current is $\qty{10}{\micro\ampere}$. Since ten times the base current is to flow through $R_2$, eleven times the base current flows through $R_1$, i.e. $\qty{110}{\micro\ampere}$. The difference between the operating voltage ($\qty{10}{\volt}$) and the base potential is dropped across $R_1$, i.e. $\qty{8.4}{\volt}$. Now we can determine $R_1$:

$R_1 = \frac{\qty{8.4}{\volt}}{\qty{110}{\micro\ampere}} = \qty{76.4}{\kilo\ohm}$

[question:AC519]

If, because of the fault, no current flows through $R_1$, no voltage is dropped across $R_2$ – the base is at chassis potential. Then the condition $U_{BE} \geq \qty{0.6}{\volt}$ is not met, and no current flows through the transistor. Since no voltage is dropped across the collector resistor $R_C$, the collector potential rises to the operating voltage.

[question:AC520]

With the fault given here, no current flows through $R_2$. The base is connected to the operating voltage through $R_1$. A base current is injected along this path. With the usual choice of values (divider current ten times the normal base current), the base current is 11 times the normal base current – the collector current will rise very sharply, the voltage drop across $R_C$ rises sharply, and the collector-emitter voltage falls to the saturation value of about $\qty{0.1}{\volt}$. The collector current is limited only by $R_C$.

---

The next question is about a relay that is switched by the npn transistor shown in series with it (see Figure [ref:a_relais_schaltung]). Let us assume that the transistor is switched on at first: a current flows through the relay coil, and the relay has pulled in.

<margin>
[picture:426:a_relais_schaltung:Relay circuit with npn transistor and freewheeling diode]
</margin>

Now the transistor switches off and the current flow collapses. However, the sharp change in current briefly induces a high negative voltage in the relay coil, which can destroy the transistor.

To prevent this, we connect a freewheeling diode *in parallel*. It is connected so that it carries no current in normal operation (transistor switched on) – so it must be fitted in the reverse direction. The negative voltage that briefly appears when the current collapses forward-biases the diode, and the resulting voltage is limited (with silicon diodes) to $\qty{-0.7}{\volt} \ldots \qty{-0.8}{\volt}$.

[question:AC524]

---

Field-effect transistors work on a completely different control principle from bipolar transistors. Whereas in bipolar transistors both electrons and electron vacancies ("holes") have to be considered (hence "bipolar"), only one kind of charge carrier is involved in the field-effect transistor ("unipolar"). These can be either electrons (*n-channel field-effect transistor*) or holes (*p-channel field-effect transistor*).

The electrodes of the FET, which are shown in Figure [ref:a_fet_schnitt_aus], are named as follows:

* *Source*: this is the "source" of the charge carriers in the channel. Do not be confused: so-called conventional current flow is defined as opposite to the direction in which the charge carriers flow!
* *Drain*: this is where the charge carriers in the channel flow away ("drain").
* *Gate*: the gate controls the flow of charge carriers in the channel.

[question:AC512]

What all field-effect transistors (or *FETs*) have in common is that in normal operation no current flows at the input, the gate electrode. The control of the charge in the channel (the region between *source* and *drain*) depends solely on the gate-source voltage.

<margin>
[picture:1073:a_fet_schnitt_aus:FET in cross-section, not conducting]
[picture:1074:a_fet_schnitt_ein:FET in cross-section, conducting]
</margin>

Figures [ref:a_fet_schnitt_aus] and [ref:a_fet_schnitt_ein] show the cross-section of an n-channel MOSFET in the off state and in the conducting state. In the upper picture, no sufficient gate-source voltage $U_{GS}$ is applied. Between the n-doped regions of the source and drain lies the p-doped substrate, so there is no conducting channel. The transistor is off, and no current can flow between source and drain.

If a voltage that is positive with respect to the source is applied to the gate (see Figure [ref:a_fet_schnitt_ein]), an electric field is set up through the insulating SiO$_2$ layer. This field attracts electrons to the surface of the p-doped substrate directly below the gate. As a result, a conducting n-channel forms there, connecting the source and drain. The MOSFET starts to conduct, and a current can flow between drain and source.

The important point is that the gate is electrically insulated by the oxide layer. Ideally, therefore, no gate current flows; the MOSFET is controlled not by a control current but by the electric field at the gate. That is why it is also described as a *voltage-controlled* component.

[question:AC502]

[question:AC513]

[question:AC514]

As we have already established, the FET is a *voltage-controlled* component in which no gate current flows. The answer wanted is that the gate-source voltage controls the *resistance of the channel*. However, the behaviour of the channel can only be described as a resistance for very small drain-source voltages, so the answer is somewhat unfortunately worded. It would be better to say: the gate-source voltage controls the channel current.

---

The vertical line represents the channel, which is contacted at the top (drain) and at the bottom (source). The gate can be seen on the left – the arrow together with the vertical bar is reminiscent of a diode. So this is a FET, strictly speaking a junction FET. Figure [ref:a_fet_overview] gives an overview of the different types of FET with their circuit symbols.

<margin>
[picture:1075:a_fet_overview:Overview of FETs with their symbols]
</margin>

[question:AC506]

The following questions are about matching certain types of FET to their circuit symbols. A few basic rules:

* The current in the channel can be carried either by electrons or by holes. In the first case we speak of an *n-channel FET*, in the second of a *p-channel FET*.
* We can also distinguish FETs by whether or not a current flows in the channel when the gate-source voltage $U_{GS}=0$. They are then called either *depletion-mode* or *enhancement-mode*. 
* Finally, we can distinguish FETs by whether the gate electrode is a diode or a capacitor structure. If the gate is a diode, we speak of a junction FET. Examples are the JFET (junction field-effect transistor) and the MESFET (metal-semiconductor field-effect transistor). In the MESFET the gate diode is a Schottky diode. In an *insulated-gate FET* the gate electrode is separated from the channel by an insulator (a dielectric). The applied voltage controls the density of charge carriers in the channel. If the insulator is an oxide, for example silicon dioxide, we also speak of a MOSFET (metal-oxide-semiconductor FET). Because of their use in digital circuits, MOSFETs are by far the most common type of transistor.

The arrow shows whether it is an n-channel or a p-channel FET. As with the diode, the arrow points to the cathode, i.e. the n-doped region. So if the arrow points to the channel, it is an n-channel FET. In the junction FET the gate carries the channel; in the insulated-gate FET the arrow is seen between the channel and the so-called bulk layer, which lies under the channel and is usually connected internally to the source electrode.

In the insulated-gate FET, the gate and the channel also form a capacitor in the drawing.

In the depletion-mode FET the line between source and drain is continuous, whereas in the enhancement-mode FET it is broken.

[question:AC507]
[question:AC508]
[question:AC509]
[question:AC510]
[question:AC511]

In what follows we will also look at a few MOSFET circuits that build on the previous questions.

[question:AC521]

No direct current flows into the gate terminal of a MOSFET. So this is an *unloaded* potential divider, and:

$U_{GS} = \frac{R_2}{R_1 + R_2} \cdot U_B = \frac{\qty{1}{\kilo\ohm}}{\qty{11}{\kilo\ohm}} \cdot \qty{44}{\volt} = \qty{4}{\volt}$

[question:AC522]

Here too we have an unloaded potential divider. Since the voltages are given, the simplest approach is:

$\frac{R_2}{R_1} = \frac{\qty{2.8}{\volt}}{\qty{44}{\volt} - \qty{2.8}{\volt}} \rightarrow R_2 = 0.068 \cdot \qty{10}{\kilo\ohm} = \qty{680}{\ohm}$

[question:AC523]

The power MOSFET here is fully switched on, and the channel can be represented as an ohmic resistance of $R_\mathrm{DSon} = \qty{4}{\milli\ohm}$ (as stated in the question). A current of $\qty{25}{\ampere}$ flows. We simply calculate the power dissipation with the familiar power formula:

$P_V = I^2 \cdot R_{\mathrm{DSon}} = \qty{2.5}{\watt}$