Oscillators whose frequency can be controlled can be implemented in various ways. One possibility is the so-called *voltage-controlled oscillator (VCO)*.

[question:AD601]

<margin>
[picture:752:a_vco_schaltung:VCO circuit with a varactor diode]
</margin>

---

To make the frequency of the oscillator variable, a varactor diode can be inserted into its tuned circuit; its capacitance can be varied by a DC voltage (see Figure [ref:a_vco_schaltung]). A change in this DC voltage then leads to a corresponding change in the oscillator frequency. In this way the oscillator can be tuned by a control voltage. 

The varactor diode is operated with reverse bias. The higher the reverse voltage across the diode, the lower its capacitance, which is determined by the width of the depletion layer at the PN junction. The depletion layer widens as the reverse voltage applied is increased, which reduces the capacitance and so, according to Thomson's formula, raises the frequency of the tuned circuit.

Conversely, the depletion layer of the varactor diode narrows as the reverse voltage applied is reduced, which increases the capacitance and so lowers the frequency of the tuned circuit. The reverse voltage can be produced, for example, by a potentiometer or a control circuit.

<tip>
The higher the voltage across the varactor diode, the greater the spacing of the "plates" ($d$). A look at the formula sheet is always a good idea for understanding these chains of cause and effect.

$C = \epsilon_0 \cdot \epsilon_r \cdot \frac{A}{d}$

$f = \frac{1}{2\pi\sqrt{L\cdot C}}$

$U \uparrow \quad\rightarrow\quad C \downarrow \quad\rightarrow\quad f \uparrow$

$U \downarrow \quad\rightarrow\quad C \uparrow \quad\rightarrow\quad f \downarrow$
</tip>

[question:AD218] 

For all oscillator circuits, whatever their design, unwanted feedback can lead to frequency instability. This applies to VCOs as well as to VFOs (e.g. with variable capacitors) and other oscillators.

[question:AD611]