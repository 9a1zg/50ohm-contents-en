---

### Symbol
* A *symbol* is a distinguishable signal state.
* Symbols can differ, e.g. in amplitude, frequency or phase.
* More possible symbols allow more bits per symbol.

---

### Symbol rate
* The *symbol rate* gives the number of symbols transmitted per second; the unit of the symbol rate is the *baud*
* Data rate and symbol rate are therefore not always the same.
* If only two symbols are used, so that each bit is sent on its own, the symbol rate in baud equals the data rate in $\unit{\bit\per\second}$.
* If, however, more symbols are used, so that several bits are transmitted at once, the data rate is higher than the symbol rate.

---

**Examples**

* 2 symbols → 1 bit/symbol
* 4 symbols → 2 bits/symbol
* 8 symbols → 3 bits/symbol

---

* The formula $R_\mathrm{D} = R_\mathrm{S} \cdot N$ expresses the relationship:

<fragment>
* $R_\mathrm{D}$ → data rate in $\unit{\bit\per\second}$
* $R_\mathrm{S}$ → symbol rate in $\unit{\baud}$
* $N$ → symbol size in $\unit{\bit\per\text{symbol}}$
</fragment>

---

[question:AA104]

---

Examples:

<fragment>
*RTTY*: switching between two symbol frequencies, so that one bit ($\num{0}$ or $\num{1}$) can be transmitted per symbol.
→ data rate = symbol rate
</fragment>

<fragment>
*FT4*: switching between four symbol frequencies, so that two bits ($\num{00}$, $\num{01}$, $\num{10}$ or $\num{11}$) can be transmitted per symbol.
→ data rate = 2 $\cdot$ symbol rate
</fragment>

---

[question:AE405]

---

#### Solution
* given: $R_S = \qty{45.45}{\baud}$
* given: $N=\qty{1}{\bit\per\text{symbol}}$
* required: $R_\mathrm{D}$

<fragment>
$R_\mathrm{D} = R_\mathrm{S} \cdot N = \qty{45.45}{\baud} \cdot \qty{1}{\bit\per\text{symbol}} = \qty{45.45}{\bit\per\second}$
</fragment>

---

[question:AE406]

---

#### Solution
* given: $R_S = \qty{23.4}{\baud}$
* given: $N=\qty{2}{\bit\per\text{symbol}}$
* required: $R_\mathrm{D}$

<fragment>
$R_\mathrm{D} = R_\mathrm{S} \cdot N = \qty{23.4}{\baud} \cdot \qty{2}{\bit\per\text{symbol}} = \qty{46.8}{\bit\per\second}$
</fragment>