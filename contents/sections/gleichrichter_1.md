<margin>
[picture:666:n_halbleiter_diode_merkhilfe:Diode memory aid]
</margin>

To produce a DC voltage from an AC voltage, a rectifier is needed. The simplest form of rectification uses a diode. As we already learnt in Class N, a diode lets current flow in one direction only.

---

We use this property of the diode to produce a DC voltage from an AC voltage (see Figure [ref:e_einweggleichrichter_ue]). If a load resistor is connected to an AC voltage source through a diode in series (circuit in Figure [ref:e_einweggleichrichter]), the diode conducts the current only when the anode is more positive than the cathode. In this case the positive half cycle of the AC voltage is let through.

During the negative half cycle the diode blocks, so that the output voltage stays at zero during this time (see Figure [ref:e_einweggleichrichter_ul]). Since this circuit uses only one half cycle of the sinusoidal AC voltage, it is called *half-wave rectification*.

---
<margin>
[picture:797:e_einweggleichrichter:Half-wave rectifier]
[picture:798:e_einweggleichrichter_ue:Input voltage of a half-wave rectifier]
[picture:796:e_einweggleichrichter_ul:Load voltage of a half-wave rectifier]
</margin>

[question:ED304]

If a sufficiently large capacitor is now also connected in parallel with the load resistor, it charges up quickly through the diode during the conducting half cycle. In the following half cycle, in which the diode blocks, the capacitor discharges slowly through the resistor. In this way the pulsating voltage is smoothed and approaches a DC voltage.

Besides half-wave rectification there are other rectifier circuits, for example the bridge rectifier. We will not go into these in more detail until Class A, however.