A series connection of two resistors is often used as a potential divider. In Class E we first look at the *unloaded potential divider*, as it appears in the following questions. In an unloaded potential divider, the voltages are proportional to the resistances. This means, for example, that a larger voltage is dropped across a high-value resistor, while a correspondingly smaller voltage can be measured across a low-value resistor.

<margin>
[picture:819:E 63. Spannungsteiler:Potential divider]
</margin>

<indepth>
An important potential divider is found, for example, at the base of a transistor in an amplifier circuit. 
It is therefore called the base potential divider. We will look at this more closely in the chapter on amplifiers.
</indepth>

This relationship can be expressed in various formulas, which we find in the formula sheet:

$\frac{U_{1}}{U_{2}} = \frac{R_{1}}{R_{2}}$

or

$\frac{U_{2}}{U_g} = \frac{R_{2}}{R_{1} + R_{2}}$

% TODO implementiere Attention in CSS!
<danger>
These formulas do not apply to a loaded potential divider. Questions on it follow in Class A.
</danger>

The following questions do not mention the term potential divider directly, but the wording "How is the voltage divided between two resistors connected in series ..." should tell you that this is a potential divider.

[question:ED101]

No actual resistance values are given, so the result has to be stated as a general formula. 
According to the question, $R_1$ is 5 times as large as $R_2$, so a voltage 5 times as large must be measurable across it; in other words, $R_1 = 5 \cdot R_2$

This relationship can be written as a formula.

$\frac{U_{1}}{U_{2}} = \frac{5 \cdot R_2}{R_2}$

The $R_2$ terms cancel out, giving:

$\frac{U_{1}}{U_{2}} = \frac{5}{1}$

After a little rearranging we get the result:

$U_{1} = U_{2} \cdot \frac{5}{1}$

$U_{1} = 5 \cdot U_{2}$

[question:ED102]

This question has the reverse relationship to question ED 101. According to the question, $R_1$ is smaller than $R_2$ by a factor of 6, so the voltage measurable across it must also be smaller by a factor of 6. 

Expressed as a formula, this relationship is now:

$\frac{U_{1}}{U_{2}} = \frac{1}{6}$
  
$U_{1} = U_{2} \cdot {\frac{1}{6}}$
  
$U_1 = \frac{U_2}{6}$

[question:ED103]

In this question, actual resistance values are given, from which the divider ratio is found. $R_1$ is to $R_2$ as $\qty{10}{\kilo\ohm}$ is to $\qty{20}{\kilo\ohm}$, that is, $1$ to $2$. $U_2$ must therefore be twice as large as $U_1$. However, it is the total voltage $U_g$ that is given. It is applied across a total resistance of $\qty{30}{\kilo\ohm}$ and is therefore divided in the ratio $30$ to $20$ (or $3$ to $2$) with respect to $R_2$. So the voltage measurable across $R_2$ must be $2/3$ of $U_g$.

Of course, this result can also be calculated with the formula from the formula sheet:

$\frac{U_{2}}{U_g} = \frac{R_{2}}{R_{1} + R_{2}}$

and then rearranging it for $U_2$:

$U_{2} = \frac{R_{2}}{R_{1} + R_{2}} \cdot U_g$
