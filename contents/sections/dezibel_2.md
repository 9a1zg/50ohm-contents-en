In Class E we already met the decibel as a tool for describing ratios, and saw that a change in power of $\qty{3}{\dB}$ corresponds to a power ratio of $\num{2}$. In the formula sheet we find Table [ref:a_dezibel_leistungsfaktoren], which contains further important equivalents. 

<margin>
| c:dB | c:≈ Power ratio |
| $-20$ | $\num{0.01}$ |
| $-10$ | $\num{0.1}$ |
| $-6$ | $\num{0.25}$ |
| $-3$ | $\num{0.5}$ |
| $-1$ | $\num{0.79}$ |
| $0$ | $\num{1}$ |
| $1.5$ | $\sqrt{2} = \num{1.41}$ |
| $2.15$ | $\num{1.64}$ |
| $3$ | $\num{2}$ |
| $5$ | $\sqrt{10} = \num{3.16}$ |
| $6$ | $\num{4}$ |
| $10$ | $\num{10}$ |
| $20$ | $\num{100}$ |
[table:a_dezibel_leistungsfaktoren:Important power ratios in $\unit{\dB}$]
</margin>

For converting a power ratio into $\unit{\dB}$, the formula sheet gives the following formula, which we already met in Class E. The ratio $g$ of two powers $P_1$ and $P_2$ in $\unit{\dB}$ is:

$g = 10\cdot \log_{10}\left(\frac{P_2}{P_1}\right)\unit{\dB}$

[question:AD428]

To obtain a ratio from a $\unit{\dB}$ value, the formula has to be rearranged: 

$\begin{align*} g &= 10 \cdot \log_{10}\left( x \right) \unit{\dB} & \quad\quad\quad &|: \qty{10}{\dB} \\ \frac{g}{\qty{10}{\dB}} &= \log_{10}\left( x \right) &~&| \quad 10^{x}\\ x &= 10^{\frac{g}{\qty{10}{\dB}}} &~&~\end{align*}$

With these two formulas we can therefore easily convert between $\unit{\dB}$ values and ratios. Now try to work out the following three questions: 

---

[question:AA105]
[question:AA106]
[question:AD426]

<tip>
In Class E we already learnt the following trick: decibel values that end in "$0$" can be estimated without any calculator at all: just cover up the last zero, and the digit then gives the number of zeros in the ratio. Example: $\qty{30}{\dB} \rightarrow 3 \rightarrow 3~\text{zeros} \rightarrow \text{ratio}~1000$!

It is just as easy the other way round: a one followed by $12$ zeros ($\num{1000000000000}$) in $\unit{\dB}$ is simply the number of zeros, i.e. $12$, multiplied by $10$. This gives a gain of $\qty{120}{\dB}$.

But even for $\unit{\dB}$ values that do not end in $0$, the corresponding factor can be found by splitting them up:

* $\qty{9}{\dB}$ can be split into $\qty{6}{\dB} + \qty{3}{\dB}$, which corresponds to a multiplication $4\cdot 2 = 8$. 
* Which factor corresponds to a power ratio of $\qty{17}{\dB}$? $\qty{17}{\dB} = \qty{20}{\dB} - \qty{3}{\dB}$, so a factor of $100$ divided by $2$, which is $50$.
</tip>

The decibel ($\unit{\dB}$) basically describes a dimensionless ratio, for example of powers or voltages. That is why $\unit{\dB}$ is used above all to state gains and attenuations. In these cases no further addition is needed, since only the ratio of two quantities is being stated. Negative decibel values, by the way, indicate ratios smaller than $1$. For example, $\qty{-3}{\dB}$ corresponds to a ratio of $\frac{1}{2} = \num{0.5}$.

Decibel values can also be used to state an absolute level, however. This requires a fixed reference quantity $P_0$:

$p = 10\cdot \log_{10}\left(\frac{P}{P_0}\right)\unit{\dB}$

---

This reference quantity can be, for example, a power of $\qty{1}{\milli\watt}$. In this case the decibel value gets a corresponding addition: if the level is relative to $\qty{1}{\milli\watt}$, we speak of $\unit{\dBm}$. This makes it unambiguous which absolute power value the decibel level refers to.

