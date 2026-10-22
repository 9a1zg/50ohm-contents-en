In many applications, capacitors are used in series, in parallel or in series-parallel combinations. The parallel connection is easier to understand, so we look at it first.

Connecting capacitors in parallel means that more plates face each other, so the plate area increases proportionally. The capacitance of the circuit as a whole increases accordingly.

<margin>
[picture:822:e_3C-parallel: Parallel connection of 3 capacitors]
</margin>

---

When capacitors of equal value are connected in parallel, the capacitance doubles while the voltage rating stays the same. Of course, the total capacitance can be calculated. The formula is in the formula sheet:

$C_{\mathrm{ges}} = C_{1} + C_{2} + C_{3} + \dots$

<tip>
In a parallel connection, the total capacitance is always greater than the smallest individual capacitance.
</tip>

The following question has an additional difficulty, because the capacitance values have different prefixes. First, all the values have to be converted to a common prefix. The numbers should be neither too large nor too small, so it is best to choose the prefix nano ($\unit{\nano}$). 

$\begin{split} \qty{0.1}{\micro\farad} &= \qty{100}{\nano\farad} \\ \qty{50000}{\pico\farad} &= \qty{50}{\nano\farad}\end{split}$

Now all you have to do is add up all the values in $\unit{\nano\farad}$.

[question:ED117]

<margin>
[photo:262:a_Netzteil BEKO PA $7 \times \qty{10000}{\micro\farad}$ parallel: $7 \times \qty{10000}{\micro\farad}$ connected in parallel in the power supply of a power amplifier]
</margin>

The next question can be used to test your understanding.

[question:ED118]


---

When capacitors are connected in series, as shown in Figure [ref:e_3C-parallel], the voltage rating increases, but the capacitance decreases. Of course, the total capacitance can again be calculated. The calculation is very similar to that for resistors in parallel:

$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{C_{1}} + \frac{1}{C_{2}} + \frac{1}{C_{3}}$

<margin>
[picture:823:e_3C-parallel:Series connection of 3 capacitors] 
</margin>

<tip>
In a series connection, the total capacitance is always smaller than the smallest individual capacitance.
</tip>

<tip>
The following approach is recommended for solving the questions:
  
1. Sketch the circuit
2. Write the capacitance values next to the components.
3. Convert to the same prefixes.
4. Simplify the circuit by combining groups of the same kind
5. Calculate the total capacitance step by step
</tip>

If all the capacitors have the same capacitance, the total capacitance is easy to calculate by dividing one individual capacitance by 3. In the following question, the calculation is $\qty{0.33}{\micro\farad} / 3 = \qty{0.11}{\micro\farad}$.

[question:ED119]

In the series connection of capacitors in the following question, you find $\unit{\micro\farad}$ and $\unit{\nano\farad}$ as prefixes. It makes good sense to convert $\qty{200000}{\nano\farad}$ to $\qty{200}{\micro\farad}$ first. For a series connection, you can now apply the formula from the formula sheet.


$C_{\mathrm{ges}} =\frac{1}{\frac{1}{\qty{100}{\micro\farad}} + \frac{1}{\qty{200}{\micro\farad}} + \frac{1}{\qty{200}{\micro\farad}}}$

[question:ED120]

---
  
In the next question, 3 capacitors are combined in series and in parallel. 

[question:ED121]

Which part of the circuit can be simplified first? Correct: the series connection.
This group has a total capacitance of half of $\qty{10}{\nano\farad}$, i.e. $\qty{5}{\nano\farad}$. Now it is easier to continue, since in a parallel connection the capacitance values are added. Congratulations on the result of $\qty{10}{\nano\farad}$.

The other questions are similar and easy to solve.

[question:ED122]
[question:ED123]
[question:ED124]

%<margin>
%
%Lösungshilfen:
%
%*ED 118:* Reihenschaltung von $\qty{22}{\nano\farad}$, $\qty{0,033}{\micro\farad} = \qty{33}{\nano\farad}$ und $\qty{15000}{\pico\farad} = \qty{15}{\nano\farad}$.
%$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{\qty{22}{\nano\farad}} + \frac{1}{\qty{33}{\nano\farad}} + \frac{1}{\qty{15}{\nano\farad}}$
%Eigentlich muss man nicht rechnen, denn es gibt nur ein Ergebnis, das kleiner als $\qty{15}{\nano\farard}$ ist.
%*ED 120:* $\qty{50}{\micro\farad}$ 
%*ED 122:* $C_2 = \qty{1}{\micro\farad}$ und $C_3 = \qty{1}{\micro\farad}$ in Parallelschaltung ergibt zusammen $\qty{2}{\micro\farad}$. Dazu $C_1 = \qty{2}{\micro\farad}$ in Reihe %ergibt die Hälfte , also $\qty{1}{\micro\farad}$.
% 
%*ED 123:* $C_2 = \qty{4}{\nano\farad}$ und $C_3 = \qty{4}{\nano\farad}$ in Parallelschaltung ergibt zusammen $\qty{8}{\nano\farad}$. Dazu $C_1 = \qty{8}{\nano\farad}$ in Reihe %ergibt die Hälfte , also $\qty{4}{\nano\farad}$.
%  
%*ED 124:* $C_2 = \qty{100}{\nano\farad}$ und $C_3 = \qty{100000}{\pico\farad} = \qty{100}{\nano\farad}$ in Parallelschaltung ergibt zusammen $\qty{200}{\nano\farad}$. Dazu %$C_1 = \qty{200}{\nano\farad}$ in Reihe ergibt die Hälfte , also $\qty{100}{\nano\farad}$.
%</margin>
