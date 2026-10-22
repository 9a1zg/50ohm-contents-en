We have already met the three most important quantities in electrical engineering, namely electric voltage, electric current and resistance:
* First we learnt that electric charges are separated in voltage sources, and that this produces an electric voltage. We denote it by the letter $U$ and measure it in volts ($\unit{V}$).
* Then we learnt that the electric voltage causes an electric current to flow in a closed circuit; we denote the current by the letter $I$ and measure it in amperes ($\unit{A}$).
* And at the beginning of this chapter we then learnt that loads in a circuit present a resistance and so slow down the flow of current. We denote resistance by the letter $R$ and measure it in ohms ($\unit{\ohm}$).

%<margin>
%[p-h-o-t-o:147:ohmsches_gesetz_comic:Bildhafte Darstellung der Zusammenhänge des Ohmschen Gesetzes]
%</margin>

[question:NA203]

---

But how are these three quantities related? Let us look at an example in Figure [ref:n_ohmsches_gesetz_stromkreis_mit_batterie]. We have a circuit consisting of a battery as the voltage source and a resistor. We know the voltage and we can measure the current. The battery has a voltage of $\qty{10}{\volt}$, and a current of $\qty{1}{\milli\ampere}$ flows.

<margin>
[picture:664:n_ohmsches_gesetz_stromkreis_mit_batterie:Circuit with a battery]
</margin>

If the $\qty{10}{\volt}$ battery in the example were replaced by a $\qty{20}{\volt}$ battery, the current would also increase, from $\qty{1}{\milli\ampere}$ to $\qty{2}{\milli\ampere}$. So if you double the voltage, the current doubles too. Correspondingly, the current would halve to $\qty{0.5}{\milli\ampere}$ if the voltage were halved to $\qty{5}{\volt}$.

We can see a pattern: in our example, the voltage $U$ in volts is always 10000 times the current $I$ in amperes. Or, expressed mathematically:

$\dfrac{U}{I} = \dfrac{\qty{10}{\volt}}{\qty{0.001}{\ampere}} = \dfrac{\qty{20}{\volt}}{\qty{0.002}{\ampere}} = \dfrac{\qty{5}{\volt}}{\qty{0.0005}{\ampere}} = 10000 \frac{\unit{\volt}}{\unit{\ampere}}$

---

In technical language this is called proportionality: $I$ is proportional to $U$. Leaving the units aside for a moment, the *constant of proportionality* in our example is 10000: multiply the one value by 10000 and you get the other.
%Dieses Verhalten kann man sich auch wieder am Wasserkreislauf vorstellen: Wenn die Pumpe mit mehr Druck pumpt, wird auch mehr Wasser durch den Kreislauf fließen.

<indepth>
The *constant of proportionality* is the numerical ratio of two quantities that are proportional to each other.
</indepth>

One question remains, though. Where does this factor of 10000 come from? The answer is simple: it is our resistance $R$! And if we now also look at the units, the whole picture comes together: the unit ohm is defined so that $\qty{1}{\ohm}$ is the same as $\qty{1}{\volt\per\ampere}$. So instead of $\qty{10000}{\volt\per\ampere}$ we may simply write $\qty{10000}{\ohm}$! Our resistance is therefore $\qty{10000}{\ohm}$, or $\qty{10}{\kilo\ohm}$ for short:

$\qty{10000}{\volt\per\ampere} = \qty{10000}{\ohm}$

%Es stellt sich aber immer noch folgende Frage: Warum fließen in unserem Beispiel genau $\qty{1}{\milli\ampere}$, wenn die Spannung $\qty{10}{\volt}$ beträgt? Die Höhe des Stroms hängt vom Wert des Widerstands ab. Ist der Widerstand groß, so wird der Strom klein sein, ist der Widerstand hingegen klein, dann wird der Strom groß sein.

We have learnt that the value of the resistance can be calculated from the voltage and the current. It is the *ratio of voltage to current*, or, put another way: if you divide the voltage by the current, you get the value of the resistance.

---

This relationship can be expressed by the following formula, which is known as *Ohm's law*: 

$ R = \dfrac{U}{I} $

<person>
The German physicist *Georg Simon Ohm* discovered the relationship between electric voltage, electric current and resistance in 1826. In his honour, the formula $ R = \frac{U}{I} $ is called Ohm's law.
</person>

[question:NB505]

If, however, you know only the resistance and the voltage and want to calculate the corresponding current, you can use Ohm's law as follows: 

$ I = \dfrac{U}{R} $

If you know only the resistance and the current and want to calculate the corresponding voltage, there is another version of the formula: 

$ U = R\cdot I $

[question:NB504]

You do not necessarily have to memorise these formulas. They can also be found on the formula sheet that is provided as an aid in the examination. You may use a calculator for the calculations in the examination.

[question:NB502]
[question:NB503]
[question:NB501]
