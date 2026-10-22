In the previous chapter we met the common-collector circuit of a bipolar transistor. In this chapter we look at the *common-emitter circuit*.

<margin>
[picture:1118:a_emitter_collector:Common-emitter and common-collector circuits, with the base (B), collector (C) and emitter (E) labelled]

Let us briefly summarise the properties of the common-collector and common-emitter circuits in the following table: 

| l: Property | X: Common-emitter circuit | X: Common-collector circuit |
| Phase shift | $\qty{180}{\degree}$ | $\qty{0}{\degree}$ |
| Voltage gain | $\num{100}\dots\num{300}$ | $\num{0.9}\dots\num{0.98}$ |
| Input impedance | high | high |
| Output impedance | high | low |
</margin>

As we learnt in the previous chapter, the basic circuits of a bipolar transistor are named after the terminal that serves neither as the input nor as the output of the circuit, and so forms the common reference point for the input and output circuits. In the common-emitter circuit, this is the emitter. 

---

[question:AD409]

<tip>
Bipolar transistor amplifier circuits are named after the terminal to which neither the input nor the output is directly connected (see Figure [ref:a_emitter_collector]). 
</tip>

---

Figure [ref:a_emitterschaltung] shows a simple common-emitter circuit with power supply, collector resistor and coupling capacitors.

To operate as a linear voltage amplifier, the transistor in the common-emitter circuit needs a defined operating point (bias), which is normally set by a potential divider at the base.

<margin>
[picture:136:a_emitterschaltung:Common-emitter circuit]
</margin>

[question:AD411]

The collector resistor converts the current flowing through the collector-emitter path into a voltage drop, which is taken off at the collector. The collector current of the transistor (together with the base current component, which is normally negligible) flows via the emitter through the emitter resistor to chassis. Through the voltage drop it produces across the emitter resistor, the current through this resistor raises the emitter potential (emitter voltage) and so acts as negative feedback on the base voltage. This additionally stabilises the operating point of the transistor, because temperature-related changes in the collector current are compensated in this way.

The signals are coupled in and out at the base and collector through so-called coupling capacitors. Their job is to keep DC components that would shift the operating point away from the amplifier stage.

[question:AD412]

The decoupling capacitor on the supply voltage (+) serves to divert unwanted RF and AF signals, so that feedback effects on the stage and on the supply voltage are avoided.

In the common-emitter circuit, the phase shift between the input and output signals is $\qty{180}{\degree}$, because during a positive half cycle of the input voltage at the base, the collector current rises and with it the voltage drop across the collector resistor. As a result, the voltage at the output capacitor falls. A negative half cycle appears at the output of the amplifier stage.

[question:AD407]
[question:AD408]

With suitable design, the voltage gain of the common-emitter circuit lies in the range $100\dots 300$, which is very high compared with the common-collector circuit.

[question:AD410]

The capacitor at the emitter bypasses the emitter resistor for AC, which reduces the negative feedback and increases the AC voltage gain, while the DC operating point remains unchanged.

[question:AD413]

If, however, the emitter capacitor is removed, the gain of the circuit falls considerably (e.g. from $\num{100}$ to $\num{10}$). It is then ultimately determined only by the ratio of the collector resistor to the emitter resistor.

[question:AD414]
[question:AD415]

If a common-emitter circuit is operated, as in the following question, without its operating point being preset by a potential divider, the transistor is driven by the input signal alone. Only when this signal exceeds approx. $\qty{0.6}{\volt}$ does the base-emitter path of the transistor become conductive. As a result, a collector current flows only at the voltage peaks, causing a voltage drop at the output. The output signal is the supply voltage, which drops at the times when the transistor enters the conducting region. This explains the output signal in question.

[question:AD406]

