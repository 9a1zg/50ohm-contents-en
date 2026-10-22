In the next two chapters we deal with two important basic circuits of a bipolar transistor. In this chapter we first look at the *common-collector circuit*, and in the following chapter at the *common-emitter circuit*. Both circuits are shown in Figure [ref:a_emitter_collector]. They have different properties and are therefore used for different applications.

<margin>
[picture:1118:a_emitter_collector:Common-emitter and common-collector circuits, with the base (B), collector (C) and emitter (E) labelled]
</margin>

The basic circuits of a bipolar transistor are named after the terminal that serves neither as the input nor as the output of the circuit, and so forms the common reference point for the input and output circuits. In the common-collector circuit, this is the collector. 

---

[question:AD401]

<tip>
Bipolar transistor amplifier circuits are named after the terminal to which neither the input nor the output is directly connected (see Figure [ref:a_emitter_collector]). 
</tip>

Since the collector is usually connected to the supply voltage and, for AC, is at an approximately fixed potential, the voltage at the emitter follows the voltage at the base. The common-collector circuit is therefore also often called an *emitter follower*.

If the input voltage at the base rises, for example during a positive half cycle, the emitter current increases. As a result, the voltage drop across the emitter resistor increases and the output voltage rises too. Input and output signals are therefore in phase; the phase shift is $\qty{0}{\degree}$.

[question:AD405]

---

Figure [ref:a_collector_circuit] shows a simple common-collector circuit with power supply, emitter resistor and coupling capacitors. 

<margin>
[picture:140:a_collector_circuit:Common-collector circuit with power supply, emitter resistor and coupling capacitors]
</margin>

---

To operate as a linear current amplifier, the transistor in the common-collector circuit needs a defined operating point (bias), which is normally set by a potential divider at the base.

Figure [ref:a_kennlinie] shows the characteristic of an NPN transistor with the operating point set by the potential divider. The base bias is chosen so that the transistor works on the linear part of the input characteristic. This also implies that a certain quiescent current always flows, even when there is no input signal. We will look at this in more detail in the chapter on amplifier classes. 

If an input signal, e.g. a sinusoidal AC voltage, is applied as shown in the picture, this signal is amplified according to the input characteristic. Note the labelling of the axes here: microamperes become milliamperes. The resulting output voltage can also be read off this characteristic 

<margin>
[picture:1119:a_kennlinie:Characteristic of an NPN transistor with operating point and superimposed signal]
</margin>

The emitter resistor converts the current flowing through the collector-emitter path into a voltage drop, which is taken off at the emitter. The emitter current of the transistor (together with the base current component, which is normally negligible) flows via the emitter through the emitter resistor to chassis. Through the voltage drop it produces across the emitter resistor, the current through this resistor raises the emitter potential (emitter voltage) and so acts as negative feedback on the base voltage. This additionally stabilises the operating point of the transistor, because temperature-related changes in the collector current are compensated in this way.

The signals are coupled in and out at the base and emitter through so-called coupling capacitors. Their job is to keep DC components that would shift the operating point away from the amplifier stage.

The decoupling capacitor on the supply voltage (+) serves to divert unwanted RF and AF signals, so that feedback effects on the stage and on the supply voltage are avoided. In addition, the decoupling capacitor connects the collector, as far as the signal is concerned (for AC), to both the input and the output.

With suitable design, the voltage gain of the common-collector circuit lies in the range from $\num{0.9}$ to $\num{0.98}$, and is always slightly less than $1$. 

You might now ask what use an amplifier with a voltage gain of less than $1$ is. The common-collector circuit has a decisive advantage, however, which we look at below. 

[question:AD402]

The common-collector circuit has a considerable current gain. Its input impedance is relatively high, because only a small current can flow into the base. The output impedance, on the other hand, is relatively low. If the output voltage is changed by a connected load, the base-emitter voltage changes as a result, and the transistor adjusts its emitter current so as to counteract this change. This negative feedback enables the common-collector circuit to drive a low-impedance load without its output voltage changing much.

[question:AD403]

For this reason the common-collector circuit is often used as a *buffer stage between an oscillator and further parts of the circuit* that would otherwise present a low-impedance load to the oscillator, in order to decouple the oscillator and improve its frequency stability.

[question:AD404]