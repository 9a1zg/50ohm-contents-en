A *Lecher line*, as it is called, consists of two parallel conductors on which standing RF waves form through the superposition of the forward and reflected waves. It can be either open at the end (see Figure [ref:a_lecherleitung_offen]) or short-circuited (see Figure [ref:a_lecherleitung_kurzgeschlossen]). In both cases characteristic current and voltage distributions arise, which can be used, for example, to determine the wavelength.

<margin>
[picture:1112:a_lecherleitung_offen:Lecher line with an open end]
</margin>

On a Lecher line that is *open* at the end, no current can flow at the end of the line. There is therefore a current minimum there and, at the same time, a voltage maximum. From Ohm's law

$R=\frac{U}{I}$

it follows that the ratio of voltage to current at this point becomes, ideally, infinitely large, i.e. $R=\infty$. Along the line, current and voltage are displaced from each other in space by $\frac{\lambda}{4}$. At a distance of $\frac{\lambda}{4}$ from the open end of the line there is therefore a current maximum and, at the same time, a voltage minimum. Since the voltage there ideally tends to zero, Ohm's law correspondingly gives $R=0$. After each further $\frac{\lambda}{4}$, current maximum and voltage maximum alternate. After a distance of $\frac{\lambda}{2}$ the same current and voltage distribution is present again, as shown in Figure [ref:a_lecherleitung_offen].

---

On a Lecher line that is *short-circuited* at the end, the two conductors cannot have different voltages at the end of the line. There, therefore, $U=0$. There is a voltage minimum there and, at the same time, a current maximum. With $R=\frac{U}{I}$ this ideally gives $R=0$. At a distance of $\frac{\lambda}{4}$ from the short circuit, on the other hand, there is a voltage maximum and, at the same time, a current minimum. Since the current there ideally tends to zero, the ratio $\frac{U}{I}$ becomes very large, and ideally $R=\infty$. On the short-circuited Lecher line, too, current and voltage maxima alternate every $\frac{\lambda}{4}$. After a distance of $\frac{\lambda}{2}$ the same current and voltage distribution is present again, as shown in Figure [ref:a_lecherleitung_kurzgeschlossen].


<margin>
[picture:1111:a_lecherleitung_kurzgeschlossen:Lecher line with a short-circuited end]
</margin>

The frequency at which a Lecher line resonates depends mainly on its length. If the length of the line changes, the resonant frequency changes too.

[question:AG320]

With a line length of $\frac{\lambda}{2}$ the current and voltage distribution repeats completely. A load impedance at the end of the line therefore appears again at the input of the line with the same value.

A particularly important special case arises when the Lecher line has an electrical length of exactly $\frac{\lambda}{4}$ at the frequency under consideration. As we have seen from the current and voltage distributions, a current maximum and a voltage maximum swap places over a distance of $\frac{\lambda}{4}$. As a result, a high impedance is also transformed into a low impedance and vice versa.

On a $\frac{\lambda}{4}$ line that is *open* at the end, the impedance at the end of the line is, ideally, infinitely large. After a distance of $\frac{\lambda}{4}$, at the input of the line, there is on the other hand a voltage minimum and a current maximum. The input impedance is therefore almost zero ($Z_\mathrm{in} \approx \qty{0}{\ohm}$). An open end of a line is thus transformed approximately into a short circuit by a $\frac{\lambda}{4}$ long line.

---

[question:AG411]

Conversely, a line that is *short-circuited* at the end has an impedance of $\qty{0}{\ohm}$ at the end of the line. After a distance of $\frac{\lambda}{4}$, at the input of the line, there is a voltage maximum and a current minimum. The input impedance there therefore becomes very large ($Z_\mathrm{in} \rightarrow \infty$). A short circuit at the end of the line is thus transformed approximately into an open circuit by a $\frac{\lambda}{4}$ long line.

<indepth>
The behaviour of a $\frac{\lambda}{4}$ line can also be compared with tuned circuits. An open $\frac{\lambda}{4}$ line has a very low impedance at its input and behaves there much like a *series tuned circuit at resonance*. A short-circuited $\frac{\lambda}{4}$ line, on the other hand, has a very high impedance at its input and behaves much like a *parallel tuned circuit at resonance*.
</indepth>

In the next section we look at how $\frac{\lambda}{4}$ lines can be used to carry out specific impedance transformations.