We have now met resistance and its unit, the $\unit{\ohm}$ (ohm). In practice, however, the numerical value is usually not printed on resistors. Instead, colour bands are used. These colour bands encode the value of the resistor.

<margin>
[picture:665:n_widerstandsfarbcodes: A resistor with 4 colour bands]
</margin>

Figure [ref:n_widerstandsfarbcodes] shows a resistor with four colour bands. Each colour corresponds to a number, as shown in the *Value* column of Table [ref:n_widerstandsfarbcodes_tabelle]:
* The first colour band corresponds to the first digit, in this case *yellow*, i.e. four.
* The second colour band corresponds to the second digit, in our example *violet*, i.e. seven.
* The third colour band is the multiplier (see Table [ref:n_widerstandsfarbcodes_tabelle]), in our case *orange*, i.e. the value 1000.

<webmargin>
| X:Colour | l:Value | l:Multiplier | l:Tolerance |
| Silver | - | $\num{0.01}$ | $\qty{\pm 10}{\percent}$ |
| Gold | - | $\num{0.1}$ | $\qty{\pm 5}{\percent}$ |
| Black | 0 | $\num{1}$ | - |
| Brown | 1 | $\num{10}$ | $\qty{\pm 1}{\percent}$ |
| Red | 2 | $\num{100}$ | $\qty{\pm 2}{\percent}$ |
| Orange| 3 | $\num{1000}$ | - |
| Yellow | 4 | $\num{10000}$ | - |
| Green | 5 | $\num{100000}$ | - |
| Blue | 6 | $\num{1000000}$ | $\qty{\pm 0.25}{\percent}$ |
| Violet | 7 | $\num{10000000}$ | $\qty{\pm 0.1}{\percent}$ |
| Grey | 8 | $\num{100000000}$ | - |
| White | 9 | $\num{1000000000}$ | - |
| None | - | - | $\qty{\pm 20}{\percent}$ |
[table:n_widerstandsfarbcodes_tabelle:Resistor colour code table]
</webmargin>

The first and second bands together give the number 47. Multiplying this number by the multiplier gives the value of the resistor:

$ 47 \cdot \qty{1000}{\ohm} = \qty{47000}{\ohm} = \qty{47}{\kilo\ohm} $

---

That leaves a fourth colour band. It stands for the tolerance, which states by how much the actual resistance value may deviate from the printed value.
More details on this follow in Class E. 

<indepth>
*In depth:* In our example the last band is *silver*, which means a tolerance of $\qty{\pm 10}{\percent}$. The true value of the resistor can be $\qty{10}{\percent} \cdot \qty{47}{\kilo\ohm} = \qty{4.7}{\kilo\ohm}$ more or less than the stated value. So it can lie anywhere between $\qty{42.3}{\kilo\ohm}$ and $\qty{51.7}{\kilo\ohm}$.
</indepth>

---

You do not have to learn the colour code table by heart. It is part of the formula sheet provided as an aid in the examination. You should, however, remember the order of the bands and what they mean. For practice, and to build up routine, the following questions can be solved using the colour code.

<indepth>
*In depth:* There are also resistors with more than four colour bands. These, however, are not relevant to the examination. Other components are often marked with colour bands too.
</indepth>

[question:NC107]
[question:NC105]
[question:NC106]
[question:NC104]
[question:NC103]
[question:NC102]
[question:NC108]
[question:NC109]
[question:NC110]
