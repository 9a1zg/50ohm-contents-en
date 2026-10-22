SMD components are only a few millimetres in size. SMD stands for surface-mounted device. Unlike conventional components, they have no wire leads but are soldered directly onto the printed circuit board – with no through-holes at all. Below, we look at how SMD resistors are marked.

<margin>
[photo:318:e_platine_smd:Circuit board with SMD components]
</margin>

---

Figure [ref:e_smd] shows an SMD resistor. To indicate the resistance value, digits are printed on it – in this case 113. The value of the resistor is then found as follows: all the digits except the *last* are taken as a plain number. In the example 113, this gives *11* as the number. The *last* digit gives the *power of ten* by which the other digits are to be multiplied. A 1 stands for the first power of ten, $10^1$, a 2 for the second power of ten, $10^2$, and so on.

<margin>
[picture:1006:e_smd:SMD component]
</margin>

In our example we therefore get: $11 \cdot 10^3$, i.e. $\qty{11000}{\ohm}$ or $\qty{11}{\kilo\ohm}$.

[question:EC114]
[question:EC115]
[question:EC116]
[question:EC117]