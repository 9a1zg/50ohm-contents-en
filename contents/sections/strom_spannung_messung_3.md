In Classes N and E we have already learnt how to measure current and voltage correctly and what properties the internal resistances of the meters have. If the meters are not connected into the circuit correctly, you get wrong or meaningless readings or, in the worst case, can damage the meter. In Class A there are two more questions on this that test correct measurement of current and voltage – but in a somewhat more complex context.

The first question is about measuring the power of a power amplifier (PA). We already know the relationship $P = U \cdot I$: the power can be determined by measuring voltage and current and then multiplying the two values. In Figure [ref:a_strom_spannung_messung], the supply, in the form of a power supply unit, is connected on the left, the PA is in the middle, and on the right a further load, the transmitter (TRX), is connected. If we now want to determine the power of the PA, only the current flowing into the PA may be measured.

<margin>
[picture:1003:a_strom_spannung_messung:Measuring the power of an amplifier (PA)]
</margin>

[question:AI101]

For the next question, let us remember the rules from Class E that voltmeters are always connected in parallel and ammeters always in series. This makes the question very easy to answer. 

[question:AI102]

---

In the following, we want to look at two parameters of measurement that are often confused:

- Resolution
- Accuracy (also called tolerance or error)

*Resolution* is the smallest change in the measured quantity that a meter can still display. Example: a multimeter with a resolution of $\qty{0.1}{\volt}$ cannot distinguish between $\qty{10.5}{\volt}$ and $\qty{10.45}{\volt}$ if the difference is smaller than the resolution. A meter with a resolution of $\qty{0.01}{\volt}$, on the other hand, can distinguish much more finely. The resolution is normally stated by the manufacturer of the meter.

<tip>
Let us first look at *resolution* using a clock. If the clock shows hours and minutes, the time can be given to the nearest minute. But whether it is 13 hours, 3 minutes and 10 seconds or 13 hours, 3 minutes and 59 seconds cannot be read off. *One minute* is therefore the *finest resolution* of the clock (correspondingly, a clock with a second hand has a finest resolution of one second).
</tip>

The *accuracy* (also measurement error or tolerance) of a meter describes by how much, at most, the displayed value may deviate from the true value – both upwards and downwards, for example $\pm\qty{5}{\percent}$. A simple rule of thumb is: the larger the range a meter is meant to cover, the lower, as a rule, the accuracy of the measurement.

The accuracy depends, among other things, on the internal resistance of the meter, since this affects the measurement result.
In Class E we learnt that an ammeter has a very low internal resistance (ideally $\qty{0}{\ohm}$), whereas a voltmeter has a very high internal resistance (ideally $\qty{\infty}{\ohm}$). In Class A we now also want to look at how accurately our meters can record the voltage or current that is actually present. The displayed value usually differs from the true value – and this is due to the imperfect internal resistances of the meters, which affect the measurement.

---

Let us look at the equivalent circuit of a real voltmeter in Figure [ref:a_reale_spannungsmessung] for the following examination question. Besides the ideal ammeter, a real voltmeter contains a resistor connected in parallel, e.g. of $\qty{10}{\mega\ohm}$. If this resistor were infinitely large, it would in practice not exist – and we would have an ideal meter. This means, however, that in a real voltage measurement a small current always flows through this resistor, and it affects our measurement result. Let us imagine, for example, that we want to measure the voltage at a potential divider: the internal resistance of the meter places a slight load on the potential divider, so that we do not measure exactly the voltage that an ideal meter would show. 

<margin>
[picture:1004:a_reale_spannungsmessung:Equivalent circuit of a real voltmeter]
</margin>

---

The ammeter behaves in a similar way to the voltmeter. A real ammeter consists of the actual ammeter and a small resistor connected in series, across which a small voltage is always dropped. If this resistor were zero, it would in practice not exist – and we would again have the ideal meter.

<margin>
[picture:1007:a_reale_strommessung:Equivalent circuit of a real ammeter]
</margin>

---

[question:AI104]

<tip>
In this question, the information "finest resolution $\qty{100}{\micro\volt}$" is not important. It can be solved with Ohm's law alone.
</tip>

---

What about parameters that are calculated from measured values – such as the power in our example from the beginning ($P = U \cdot I$) after measuring current and voltage? The individual measured quantities, such as current and voltage, each deviate from the true value because of measurement errors, and these deviations carry through into the calculation accordingly.

Let us look at a concrete example: suppose we want to determine the power, and to do so we measure a DC voltage and a direct current. Both meters show values that are each five per cent too low. Now you must not make the mistake of simply adding the deviations of the individual measured quantities. The power formula makes it clear that in this case the errors multiply. Let us look at this in detail:

$U_\text{Gemessen}=0.95 \cdot U_\text{Wahr}$ and $I_\text{Gemessen}=0.95 \cdot I_\text{Wahr}$

We calculate the power with our familiar formula:

$P_\text{Gemessen}=U_\text{Gemessen} \cdot I_{Gemessen}$

Now we substitute the true values: 

$P_\text{Gemessen} = 0.95 \cdot U_\text{Wahr} \cdot 0.95 \cdot I_\text{Wahr} = 0.9025 \cdot U_\text{Wahr} \cdot I_\text{Wahr}$

This means that the measured power is about $\qty{9.75}{\percent}$ lower than the actual power, because $1-0.9025 \equiv \qty{9.75}{\percent}$. With this knowledge the following examination question can be answered; the actual values of current and voltage are not relevant to the solution.

[question:AI103]
