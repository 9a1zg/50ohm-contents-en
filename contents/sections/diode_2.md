[question:AC401]

The pn diode consists of two semiconductor regions which, through the process of doping, have either an excess of free electrons (n) or of free holes (p). On either side of the boundary a so-called space-charge region forms, which contains practically no free charge carriers. The n-region is the cathode, the p-region the anode. 

If a forward voltage is applied to the diode (positive at the anode, negative at the cathode), electrons are driven from the n-doped region towards the p-region, and holes from the p-region towards the n-region. This gives the correct answer.

What may be a little confusing is that the conventional current flow is in the opposite direction to the flow of electrons. So the current arrow points from the anode to the cathode, although the electrons flow from the cathode to the anode.

[question:AC403]

pn diodes show an exponential dependence of the diode current on the diode voltage. The saturation current rises as the temperature rises. As a result, the diode voltage needed for a given diode current becomes smaller as the temperature rises. So the "forward voltage" falls (as a rule of thumb, by $\qty{-2}{\milli\volt\per\kelvin}$ of temperature rise).
<indepth>

The diode current is:
  
$I_D(T) = I_S(T) \cdot e^{\frac{U_D}{U_T}}$
  
$I_S$ is the saturation current, and $U_T = k T/q$ is the so-called thermal voltage. Here $k$ is the Boltzmann constant and $q$ the elementary charge.
  
As the temperature rises, the saturation current rises and the exponential function falls. However, the temperature dependence of the saturation current predominates.

</indepth>

[question:AC404]

---

The varactor diode (see Figure [ref:a_diode_kapazitaet]) uses the capacitance between the n- and p-regions across the space-charge region, in the same way as a parallel-plate capacitor. However, no appreciable direct current may flow, so the diode must be reverse-biased.

<margin>
[picture:1068:a_diode_kapazitaet:Circuit symbol of a varactor diode]
</margin>

The more negative the diode voltage (or the higher the reverse voltage), the further the space-charge region extends and the smaller the diode capacitance becomes.

In questions AC405 and AC406, *diodes in inverse parallel* are used to limit the amplitude of an AC voltage. Circuits like this are used, for example, to protect receiver inputs from voltages that could destroy the input transistors.

[question:AC405]

These are silicon diodes, which have a threshold voltage of about $\qty{0.6}{\volt}$. So if the input voltage exceeds $\qty{0.6}{\volt}$, the right-hand diode switches on. If it falls below $\qty{-0.6}{\volt}$, the left-hand diode switches on.

In the first half cycle the necessary voltage is not yet reached, so it is passed on unchanged. The next two half cycles, however, have amplitudes that exceed the threshold voltage. The amplitudes are "clipped" at $\qty{\pm 0.6}{\volt}$.

[question:AC406]

The solution is the same as for the previous question – but here the diodes are *germanium diodes*, with a threshold voltage of about $\qty{0.3}{\volt}$. That is why all the half cycles are clipped.

[question:AC407]

The following describes components that interact with light: the light-dependent resistor and the photodiode.

The light-dependent resistor is a component with two non-rectifying contacts. It behaves like a conventional ohmic resistor – the current rises linearly with the applied voltage. Its resistance can be reduced by the absorption of light – the absorbed photons increase the density of free charge carriers. If no voltage is applied, no current flows either.

---

The photodiode, on the other hand, is a pn diode (see Figure [ref:a_photodiode]). Here the light is absorbed in the space-charge region, producing electron-hole pairs, which are separated in the electric field of the space-charge region. This field exists even without an external bias. A current flows even for $U_D=0$ (a short-circuit current). This current flows in the opposite direction to the conventional diode current. 

<margin>
[picture:1069:a_photodiode:Circuit symbol of a photodiode]
</margin>

---

[question:AC408]

Optocouplers combine a light-emitting diode and a photodiode in one package, with the input side (light-emitting diode) and the output side (photodiode) insulated from each other (galvanically isolated).

These components are used to isolate interfaces galvanically, for example to prevent earth loops, which can cause mains hum to be picked up.

<margin>
[picture:1070:a_optokoppler:Circuit symbol of an optocoupler]
</margin>