If, for example, you come across the statement "The transmitter has an output power of $\qty{20}{\dBm}$", this value can easily be converted into milliwatts. A level of $\qty{20}{\dB}$ corresponds to a power ratio of $100$ (that is, two zeros). This factor is multiplied by the reference quantity of $\qty{1}{\milli\watt}$:

$ P = 100 \cdot \qty{1}{\milli\watt} = \qty{100}{\milli\watt}$

Table [ref:a_bezugsgroessen] lists the most important reference quantities and their $\unit{\dB}$ abbreviations.

<margin>
| l: Abbreviation         | X: Reference value     |
| $\unit{\dBm}$           | $\qty{1}{\milli\watt}$ | 
| $\unit{\dBW}$           | $\qty{1}{\watt}$       | 
| $\unit{\dBu}$           | $\qty{0.775}{\volt}$   | 
| $\unit{\dB\micro\volt}$ | $\qty{1}{\micro\volt}$ | 
[table:a_bezugsgroessen:Important reference quantities from the formula sheet]
</margin>

The following questions can be worked out with the formula from the formula sheet and its rearrangement from the beginning of this lesson, provided the right reference quantity is used. 

[question:AA109]
[question:AA110]
[question:AA107]
[question:AA108]

---

Why do we do all this at all, and state absolute powers in $\unit{\dBm}$ and $\unit{\dBW}$? As already hinted at in Class E, the main purpose of using decibels is to simplify calculations. By expressing gains and attenuations in decibels, complete signal chains can be estimated very easily by addition and subtraction, without having to resort to cumbersome multiplications and divisions.

Figure [ref:e_signalkette] shows such a signal chain with three amplifier stages. The input signal has a power of $\qty{1}{\milli\watt}$, which corresponds to $\qty{0}{\dBm}$. The three amplifier stages amplify the signal to a total of $\qty{60}{\dBm}$ (that is, $\num{1000000}\cdot \qty{1}{\milli\watt}$), which corresponds to a power of $\qty{1000}{\watt}$.

Figure [ref:e_signalkette_2] shows another example of a signal chain, in which an attenuator with an attenuation of $\qty{20}{\dB}$ is also used, which corresponds to a gain of $\qty{-20}{\dB}$. The input signal has a power of $\qty{1}{\milli\watt}$, i.e. $\qty{0}{\dBm}$. The first amplifier stage raises the signal to $\qty{10}{\dBm}$. The attenuator then reduces it to $\qty{-10}{\dBm}$, and finally the second amplifier stage amplifies it back to $\qty{0}{\dBm}$, which again corresponds to $\qty{1}{\milli\watt}$.

<margin>
[picture:877:e_signalkette:Signal chain with three amplifiers]
[picture:1053:e_signalkette_2:Signal chain with two amplifiers and an attenuator]
</margin>

<indepth>
Why is it allowed to subtract an attenuation of $\qty{3}{\dB}$ from a level of $\qty{9}{\dBm}$? After all, the two values have different units! The bel ($\unit{\bel}$) and the decibel ($\unit{\dB}$) are an auxiliary unit (also called a pseudo-unit).
In principle, the numerical value could also be written without the unit $\unit{\dB}$. But adding $\unit{\dB}$ makes it clear that we are dealing with a logarithmic ratio of two quantities. Without this unit, you would have to describe in words what the numerical value means.
</indepth>

To find the total gain of a multi-stage power amplifier, the difference between output and input power has to be taken by subtracting the dBm values with their correct signs. Example: an input power of $\qty{-5}{\dBm}$ and an output power of $\qty{20}{\dBm}$ give a total gain of $\qty{25}{\dB}$ ($\qty{20}{\dBm} - (\qty{-5}{\dBm}) = \qty{25}{\dB}$)

[question:AF428]
  
In Class E we also already met the additions $\unit{\dBd}$ and $\unit{\dBi}$, which are used when stating antenna gains. In this case the decibel value does not refer to a power or a voltage, but to a particular reference radiator. The usual ones are $\unit{\dBi}$, relative to the isotropic radiator, and $\unit{\dBd}$, relative to the half-wave dipole.

