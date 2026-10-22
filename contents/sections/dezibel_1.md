Power ratios play an important part in many areas of radio-frequency engineering, for example in the gain of an antenna or an amplifier, or in the loss of a cable. In Class N we met these relationships only in the form of simple factors, for example: "The antenna has a gain of a factor of $2$".

These ratios can take very large or very small numerical values. For example, an HF receiver has an overall gain factor of $\num{1000000000000}$, that is, a one followed by twelve zeros. With numbers like these, calculations quickly become hard to follow, and you inevitably start counting the zeros.

Put simply, however, there is a mathematical tool for this "counting of zeros": logarithms. With their help, multiplications can also be turned into additions and divisions into subtractions. That makes calculating with large numbers very easy. 

---

It has therefore become customary to state power ratios on a logarithmic scale.
Taking the logarithm is the inverse operation of raising to a power. In amateur radio we generally use the common logarithm ("base-ten logarithm") to base $10$:

---

$a =\log_{10} (b)$, if $b=10^{a}$

The logarithm of $100$ is $\log_{10}(100)=2$, because $10^2 = 100$. In other words: the number $100$ has two zeros.

<warning>
Besides the common logarithm (labelled $\lg$ or $\log$), a scientific calculator also offers the natural logarithm *$\ln$*, whose base is Euler's number *$e=\num{2.7182818}\dots$*. Do not mix them up!
</warning>	

<margin>
| c:dB | c:≈ Power ratio |
| $0$ | $1$ |
| $1.5$ | $\sqrt{2} = 1.41$ |
| $2.15$ | $1.64$ |
| $3$ | $2$ |
| $5$ | $\sqrt{10} = 3.16$ |
| $6$ | $4$ |
| $10$ | $10$ |
| $20$ | $100$ |
[table:e_dezibel_leistungsfaktoren:Important power ratios in $\unit{\dB}$]
</margin>

The *bel* ($\unit{\bel}$) is derived from the common logarithm. Its name honours the American teacher of the deaf and telephone pioneer *Alexander Graham Bell*. In the example above we could also have written:

$\log_{10}(b)=\qty{a}{\bel}$

As a rule, the *decibel* (unit symbol $\unit{\dB}$), that is, a tenth of a bel, is used instead of the bel:

$10 \cdot \log_{10}(b) = \qty{a}{\dB}$

---

For converting a power ratio, the formula sheet gives the following formula:

$g = 10\cdot \log_{10}\left(\frac{P_2}{P_1}\right)\unit{\dB}$

where $P_1$ is the input power and $P_2$ the output power. Now let us assume we have an amplifier that amplifies the input power $P_1=\qty{50}{\watt}$ to $P_2=\qty{100}{\watt}$, that is, doubles it. Our formula then gives the following gain in $\unit{\dB}$:

$g = 10\cdot \log_{10}\left(\frac{\qty{100}{\watt}}{\qty{50}{\watt}}\right)\unit{\dB} = 10\cdot \log_{10}\left(2\right)\unit{\dB} = 10\cdot \qty{0.301}{\dB} \approx \qty{3}{\dB} $

For Class E it is enough, to begin with, to know the decibel value for a power ratio of $2$. The formula sheet contains a table for this, which is also shown in Table [ref:e_dezibel_leistungsfaktoren]. From it you can read off that a power ratio of $2$ corresponds to a decibel value of $\qty{3}{\dB}$. Calculating with decibel values in detail is only covered in Class A.

<tip>
Decibel values that end in "$0$" can be estimated without any calculator at all: just cover up the last zero, and the digit then gives the number of zeros in the ratio. Example: $\qty{30}{\dB} \rightarrow 3 \rightarrow 3~\text{zeros} \rightarrow \text{ratio}~1000$!
</tip>

[question:EA107]

Besides the unit $\unit{dB}$, in practice you will often also come across values such as $\unit{\dBi}$, $\unit{\dBm}$, $\unit{\dBW}$ or $\unit{\dBu}$. These additions indicate which reference quantity the decibel value in question refers to. In Class E we will meet $\unit{\dBi}$ and $\unit{\dBd}$ in particular, for antennas, in the antenna chapter. The others, such as $\unit{\dBm}$ and $\unit{\dBW}$, are only needed for Class A.