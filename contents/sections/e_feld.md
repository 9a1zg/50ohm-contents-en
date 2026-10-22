The physical phenomenon that makes radio signals possible in the first place is the electromagnetic field. That this field can propagate through empty space, without a medium to carry it, was one of the most important discoveries of the 19th century. 

<margin>
For a long time, physics believed in the existence of an "aether" that is present everywhere and in which electromagnetic waves propagate as sound does in air. This idea was wrong, but the term has survived in everyday language as "the ether": we sit at the receiver, for example, and *listen in to the ether*.
</margin>

---

As the name already suggests, the electromagnetic field consists of two components, the electric field and the magnetic field. When the electric and the magnetic field vary with time, the two field components always occur together.

But let us begin with the electric field that does not vary with time, also called a static field. The electric field is generally denoted by the letter $E$.

<margin>
[picture:881:e_plattenkondensator: A parallel-plate capacitor with a voltage applied and a uniform electric field]
</margin>
  
---

Figure [ref:e_plattenkondensator] shows a schematic of a *parallel-plate capacitor* with a voltage $U$ applied to its plates. The plates are insulated from each other, and no current flows. The voltage causes positive charge carriers to collect on the left plate and negative ones on the right plate. A static electric field $E$ builds up between the two plates. If we assume that the length and width of the plates are very much greater than their spacing, the strength of the field does not depend on position -- we speak of a *uniform* field. The electric field strength can then be calculated quite simply:

$E = \frac{U}{d}$

where $d$ is the spacing of the plates. 

<unit>
The equation $E = \frac{U}{d}$ also gives the unit of electric field strength: $\unit{\volt\per\meter}$
</unit>

[question:EB101]
[question:EA103]

---

To calculate the electric field strength in a parallel-plate capacitor, we need to know the applied voltage and the plate spacing. Parallel-plate capacitors are often found in antenna tuning units. 

<danger>
In these questions, it is essential to pay attention to the correct unit!
</danger>

[question:EB102]

Here, again, we can simply calculate with the formula from above: 

$E = \frac{\qty{9}{\volt}}{\qty{0.6}{\centi\meter}} = \frac{\qty{9}{\volt}}{\qty{0.006}{\meter}} = \qty{1500}{\volt\per\meter}$

We can imagine a *wound capacitor* as a parallel-plate capacitor with very wide plates that have been rolled up. Between the plates, however, there is an insulating layer, the *dielectric*. It increases the *capacitance* of the capacitor -- its ability to store charge. The dielectric has no effect, however, on calculating the field strength inside.

[question:EB103]

For this question, too, we call on our formula again: 

$E = \frac{\qty{300}{\volt}}{\qty{0.15}{\milli\meter}} = \frac{\qty{300}{\volt}}{\qty{0.00015}{\meter}} = \qty{2000000}{\volt\per\meter} = \qty{2000}{\kilo\volt\per\meter}$

Dielectrics can withstand only a limited electric field strength before they lose their ability to insulate. The limiting field strength at which this happens is also called the *breakdown field strength*. If we know the breakdown field strength and the thickness of the dielectric, we can calculate the maximum voltage the capacitor can withstand.

If the breakdown field strength is $E_d$ and the thickness of the dielectric is *d*, the breakdown voltage is:

$U_d =E_d \cdot d$

[question:EB104]

Here we calculate with the formula from above (careful: watch the units!):

$\begin{split} U_d &= \qty{400}{\kilo\volt\per\centi\meter} \cdot \qty{0.15}{\milli\meter} \\ &= \qty{40000000}{\volt\per\meter} \cdot \qty{0.00015}{m} \\ &= \qty{6000}{\volt} \\ &= \qty{6}{\kilo\volt} \end{split}$

---

Another important skill is telling the electric field lines in sketches apart from the magnetic field lines, which are covered later. 

With a simple rule of thumb this is quite easy: electric field lines have a beginning and an end, magnetic field lines do not! The electric field always points from the more positive potential to the more negative one. 

[question:EB105]

<margin>
[picture:884:e_feldlinien_vertikalantenne:Field lines at a vertical antenna]
</margin>




