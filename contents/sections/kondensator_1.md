A very important and frequently used component in radio engineering and electronics is the capacitor. As shown in Figure [ref:e_kondensator_aufbau], a capacitor consists in principle of two conducting surfaces (plates, layers or electrodes) separated from each other by an insulator – the so-called dielectric.


<margin>
[picture:922:e_kondensator_aufbau:Basic construction of a capacitor]
</margin>

The geometrical dimensions determine an important property of a capacitor: its ability to store charge. This ability is called capacitance, and the symbol $C$ is used for it. The greater the capacitance, the more electric charge $Q$ can be stored. If the applied voltage is increased, more charge is stored as well.

The following formula shows the relationship. 

$Q = C \cdot U $ 

This formula is not on the formula sheet and is not needed for the examination either.

<unit>
The unit of charge $Q$ is the $\unit{\ampere\second}$
</unit>

<unit>
The unit of capacitance $C$ is the $\unit{\ampere\second\per\volt}$, or *farad* $\unit{\farad}$ for short, in honour of the English natural philosopher Michael Faraday (1791 - 1867). $\qty{1}{\farad}$ is the capacitance of a capacitor that stores a charge of $\qty{1}{\ampere\second}$ at a voltage of $\qty{1}{\volt}$.
</unit>

[question:EA101]

When a voltage is applied to a capacitor, an electric field $E$ arises between the conducting plates. We have already met this relationship in the chapter on the electric field: the higher the applied voltage and the smaller the spacing between the plates, the stronger the electric field. Mathematically this can be expressed as:

$E = \frac{U}{d}$

The capacitance of a capacitor is calculated from its dimensions with the following formula from the formula sheet:

---

$C = \frac{\varepsilon_0 \cdot \varepsilon_r \cdot A}{d}$

The individual quantities in the formula are explained below:

- $A$ is the area of the conducting plates facing each other
- $d$ is the spacing between the plates
- $\varepsilon_0 = \qty{0.855e-11}{\ampere\second\per\volt\meter}$ is the electric constant, a constant of nature
- $\varepsilon_r$  (say: "epsilon R") is a particular property of the insulator (dielectric), the so-called relative permittivity, which depends on the material used. Table [ref:e_Dielektrizitätszahl] with values for materials can also be found on the formula sheet.

<margin>
| Material | $\varepsilon_r$  |
| Air (dry) | 1.00059 |
| Solid PE (polyethylene) | 2.29 |
| Foam PE | 1.5 |
| PTFE (Teflon) | 2.0 |
[table:e_Dielektrizitätszahl:Relative permittivity $\varepsilon_r$ ]
</margin>

With the help of the formula, a number of examination questions can already be solved. The first thing to notice is that the voltage $U$ does not appear in the formula. 

[question:EC205]

The capacitance of a capacitor decreases when the plate spacing increases. 

[question:EC204]
[question:EC203]

---

Let us first look at the capacitor with direct current. Figure [ref:e_stromkreis_kondensator] shows a circuit for charging a capacitor. We assume that the capacitor $C$ is initially uncharged, that is, it has not yet stored any electric charge. When the switch is closed, the capacitor $C$ is connected through a resistor $R$ to a DC voltage source (a battery).

The applied voltage creates an electric field between the capacitor plates. This field causes charges to be redistributed: electrons are pushed from the negative terminal of the voltage source onto the capacitor plate connected to it, so that an excess of electrons builds up there. At the same time, electrons are drawn from the opposite plate to the positive terminal of the voltage source, which leaves a deficiency of electrons there. Although no current flows through the dielectric, this separation of charge charges the capacitor. 

<margin>
[picture:1015:e_stromkreis_kondensator:Circuit for charging a capacitor]
</margin>

---

This means that at first a large current flows, limited only by the resistor $R$. Over time, more and more charge is stored in the capacitor. As a result, the current falls steadily while the voltage $U_C$ across the capacitor rises, until the capacitor is fully charged. In this state, no current flows any more.

This process does not happen instantly, however, but with a delay. The capacitor voltage rises following a so-called exponential function, as shown in Figure [ref:e_ladekurve_c]. How long the charging takes depends on the resistor in series: the larger the resistance, the longer it takes until the capacitor is "fully" charged. With an oscilloscope, which we have already met, this variation with time can be clearly observed and studied, as shown in Figure [ref:e_lade_entladespannung_mit_oszilloskop].

