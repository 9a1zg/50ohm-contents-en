In digital transmission, information is transmitted in the form of symbols. A symbol is a distinguishable signal state that is transmitted for a certain time. These signal states can differ, for example, in their amplitude, frequency or phase, or in combinations of these properties. How such symbols are generated is something we will look at in the following sections. Depending on how many different symbols a transmission method can use, a single symbol can contain one or more bits of information.

If only two different symbols are available, exactly one bit can be transmitted with each symbol. With four possible symbols, two bits can already be transmitted with one symbol, since two bits can represent four different combinations. Correspondingly, eight different symbols can transmit three bits and $\num{16}$ different symbols four bits at once.

In general, the number $N$ of bits that can be transmitted with one symbol follows from the number $M=2^N$ of possible symbols:

$N = \log_2(M)$

The *symbol rate* indicates how many symbols are transmitted per second. Its unit is the *baud*. A symbol rate of $\qty{1000}{\baud}$ therefore means that $\num{1000}$ symbols are transmitted per second.

The symbol rate is not necessarily the same as the data rate. If several bits are transmitted with each symbol, the data rate is correspondingly higher. For the data rate $R_\mathrm{D}$ (with the unit $\unit{\bit\per\second}$) and the symbol rate $R_\mathrm{S}$:

$R_\mathrm{D} = R_\mathrm{S} \cdot N$

If, for example, two bits are transmitted with each symbol at a symbol rate of $\qty{1200}{\baud}$, the data rate is:

$R_\mathrm{D} = \qty{1200}{\baud} \cdot \qty{2}{\bit\per{symbol}} = \qty{2400}{\bit\per\second}$

The number of possible symbols and the symbol rate are therefore important quantities for digital transmission methods. How the individual symbols can be represented by different properties of a signal is something we will look at in the following sections.

[question:AA104]

---

A simple example of how different symbols can be represented by different signal states is *frequency-shift keying* (FSK), already familiar from Class E.

In FSK, the frequency of the transmitted signal is switched between different values. Figure [ref:a_fsk] shows binary FSK with two possible symbol frequencies in the time domain. For example, the higher frequency can stand for the symbol $1$ and the lower frequency for the symbol $0$. Since two different symbols are available, one bit can be transmitted with each symbol.

<margin>
[picture:703:a_fsk:FSK (frequency-shift keying)]
</margin>

One example is *RTTY*. Here the signal is shifted between two symbol frequencies, for example between $\qty{14072.43}{\kilo\hertz}$ and $\qty{14072.60}{\kilo\hertz}$. One bit, that is, $0$ or $1$, can therefore be transmitted with each symbol.

[question:AE405]

FSK is not, however, limited to two symbol frequencies. If, for example, four different frequencies are used, four different symbols are available. Each symbol can then be assigned one of the four possible bit combinations $00$, $01$, $10$ or $11$. As a result, two bits can be transmitted with each symbol.

One example of this is the *FT4* transmission method. Here the signal can be shifted between four symbol frequencies, for example $\qty{14081.20}{\kilo\hertz}$, $\qty{14081.40}{\kilo\hertz}$, $\qty{14081.61}{\kilo\hertz}$ and $\qty{14081.83}{\kilo\hertz}$.

[question:AE406]