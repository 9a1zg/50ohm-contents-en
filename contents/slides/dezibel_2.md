## Decibels

* Logarithmic way of stating ratios, especially of powers
* Makes working with small and large powers easier
* Gains and attenuations are easier to calculate

---

## Why decibels?

[picture:877:e_signalkette:Signal chain with three amplifiers]

[picture:1053:e_signalkette_2:Signal chain with two amplifiers and an attenuator]

--- style="font-size: 0.7em;"
## Power level

Factor 10

*Power relative to $\qty{1}{\milli\watt}$*
$p = 10\cdot \log_{10}\left(\frac{P}{\qty{1}{\milli\watt}}\right)\unit{\dBm}$
<fragment>
$\rightarrow\qty{0}{\dBm}$ corresponds to $P = \qty{1}{\milli\watt}$
</fragment>

<fragment>
*Power relative to $\qty{1}{\watt}$*
$p = 10\cdot \log_{10}\left(\frac{P}{\qty{1}{\watt}}\right)\unit{\dBW}$
</fragment>
<fragment>
$\rightarrow\qty{0}{\dBW}$ corresponds to $P = \qty{1}{\watt}$
</fragment>

---
[question:AD428]
---
#### Solution
* given: $P_1 = \qty{38}{\watt}$
* given: $P_2 = \qty{2.5}{\watt}$
* required: $g$

<fragment>
$\begin{split} g &= \qty{10\cdot \log_{10}{\left(\frac{P_2}{P_1}\right)}}{\dB}\\ &= \qty{10\cdot \log_{10}{\left(\frac{\qty{38}{\watt}}{\qty{2.5}{\watt}}\right)}}{\dB} = \qty{11.8}{\dB} \end{split}$
</fragment>

---
[question:AA110]
<note>
Just substitute the values
</note>
---
[question:AA105]

--- style="font-size: 0.7em;"

## Voltage level

Factor $20$

$u = 20\cdot \log_{10}\left(\frac{U}{\qty{0.775}{\volt}}\right)\unit{\dBu}$

<fragment>
*Voltage relative to $\qty{0.775}{\volt}$*
$\rightarrow\qty{0}{\dBu}$ corresponds to $U = \qty{0.775}{\volt}$
</fragment>
<fragment>
*Voltage relative to $\qty{1}{\volt}$*
$\rightarrow\qty{0}{\dBV}$ corresponds to $U = \qty{1}{\volt}$
</fragment>
<fragment>
*Voltage relative to $\qty{1}{\micro\volt}$*
$\rightarrow\qty{0}{\dBuV}$ corresponds to $U = \qty{1}{\micro\volt}$
</fragment>

<note>
Details of how the factor 20 is calculated are in the online course. In short: a voltage ratio is calculated with squares, and the square can be brought out in front of the logarithm as a factor.
</note>

---

[question:AD427]

---

#### Solution
* given: $U_1 = \qty{1}{\milli\volt}$
* given: $U_2 = \qty{4}{\milli\volt}$
* required: $g$

<fragment>
$\begin{split} g &= \qty{20\cdot \log_{10}{\left(\frac{U_2}{U_1}\right)}}{\dB}\\ &= \qty{20\cdot \log_{10}{\left(\frac{\qty{4}{\milli\volt}}{\qty{1}{\milli\volt}}\right)}}{\dB} = \qty{12}{\dB} \end{split}$
</fragment>

---

[question:AA111]

---

[question:AA108]

---

### Solution
* given: $p = \qty{20}{\dBW}$
* required: $P$

<fragment>
$\begin{split} p &= 10\cdot \log_{10}\left(\frac{P}{\qty{1}{\watt}}\right)\unit{\dBW}\\ \Rightarrow P &= 10^{\frac{p}{10}} \cdot \qty{1}{\watt} = 10^{\frac{\qty{20}{\dBW}}{10}} \cdot \qty{1}{\watt} = \qty{10^2}{\watt} \end{split}$
</fragment>
---
[question:AA107]
---
[question:AA109]
---
### Solution

$\qty{1}{\watt} = \qty{1000}{\milli\watt}$
$\qty{10}{\dB} = \text{factor 10}$
$\qty{1000}{\milli\watt} \cdot 10 = \qty{10000}{\milli\watt} = \qty{40}{\dBm}$
---
[question:AA106]
---
## Solution
* $\qty{16}{\dB} = \qty{10}{\dB} + \qty{6}{\dB} = 10 \cdot 4 = 40$
* $\qty{1}{\watt} \cdot 40 = \qty{40}{\watt}$

<note>
From the table in the formula sheet
</note>

---
[question:AD426]
---
#### Solution
* given: $g = \qty{16}{\dB}$
* given: $P_1 = \qty{1}{\watt}$
* required: $P_2$

<fragment>
$g = \qty{16}{\dB} = \qty{10}{\dB} + \qty{6}{\dB} = 10 \cdot 4 = 40$
</fragment>
<fragment>
$P_2 = P_1 \cdot g = \qty{1}{\watt} \cdot 40 = \qty{40}{\watt}$
</fragment>

---
[question:AA112]
---
### Solution
* given: $u = \qty{120}{\dBuV\per\meter}$
* required: $U$

<fragment>
$\begin{split} u &= 20\cdot \log_{10}\left(\frac{U}{\qty{1}{\micro\volt}}\right)\unit{\dBuV}\\ \Rightarrow U &= 10^{\frac{u}{20}} \cdot \qty{1}{\micro\volt} = 10^{\frac{\qty{120}{\dBuV\per\meter}}{20}} \cdot \qty{1}{\micro\volt} = \qty{1}{\volt\per\meter} \end{split}$
</fragment>
<fragment>
The literature often gives: $\qty{120}{\dBuV} = \qty{1}{\volt}$
</fragment>
