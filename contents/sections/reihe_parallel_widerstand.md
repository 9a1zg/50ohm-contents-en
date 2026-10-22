We are often faced with the problem that a resistance value we want is not in the so-called "preferred-value series" for resistors. It could also be that a resistor has to dissipate a large amount of power, more than commercially available single resistors can handle -- to name just two examples. We will now look at how we can obtain other resistance values by connecting resistors in series or in parallel.

From Ohm's law we can derive the rules for series and parallel connections of resistors:

$U=R \cdot I$

<margin>
[picture:819:e_spannungsteiler:Potential divider]
</margin>

Figure [ref:e_spannungsteiler] shows two resistors $R_1$ and $R_2$ connected one after the other. The same current *I* flows through both of them. The voltages dropped across the resistors are then

$U_1 = R_1 \cdot I$ and  $U_2 = R_2 \cdot I$. 
The total voltage $U_g$ is simply the sum of these two voltages:

$U_g = U_1 + U_2 = R_{\mathrm{ges}} \cdot {I} = R_1 \cdot I + R_2 \cdot I$

Now we can calculate the resistance seen between the outer terminals:
$R_{\mathrm{ges}} = \frac{U_g}{I} = R_1 + R_2$, because the current $I$ cancels out on both sides of the equation.

This also works for more than two resistors, as given in the formula sheet:

$R_{\mathrm{ges}} = R_1 + R_2 + R_3 + R_4 + \dots$

---

But what happens when we connect two resistors $R_1$ and $R_2$ in parallel, as shown in Figure [ref:e_parallelschaltung]? 

Now the same voltage $U$ is applied to both resistors, causing the currents

$I_1 = \frac{U}{R_1}$ and $I_2 = \frac{U}{R_2}$

to flow in them. 

<margin>
[picture:945:e_parallelschaltung:This circuit shows all the voltages and currents.]
</margin>

The current flowing in the external circuit is the sum of these two currents:

$I = I_1 + I_2 = \frac{U}{R_1} + \frac{U}{R_2}$

Again we are looking for a total resistance $R_{\mathrm{ges}}$, for which $I=\frac{U}{R_{\mathrm{ges}}}$ must then hold, and so:

$\dfrac{1}{R_{\mathrm{ges}}} = \dfrac{1}{R_1} + \dfrac{1}{R_2}$

---

The reciprocal of the total resistance is therefore the sum of the reciprocals of the individual resistances. One consequence is that, for a number of equal resistors connected in parallel, you simply divide the value of one resistor by the number of resistors.

Here too we can do the calculation for any number of resistors in parallel (see the formula sheet):

$\dfrac{1}{R_{\mathrm{ges}}} = \dfrac{1}{R_1} + \dfrac{1}{R_2} + \dfrac{1}{R_3} + \dfrac{1}{R_4} + \dots$

Using the rules for working with fractions, we can also write the expression for two resistors in parallel as:

$R_{\mathrm{ges}} = \dfrac{R_1 \cdot R_2}{R_1 + R_2}$

<tip>
In a series connection, the total resistance is always greater than the largest individual resistance. In a parallel connection, the total resistance is always smaller than the smallest individual resistance.
</tip>

---

[question:ED104]
[question:ED105]
[question:ED106]

<tip>
Take care that the resistances used in the calculation always have the same units. We always recommend converting to the base unit ($\unit{\ohm}$) where possible. If, for example, we connect a $\qty{1}{\kilo\ohm}$ and a $\qty{10}{\ohm}$ resistor in series, we calculate $\qty{1000}{\ohm} + \qty{10}{\ohm} = \qty{1010}{\ohm}$.
</tip>

---

Some of the questions contain resistor networks with both a series and a parallel connection. Here we proceed by first converting, for example, the parallel connection into an equivalent resistance, which we then combine with the third resistor connected in series. Or simply the other way round, whichever the circuit diagram suggests.

<tip>
[picture:305:e_tipp_aufgabe:Example circuit]

An important technique is "solving by inspection" ... take, for example, a circuit with a resistor $R_1$ in series with two resistors $R_2$ and $R_3$ connected in parallel. The values are $R_1 = \qty{1}{\kilo\ohm}$, $R_2 = \qty{2000}{\ohm}$ and $R_3 = \qty{2}{\kilo\ohm}$. But $\qty{2}{\kilo\ohm} = \qty{2000}{\ohm}$. The parallel connection of $R_2$ and $R_3$ gives a resistance half as large: $\qty{1000}{\ohm} = \qty{1}{\kilo\ohm}$. We put this in series with $R_1$ and get the result: $R_{\mathrm{ges}} = \qty{2}{\kilo\ohm}$.
</tip>

[question:ED111]
[question:ED110]
[question:ED112]
[question:ED113]
[question:ED108]
[question:ED109]

When considering power, it is best to start from the familiar expression for power:

$P = U \cdot I$

When, for example, three equal resistors are connected in series, the same current flows through all of them, but only a third of the external voltage is dropped across each one. In a parallel connection, all the resistors have the same voltage across them, but the current divides between three paths. In both cases, therefore, the circuit can handle three times the power of a single resistor.

[question:ED107]