---

Besides power ratios, we can also use the decibel to state *voltage ratios* and *voltage levels*. For this we can use the formula $P = \frac{U^2}{R}$. So we can write:

$\begin{split}g &= 10 \cdot \log_{10}\left(\frac{P_1}{P_2}\right)\\ g &= 10 \cdot \log_{10}\left(\frac{\frac{U_1^2}{\cancel{R}}}{\frac{U_2^2}{\cancel{R}}}\right)\\ g &= 10 \cdot \log_{10}\left(\left(\frac{U_1}{U_2}\right)^2\right) \end{split}$

<tip>
*Calculating with logarithms:*
A few simple rules make it possible to solve decibel problems without a calculator.

* The logarithm of the product of two numbers equals the sum of the logarithms: $\log_{10}(a\cdot b) = \log_{10}(a)+ \log_{10}(b)$
* The logarithm of the quotient of two numbers equals the difference of the logarithms: $\log_{10}(a / b) = \log_{10}(a) - \log_{10}(b)$
* The logarithm of a squared number: $\log_{10}(x^2)= 2 \cdot \log_{10}(x)$
* The logarithm of a square root: $\log_{10}(\sqrt{x})= \frac{1}{2} \cdot \log_{10}(x)$
</tip>

But the logarithm of a squared number is equal to twice the logarithm of the number:

$\log_{10}(x^2)=2 \cdot \log_{10}(x)$

It follows that:

$\begin{split} g &= 10 \cdot \log_{10}\left(\left(\frac{U_1}{U_2}\right)^2\right)\\ g &= 10 \cdot 2 \cdot \log_{10}\left(\frac{U_1}{U_2}\right) \\ g &= 20 \cdot \log_{10}\left(\frac{U_1}{U_2}\right) \end{split}$

---

So we calculate a ratio *$a$* of two voltages $U_1$ and $U_2$ by multiplying the logarithm of the ratio not by a factor of $10$ but by a factor of $20$. This formula can also be found in the formula sheet.

[question:AA111]
[question:AD427]

<attention>
In decibel calculations, always check carefully whether you are dealing with power ratios or voltage ratios!
</attention>

To determine voltage levels, we again first have to fix a reference voltage (see Table [ref:a_bezugsgroessen]). For received signals, we like to measure the (very small) voltages at the receiver input in $\unit{\micro\volt}$. The corresponding voltage level then has the unit $\unit{\dBuV}$. Example:

$\qty{10}{\micro\volt} \rightarrow 20 \cdot \log_{10}\left(\frac{\qty{10}{\micro\volt}}{\qty{1}{\micro\volt}}\right)=\qty{20}{\dBuV}$

---

In the following question the reference value is $\qty{1}{\micro\volt\per\meter}$. Try to solve the question with what you know.

<attention>
Note: what is meant here is $\unit{\dB(\micro\volt\per\meter)}$, not $\unit{(\dB\micro\volt)/\meter}$! 
</attention>

[question:AA112]

<tip>
With voltages, too, a lot can be worked out in your head with the help of the table from the formula sheet:

| c:dB | c:≈ Voltage ratio |
| $-20$ | $\num{0.1}$ |
| $-10$ | $\num{0.32}$ |
| $-6$ | $\num{0.5}$ |
| $-3$ | $\num{0.71}$ |
| $-1$ | $\num{0.89}$ |
| $0$ | $\num{1}$ |
| $1$ | $\num{1.12}$ |
| $3$ | $\num{1.14}$ |
| $6$ | $2$ |
| $10$ | $3.16$ |
| $20$ | $10$ |
[table:a_spannungsverhaeltnisse:Important voltage ratios in $\unit{\dB}$]

*Example:*

* How many $\unit{\dB}$ does a voltage ratio of $4$ correspond to? $4 = 2 \cdot 2 \rightarrow \qty{6}{\dB} + \qty{6}{\dB} = \qty{12}{\dB}$
</tip>