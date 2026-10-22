The basic function of the diode is already familiar from the Class N course: it lets current flow in one direction only, namely when the voltage at the anode ($U_a$) is greater than the voltage at the cathode ($U_k$), see Figure [ref:e_diode_u_i].

<margin>
[picture:859:e_diode_u_i:Voltages and current in a diode with a series resistor]
</margin>

Mathematically, we can write this condition as:

$U_d = U_a - U_k > 0$

However, if $U_d$ is only very slightly greater than 0, no appreciable current flows yet. This is due to the *exponential characteristic* of a diode. The diode current is:

$I_d = I_S \left(e^{\frac{U_d}{U_T}}-1\right)$

$e$ is Euler's number ($e\approx 2.718$), and $U_T$ is a constant of about $\qty{26}{\milli\volt}$ at room temperature.

$I_S$ here is the *reverse saturation current*, the very small current that flows through the diode at negative voltages. Besides a few parameters of the diode, such as the diode area, the value of $I_S$ depends above all on the semiconductor material used. In materials such as germanium (Ge) with a small *energy band gap* (we go into this in more detail in the Class A course), $I_S$ is larger; in materials with a larger energy band gap, $I_S$ is smaller. 

<margin>
[picture:861:e_diode_kennlinie_iu:Characteristic of a diode]
</margin>

[question:EC501]

If we look at a diode characteristic in Figure [ref:e_diode_kennlinie_iu], the diode current rises steeply for positive $U_d$ above a certain voltage. This voltage is also called the *threshold voltage* $U_{th}$, but it is only an expression of the different values of $I_S$: the smaller $I_S$, the higher the threshold voltage. 

As a guide to the threshold voltage of pn diodes, we can give about $\qtyrange{0.2}{0.3}{\volt}$ for Ge and about $\qtyrange{0.6}{0.7}{\volt}$ for Si.

*Light-emitting diodes* (LEDs) are also pn diodes, in which the semiconductor material is such that it emits light when the diode is forward-biased. This only works with certain materials – not with Si and Ge. The colour of the light is determined by the energy band gap. The larger the energy band gap, the shorter the wavelength of the light, the lower the reverse saturation current, and therefore the higher the threshold voltage. That is why red LEDs have a threshold voltage of about $\qty{1.7}{\volt}$ and green LEDs $\qty{2.5}{\volt}$. The different characteristics are shown in Figure [ref:e_diode_kennlinien].

[question:EC513]
[question:EC510]
[question:EC509]
[question:EC511]
[question:EC512]

---

<margin>
[picture:858:e_diode_kennlinien:Characteristics of different diodes]
</margin>


[question:EC503]
[question:EC506]
[question:EC507]
[question:EC508]

Since LEDs are operated in the forward direction, it is important to connect a resistor $R_V$ between the voltage source $U$ and the LED. $R_V$ sets the desired current $I$. The threshold voltage $U_{th}$ of the LED has to be taken into account:

$ I=\frac{U-U_{th}}{R_V}$

[question:EC514]
[question:EC515]
[question:EC516]

---

In our simple model, only a small reverse current flows for negative $U_d$. But this is not true for very negative voltages. At some point the electric field across the depletion region between n and p becomes too high and the diode "breaks down": the current in the reverse direction rises extremely sharply, as shown in Figure [ref:n_diode_kennlinie_uz].

This *reverse breakdown* can have various physical causes, which we cannot cover in detail here. The voltage at which this breakdown happens is commonly called the *Zener voltage* $U_z$, even though the Zener effect (a quantum-mechanical tunnelling effect) is only one possible breakdown mechanism. *Zener diodes* are used for voltage stabilisation. It is important to limit the breakdown current with a series resistor. 

<margin>
[picture:862:n_diode_kennlinie_uz:Characteristic of a Zener diode]
</margin>

---

The circuit symbol of a Zener diode (Figure [ref:e_zener_symbol]) is that of an ordinary diode in which the cathode bar has an additional extension at $\qty{90}{\degree}$. This is meant as a reminder of the "bend" in the characteristic at breakdown.

<margin>
[picture:860:e_zener_symbol:Circuit symbol of a Zener diode]
</margin>



[question:EC517]
[question:EC520]
[question:EC521]
[question:EC522]

The diodes covered so far were all *pn diodes*: the diode property comes from a semiconductor junction. The *Schottky diode* is a diode whose properties come from a metal-semiconductor junction. Its threshold voltage is about half that of a pn diode made of the same material, or less, depending on the exact design of the metal-semiconductor junction. Schottky diodes are used where the threshold voltage is to be low, or else as very fast switching diodes.  

[question:EC504]
[question:EC505]

<margin>
Metal-semiconductor diodes are the oldest semiconductor rectifier components. Ferdinand Braun discovered their rectifying effect as early as 1874, but without being able to explain his observation.
</margin>

To sum up:

Diodes let current flow in one direction only. This makes them suitable for rectifying alternating current.

At high reverse voltages ($U_d < U_z$), however, the current in the reverse direction rises sharply. This operating point can be used very well for voltage stabilisation (*Zener diode*).

In addition, in the reverse direction they can also be used as voltage-controlled capacitances, but we will not cover this until the Class A course. 

[question:EC502]
[question:EC518]
[question:EC519]
