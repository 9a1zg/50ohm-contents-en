% Halbleiter II
% DF2DR 2024-08-19

Semiconductor materials are the basic stuff of our modern world. Reason enough to look at them in a little more detail. Semiconductors have a crystal lattice structure, which means that their atoms are arranged periodically. 

<margin>
[picture:854:a_silizium_halbleiter:Silicon semiconductor crystal]
</margin>

All semiconductor materials have two properties in common:

---

There is an *energy band gap*, which is a consequence of the periodic structure. This means that electrons in the crystal cannot take on certain energies. We call the highest energy that electrons bound to atoms have the *valence band energy*. But since these electrons are all bound to lattice atoms, they cannot contribute to current flow. There are further energy states that the electrons can reach – they lie in the *conduction band*, which lies above the valence band edge by the amount of the band gap. Electrons in the conduction band can contribute to current flow when we apply a voltage to the semiconductor sample. To get there, they need an energy greater than the energy band gap. They can take up this energy in the form of thermal energy, which is why high-purity semiconductors are very good insulators at low temperatures.

[question:AB104]

<margin>
The band-gap energy is determined by the chemical composition of the semiconductor. Compared with Si, Ge has a considerably smaller band-gap energy, GaAs and InP a somewhat larger one, and GaN a much larger one.
</margin>

Silicon (Si) and germanium (Ge) are *elemental semiconductors* (as, incidentally, is diamond, which is crystalline carbon). But there are also chemical compounds that are semiconductors (*compound semiconductors*), such as gallium arsenide (GaAs), indium phosphide (InP) or gallium nitride (GaN). 

---

Materials with an energy band gap are only called semiconductors if they can also be *doped*. Their conductivity can be changed within wide limits by deliberately contaminating the high-purity semiconductor material. Arsenic (As), for example, has one electron more in its outer electron shell than the elemental semiconductors. This electron can very easily, and with little energy, become a free electron in the conduction band. We call this kind of doping *n-type doping*.

<margin>
[picture:855:a_n_dotierung:n-type doping]
</margin>

---

But what happens if we contaminate the semiconductor with a material that has one electron too few in its outer electron shell? We call such an electron vacancy a *hole*. Since the atom was previously neutral, the electron vacancy carries a positive charge. The holes can also move through the crystal and contribute to current flow. We call this kind of doping *p-type doping*.

<margin>
[picture:856:a_p_dotierung:p-type doping]
</margin>

To sum up, we can say:
* n-type doping produces an excess of electrons in the semiconductor.
* p-type doping produces an excess of holes in the semiconductor.

[question:AB105]
[question:AB106]
[question:AB107]

---

If p-doped and n-doped zones are combined in one crystal, but separated in space, charge carriers are exchanged at the contact plane: electrons move from the n-doped region towards the p-doped region, and holes move from the p-doped region towards the n-doped region. We call this movement of charge carriers, which is caused by the differences in the densities of electrons and holes, the diffusion current.

This separation of charge, on the other hand, creates an electric field with the opposite effect, which leads to a drift current. In equilibrium (with no externally applied voltage), the effects of diffusion and of the electric field just balance each other. Between the p- and n-zones a region with no free charge carriers forms, which is called the *depletion region* or *depletion layer*. Such a structure is a *pn diode*.

[question:AB108]

<margin>
[picture:857:a_pn_uebergang:PN junction]
</margin>

---

Now we apply an external voltage that is more positive at the p-region (*anode*) than at the n-region (*cathode*). The positive electrode attracts electrons across the depletion region, and the negative electrode attracts holes. The depletion region is broken down and current flows. This is operation in the *forward direction*.

<margin>
[picture:956:a_pn_uebergang_mit_spannung:PN junction with external voltage]
</margin>

[question:AC402]

---

If we now reverse the voltage, the depletion region widens and the current flow comes to a standstill. This is *reverse-biased operation* of the diode.

<margin>
[picture:957:a_pn_uebergang_mit_spannung:PN junction with external voltage]
</margin>


[question:AB109]