<margin>
[picture:185:e_ladekurve_c:Charging voltage of a capacitor]
</margin>

<margin>
[photo:247:e_lade_entladespannung_mit_oszilloskop:Charging and discharging voltage of a capacitor]  
</margin>
 
During discharge, the current flows in the opposite direction to the charging current, and the voltage across the capacitor slowly falls.

[question:EC201]

With alternating current and AC voltages we must take another important aspect into account: a capacitor behaves like a frequency-dependent resistance. This can be described by the relationship

$|X_C| = \frac{1}{\omega\cdot C} = \frac{1}{2\pi\cdot f \cdot C}$

and is called the capacitive reactance $X_C$ (see the formula sheet).

We only learn the exact physical background in Class A. For Class E, however, it is already important to know that the resistance of a capacitor is inversely proportional to the frequency: if the frequency is reduced, the capacitive reactance $X_C$ becomes larger. If, on the other hand, the frequency is increased, the resistance falls accordingly.

[question:EC202]

---

We have now met some basic electrical properties of a capacitor, and next we want to look at the different types. Figure [ref:e_kondensatorvarianten] shows various types of capacitor.

<margin>
[photo:206:e_kondensatorvarianten:Types of capacitor]
</margin>

Various materials can be used as the dielectric, that is, the insulating layer:

1.  Air in an air-spaced variable capacitor or air trimmer
2. Plastic film in a wound film capacitor
3. Ceramic for high-Q RF capacitors and in SMD capacitors
4. Metal oxide in an electrolytic capacitor.

Depending on the construction, a further distinction is made between:

* Fixed capacitors in the form of ceramic capacitors, film capacitors and electrolytic capacitors
* Variable capacitors in the form of rotary variable capacitors and trimmer capacitors

---

*Air-spaced capacitors* and *ceramic capacitors*, as shown in Figure [ref:e_aufbau_keramik_c], are often used in RF filters, for example. 
[question:ED216] 

<margin>
[picture:923:e_aufbau_keramik_c: Ceramic capacitor]
</margin>

*Electrolytic capacitors* contain a thin, roughened aluminium foil immersed in an electrolyte (borax, for example). The electrolyte causes the aluminium surface to oxidise chemically. The resulting oxide layer is very thin, and so the capacitance rises very sharply for a small size. However, the thin layer has only a limited voltage rating, which is marked on the electrolytic capacitor.
Electrolytic capacitors may only be operated on DC voltage. The polarity must therefore be observed, as otherwise the oxide layer breaks down and the voltage rating falls. The capacitor is destroyed. All other capacitors can also be connected to AC voltage.
[question:EC207]

%<margin>
%TODO: Bild Elko
%</margin>

For wound film capacitors, plastics are processed into extremely thin films by special methods, provided with electrodes and then either wound into a roll or built up from individual layers and assembled into a capacitor, as shown in Figure [ref:e_aufbau_wickel_c]. Together with ceramic capacitors and electrolytic capacitors, they are among the most commonly used types of capacitor.

<margin>
[picture:49:e_aufbau_wickel_c:Wound film capacitor]
</margin>

Variable capacitors are often used in output stages and matching networks. Their capacitance can be adjusted because some of the capacitor plates are mounted on an insulated spindle and rotate between fixed plates. This changes the effective overlapping area of the plates and so the capacitance, as shown in Figure [ref:e_drehkondensator]. Trimmer capacitors work on a similar principle but are not intended for regular adjustment. Rather, they are used for one-off or occasional alignment of circuits, for example when putting them into service or calibrating them.

[question:EC206]

<margin>
 [picture:840:e_drehkondensator:Construction of a variable capacitor]
</margin>

The circuit symbols used for the different capacitors also differ, as shown in Figure [ref:e_kondensator_schaltzeichen].

<margin>
[picture:924:e_kondensator_schaltzeichen:Circuit symbols of various types of capacitor]

Key to the circuit symbols: 
a) Fixed capacitor 
b) Polarised capacitor / electrolytic capacitor / tantalum capacitor
c) Variable capacitor 
d) Trimmer capacitor for alignment
</margin>
