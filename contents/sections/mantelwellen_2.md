Ideally, the currents through the inner and outer conductors of a coaxial cable are exactly equal in magnitude and opposite in direction. Their sum is therefore zero, and this is called a pure *differential-mode signal*. It is precisely then that no common-mode currents occur.

If, on the other hand, the sum of the signal is not zero, what is called a *common-mode signal* is present. The common-mode component of a current in the coaxial cable always flows on the outside of the outer conductor and is therefore a sheath current, with its associated sheath wave around the coaxial cable.

[question:AG425]

We have already learnt that a coaxial cable wound on a ferrite core is suitable for suppressing common-mode currents. This is one form of what is called the *current-compensated choke*.

A choke is an inductor intended to block RF currents. The current-compensated choke is a type of choke in which two separate windings are wound on the same magnetic core. The current-compensated choke is connected so that differential-mode signals, i.e. signals in which the current in one winding is exactly opposite to that in the other winding and otherwise of the same magnitude, induce no magnetic field in the core. The current-compensated choke therefore lets differential-mode signals pass unhindered. Common-mode components, however, e.g. currents that flow only on the outer conductor and therefore only in one winding, are blocked by the inductance.

[question:AG426]

<margin>
[picture:633:e_mantelwellen:Common-mode currents]
</margin>

---

An alternative to the current-compensated choke is an RF isolating transformer. Since the primary and secondary windings are not connected to each other, a current that flows into the isolating transformer at one terminal must (at least approximately) also flow out again at the other terminal with the same magnitude. A common-mode component is thus ruled out.

<indepth>
Since capacitance forms between the turns of a winding of an isolating transformer, and the winding also has capacitance to the other winding, even an isolating transformer does not suppress the common-mode component of a signal completely.
</indepth>

[question:AJ115]

If a coaxial cable is free of RF common-mode signals, the outer conductor has no RF voltage to earth. This is because with a differential-mode signal, i.e. opposite currents in the inner and outer conductors, an electric field forms only between the inner and outer conductors. Seen from outside, the effects of the two currents cancel, since their sum is zero. The presence of common-mode currents is therefore directly linked to the presence of RF voltages on the outer conductor.

Exactly such voltages on the outer conductor arise, for example, when we connect a balanced antenna to the cable, because at the feed point each dipole leg has a voltage to earth. If we connect each leg to one conductor of the coaxial cable, the outer conductor will also have a voltage to earth.

Well-earthed antennas, on the other hand, e.g. a ground-plane antenna with many well-tuned or buried radials, have a voltage of almost zero to earth at the feed point of the radials. Poorly earthed ground-plane antennas, by contrast, can be prone to common-mode currents.

Another way in which common-mode currents can arise is through contactless coupling into the coax screen. If, for example, a feeder is run parallel to a dipole leg, coupling occurs via the electromagnetic near field of the antenna.

[question:AG427]

With completely balanced antennas, what is called a voltage balun can be used to balance the currents in the coax. A popular design is an autotransformer, in which the coaxial cable is connected to the centre and to one end of a coil, and the antenna to the two ends of the coil.

% TODO: Bild Spannungsbalun / Spartransformator

Besides the desired balancing, this design also doubles the voltage ($ü = 2$) and correspondingly halves the current, which corresponds to a 1:4 impedance transformation; i.e. a $\qty{50}{\ohm}$ coaxial cable should be connected to an antenna with a feed-point impedance of $\qty{200}{\ohm}$ if possible.

[question:AG421]
[question:AG422]

However, this design is only suitable for suppressing common-mode currents if the connected antenna actually behaves in a balanced way and is not loaded unevenly by influences from its surroundings.

What all components used to suppress common-mode currents have in common is that "contactless" coupling via the electromagnetic near fields of the antennas directly onto the coax screen, i.e. beyond the common-mode choke, can still occur. Here, for example, a further, additional common-mode choke some distance from the antenna can help.

[question:AG428]
[question:AG429]