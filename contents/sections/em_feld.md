So far we have looked at electric and magnetic fields for the case where the fields do not vary with time. In radio engineering, however, such fields are actually of no interest, because we deal with voltages and currents that vary with time. The electric and magnetic fields they produce vary with time as well. 

<margin>
[picture:885:e_vertikalantenne_em:Electric and magnetic field at an antenna]
</margin>

Additional effects then come into play. As early as 1831, Michael Faraday discovered that a magnetic field that varies with time produces a voltage in a nearby conductor. This effect, called *induction*, is used for example in the transformer: a current that varies with time (e.g. a sinusoidal one) in the primary winding produces a magnetic field that varies with time, which in turn induces a voltage in the secondary winding.

To see that, conversely, a change in an electric field leads to a magnetic field, let us imagine a parallel-plate capacitor whose plates form a circuit with an external voltage source. If we change the electric field inside the capacitor, charges have to move in the external circuit. But moving charge carriers means an electric current. And this electric current in turn produces a magnetic field around the conductor.

While models with electrical conductors are easy for us to picture, it is very important to realise that these conductors are not necessary. Magnetic and electric fields also exist outside conductors, even in a vacuum. Here too, a magnetic field that changes with time produces an electric field that varies with time. This time-varying field in turn leads to a time-varying magnetic field. *Time-varying magnetic fields and time-varying electric fields are therefore always coupled.* That is why we speak of the *electromagnetic field*. In summary: an electromagnetic wave that can propagate freely in space is based on the interaction between time-varying magnetic and electric fields.

[question:EB302]

As described above, voltages and currents that are constant with time cannot produce an electromagnetic field. For that we need a current that varies with time in a conductor.

[question:EB301]

<indepth>
The magnetic field and the electric field are in fact described by *vectors*, that is, by quantities that have a direction in space. It can be shown mathematically that in the *far field*, that is, sufficiently far away from the antenna, the vectors of the two fields must be at right angles to each other. The direction of propagation of the electromagnetic wave (that is, of our radio signal ...) is in turn at right angles to both the electric and the magnetic field.
  
[picture:886:e_emfeld_ausbreitung:Propagation of the electromagnetic wave]
  
The relationships described are expressed mathematically by *Maxwell's equations*, named after James Clerk Maxwell, who worked them out between 1861 and 1864 from the observations of other physicists. In doing so, he came to the conclusion that the magnetic and electric fields must be coupled:
  
1. $\vec{\nabla} \cdot \vec{E} =\frac{\rho}{\varepsilon_{0}}$
2. $\vec{\nabla} \cdot \vec{B} = 0$
3. $\vec{\nabla} \times \vec{E} = -\frac{\partial\vec{B}}{\partial t}$
4. $\vec{\nabla } \times \vec{B} =\mu_0 (\vec{j} +\varepsilon_0 \frac{\partial\vec{E}}{\partial t})$
  
Equation (3) shows that a magnetic field that varies with time produces an electric field. According to equation (4), this time-varying electric field in turn contributes, through the displacement current, to producing a magnetic field. These relationships go far beyond what you need to know for amateur radio.
  
Experimentally, however, the existence of the electromagnetic field was demonstrated only more than twenty years later (1886), by Heinrich Hertz.
</indepth>

As shown in Figures  and [ref:e_emfeld_ausbreitung], in the far field (far away from the antenna) the magnetic field component is always at right angles to the electric field component.

[question:EB303]

The magnetic and electric field components, at right angles to each other in the far field, also determine the direction of propagation $S$, as shown in Figure [ref:e_vertikalantenne_em]: it is in turn at right angles to both. You can picture it like this: the magnetic and electric fields span a plane, and the direction of propagation is perpendicular to that plane.

[question:EB304]
