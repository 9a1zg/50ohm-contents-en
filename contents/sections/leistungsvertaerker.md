In the chapter on basic circuits we have already met various transistor amplifiers. In the transmitter we now look in particular at *power amplifiers*. They amplify the RF signal generated in the preceding stages to the desired output power of the transmitter.

RF power amplifiers can basically be divided into two designs:

1. *Broadband RF amplifiers* have as uniform a gain as possible over a relatively wide frequency range, for example over large parts of the HF range of $\qtyrange{1}{30}{\mega\hertz}$, see Figure [ref:a_breitbandverstärker].
2. *Selective RF amplifiers*, on the other hand, are tuned to a comparatively narrow frequency range, for example to a single amateur band, see Figure [ref:a_selektiver_verstaerker].

Broadband RF amplifiers can often be recognised by broadband coupling transformers between the individual amplifier stages. Together with capacitors, these do not form resonant circuits tuned to a particular frequency. The principle of the push-pull amplifier, which we already know, is also found again in many RF power amplifiers.

<margin>
[picture:491:a_breitbandverstärker:Broadband RF power amplifier with push-pull circuit]
</margin>

[question:AF412]

Selective RF amplifiers, by contrast, can typically be recognised by their frequency-selective design, characterised by series or parallel tuned circuits in the RF signal path.

<margin>
[picture:778:a_selektiver_verstaerker:Selective RF power amplifier with frequency-selective design]
</margin>

[question:AF408]

---

Amplifiers of the types mentioned above can also be built with several stages, by chaining individual stages together.

[question:AF413]

Impedance matching is necessary between the amplifier stages of a power amplifier and at their inputs and outputs. This is needed so that the RF output impedance of one stage is matched as well as possible to the RF input impedance of the following stage, for maximum gain, minimum distortion and optimum efficiency (avoiding reflections and non-linearities). 

Impedance matching can be done either over a broad band, by using a transformer with a suitable transformation ratio, or frequency-selectively, with a tapped tuned circuit.

For frequency-selective matching there are two basic ways of doing this:
- with an inductive potential divider (a tapped inductor with a parallel capacitor)
- with a capacitive potential divider (two capacitors in series, with an inductor in parallel)

These inductors and capacitors can be arranged in different configurations (parallel or series circuit) to achieve the desired impedance transformation and, where required, to suppress harmonics at the same time (pi filter).

[question:AF409]
[question:AF410]
[question:AF414]
[question:AF407]
[question:AF406]

---

Figure [ref:a_fet_verstaerker] shows an HF amplifier with LDMOS field-effect transistors. LDMOS stands for *laterally diffused metal-oxide-semiconductor* and denotes a special field-effect transistor for RF power amplifiers. The actual amplifier circuit (upper part) is very simple. It is again a push-pull amplifier, with two FETs working in push-pull configuration. The two transistors are driven through a common input transformer. The output of the amplifier is taken from a further transformer. The lower part of the circuit is also less complex than you might think: by and large, all it does is produce the bias voltage for the transistors by means of a potential divider.

Do not be misled by the well-known property of a field-effect transistor: with DC the gate draws practically no current and therefore has a very high input impedance. At high frequencies, however, the parasitic capacitances of the transistor play an important part, in particular the capacitances between gate and source and between gate and drain. Their capacitive reactance decreases with increasing frequency, so that an RF current can flow at the gate. With RF power transistors the input impedance can therefore be considerably lower than you would expect from looking at a FET for DC. The input transformer $T_1$ therefore serves to match the $\qty{50}{\ohm}$ to the low input impedance of the transistors.

<margin>
[picture:786:a_fet_verstaerker:HF amplifier with field-effect transistors]
</margin>

[question:AF417]

---

As indicated above, the active devices in a power amplifier need not only the necessary supply voltage but also a DC setting of the operating point (bias). This operating point is usually set by potential dividers, which produce the desired bias voltage at the devices from a stabilised auxiliary voltage, with preset potentiometers for optimum adjustment.

<tip>
When looking at the bias voltage and its effect on the components of the circuit, the circuit need only be considered as far as DC is concerned. Capacitors, as components that can only pass AC voltages, are ignored. Windings of transformers and inductors are treated as short circuits when the circuit is considered for DC. Basically, for these questions it is enough to apply the basic knowledge of Ohm's law and potential dividers from Classes N and E!
</tip>

[question:AF420]

---

The bias voltage for the given circuit in the next question is calculated by applying Ohm's law, taking into account the parallel and series connection of resistors. What matters in this question is that the gate terminals of the transistors are capacitances and can therefore be neglected when the circuit is considered for DC.

[question:AF421]

<indepth>
The resistor $R_5=\qty{51}{\ohm}$ has practically no effect on the DC voltage at the gate, since almost no direct current flows into the gate of the LDMOS transistor. For the RF signal, however, $R_5$ is important: together with the gate capacitance it damps possible radio-frequency oscillations and so improves the stability of the amplifier.

The resistor $R_4=\qty{6.8}{\kilo\ohm}$ ensures that the gate has a defined potential with respect to chassis even if the bias circuit is interrupted. It also discharges the gate capacitance and so prevents the transistor from conducting unintentionally because of a floating gate, e.g. if the potentiometer $R_3$ is faulty. Since $R_4$ is in parallel with the lower arm of the potential divider, it must be taken into account when the gate voltage is calculated exactly.
</indepth>

---

The circuit in Figure [ref:a_fet_verstaerker_vhf] shows a VHF power amplifier with field-effect transistors. Here too the two transistors work as a push-pull output stage, which is the simple part of the circuit. The short coaxial lines, as part of the matching network, serve to transform the low impedance of the LDMOS transistors to an impedance suitable for the rest of the circuit. The rest of the circuit is again the generation of the bias voltage for the transistors, including temperature compensation. The potentiometers $R_1$ and $R_2$ each form a potential divider that sets the bias voltage for its transistor.

[question:AF424]
[question:AF423]

<margin>
[picture:783:a_fet_verstaerker_vhf:VHF amplifier with field-effect transistors]
</margin>


---

A pi filter (see Figure [ref:a_pi_filter]) can match the impedances at its input and output through the ratio of its two capacitances. The inductor of the pi filter, together with the two capacitances, determines the design frequency of the filter. At the same time, because of its low-pass characteristic, the pi filter suppresses unwanted harmonics of the transmitted signal.

<margin>
[picture:1100:a_pi_filter:Pi filter]
</margin>

[question:AF405]

An LC circuit after an RF power amplifier has a similar function. It too is used for impedance matching and, at the same time, for suppressing harmonics.

[question:AF404]

In power amplifiers it is important to decouple the individual stages from the supply voltage as well as possible as far as RF is concerned, to avoid effects on other stages (tendency to oscillate, modulation effects, etc.). For this purpose, the supply lines of the individual stages are decoupled from one another with series inductors and with decoupling capacitors to chassis. This arrangement is a low-pass filter, since ideally only the wanted DC supply voltage is let through, while RF components are blocked.

[question:AF411]
[question:AF419]
[question:AF418]
[question:AF422]

The RF properties of real capacitors depend on frequency. Large capacitances such as electrolytic capacitors can only be used at low frequencies and are of limited effect in the RF range. To block higher frequencies with capacitors as well, a combination of different types of capacitor and capacitance values is often used, which together can block a wider frequency range.

[question:AF415]