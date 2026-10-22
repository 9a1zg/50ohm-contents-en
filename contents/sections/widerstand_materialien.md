% TODO: Wenn der Fragenkatalog 4 kommt, dann fallen hier einige Fragen weg! 

We have already met electrical resistance in connection with Ohm's law. Resistors can be made from different materials. For this reason, different resistor materials are distinguished, e.g.:

- Wirewound resistors
- Carbon-film resistors
- Metal-film resistors
- Metal-oxide resistors
- ...

<margin>
| l: Resistor | X: Property |
| Wirewound resistors | High-power resistors for low frequencies |
| Metal-film resistors | Small manufacturing tolerances and little temperature dependence, precision resistors |
| Metal-oxide resistors | For frequencies above $\qty{30}{\mega\hertz}$ |
[table:e_eigenschaften_widerstaende:Overview of the properties]
</margin>

Below we look at these materials in more detail – a summary is given in Table [ref:e_eigenschaften_widerstaende].

*Wirewound resistors* are among the oldest forms of electrical resistor. Because of their favourable properties – such as a high overload capacity and a low temperature coefficient – they are still used today. They are also often called wound resistors, since enamel-insulated resistance wire, made for example of manganin or constantan, is wound onto a ceramic former. A simple wound wirewound resistor, however, always acts as a coil as well, and therefore has a comparatively high inductance. We will look at inductors in more detail in a later chapter; it should be mentioned here, though, that this makes the impedance of the resistor frequency-dependent. In radio engineering this behaviour is usually undesirable. Wirewound resistors are therefore suited above all as high-power resistors for DC or for low-frequency applications.

%EC101 Hochlast niedrige Frequenz -> Drahtwiderstand
[question:EC101]

In carbon-film resistors, a thin film of carbon is vapour-deposited onto a substrate as the resistive material. Carbon-film resistors are inexpensive, but have a comparatively large manufacturing tolerance. They have comparatively low inductance and are therefore suitable for RF applications to a limited extent.

In *metal-oxide resistors*, the resistive material is applied as a thin film to a substrate. This type of resistor has, for the most part, low inductance and good temperature stability, so it is particularly suitable for use at higher frequencies, above $\qty{30}{\mega\hertz}$.

%EC103 induktionsarm 30Mhz - >Metalloxid
[question:EC103]

*Metal-film* resistors can be manufactured with high accuracy, that is, with a small manufacturing tolerance. They are suitable as precision resistors. They are independent of temperature, but their inductance is not as low.

%EC102 Präzisionswiderstand >Metallschichtwiderstand
[question:EC102]


We already met dummy loads in Class N. For high frequencies (e.g. VHF) it is advisable to build a dummy load preferably from metal-oxide resistors without a spiral cut. For lower frequencies (e.g. $\qty{50}{\mega\hertz}$ or $\qty{28}{\mega\hertz}$), however, carbon-film resistors can also be used. What matters above all is that the resistor has no turns, i.e. no self-inductance, and so does not act as a parasitic inductor, because such an inductance would make the resistance value frequency-dependent – exactly what is undesirable in a dummy load. The resistance should always be about $\qty{50}{\ohm}$, independent of frequency. That is why wirewound resistors should _not_ be used. For the same reason, the self-capacitance should also be as low as possible. In addition, the resistors used must be sufficiently heat-resistant, since they convert the power they absorb into heat.

%EC107 DL
[question:EC107]
%EC104 DL
[question:EC104]

To answer the following questions, you need to know that ten resistors of $\qty{500}{\ohm}$ each connected in parallel give a total resistance of $\qty{50}{\ohm}$. We will look at this relationship in more detail in a later chapter, when we talk about series and parallel connections of resistors.

%EC106
[question:EC106]
%EC105 DL
[question:EC105]