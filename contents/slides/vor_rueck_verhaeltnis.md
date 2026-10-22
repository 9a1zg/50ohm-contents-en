--- style="font-size: 0.7em;"

## Antenna characteristics and directional properties

<left>
[picture:264:a_strahlungscharakteristik_dipol_richt:Radiation pattern of a directional antenna compared with a dipole]
* The *front-to-back ratio* describes how much better the antenna transmits and receives in the direction of maximum radiation.
</left>
<right>
* Directional antennas also transmit and receive in the backward direction – an unwanted effect.  
* The antenna gain refers only to the direction of maximum radiation (compared with a dipole or an isotropic radiator).  
</right>

---

[question:AG214]

---

[question:AG213]

---

### Front-to-back ratio in decibels

<left>
[picture:263:a_strahlungscharakteristik_richt:Radiation pattern of a directional antenna]
</left>
<right>
* The front-to-back ratio is often given in decibels.
</right>

---

[question:AG217]

---
#### Solution
* given: $P_R = \qty{0.6}{\watt}$
* given: $P_V = \qty{15}{\watt}$
* required: $\frac{Front}{Back}$

<fragment>
$\begin{split}\frac{Front}{Back} &= 10 \cdot \log_{10}{\left(\frac{P_V}{P_R}\right)} \unit{\dB}\\ &= 10 \cdot \log_{10}{\left(\frac{\qty{15}{\watt}}{\qty{0.6}{\watt}}\right)} \unit{\dB}\\ &= \qty{14}{\dB}\end{split}$
</fragment>

---

[question:AG215]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $g_D= \qty{10}{\dB}$
* given: $\frac{Front}{Back} = \qty{20}{\dB}$
</left>
<right>
* given: $P_S = \qty{100}{\watt}$
* required: $P_R$
</right>

<left>
<fragment>
$\begin{split}P_V &= P_{ERP}\\ &= P_S \cdot 10^{\frac{g_d}{\qty{10}{\dB}}}\\ &= \qty{100}{\watt} \cdot 10^{\frac{\qty{10}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{1000}{\watt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\qty{20}{\dB} &= 10 \cdot \log_{10}{\left(\frac{P_V}{P_R}\right)} \unit{\dB}\\ \Rightarrow \frac{P_V}{P_R} &= 10^{\frac{\qty{20}{\dB}}{\qty{10}{\dB}}}\\ &= 100\\ \Rightarrow P_R &= \frac{P_V}{100}\\ &= \frac{\qty{1000}{\watt}}{100}\\ &= \qty{10}{\watt}\end{split}$
</fragment>
</right>
---

[question:AG216]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $g_D= \qty{15}{\dB}$
* given: $\frac{Front}{Back} = \qty{25}{\dB}$
</left>
<right>
* given: $P_S = \qty{6}{\watt}$
* required: $P_R$
</right>

<left>
<fragment>
$\begin{split}P_V &= P_{ERP}\\ &= P_S \cdot 10^{\frac{g_d}{\qty{10}{\dB}}}\\ &= \qty{6}{\watt} \cdot 10^{\frac{\qty{15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{189.7}{\watt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\qty{25}{\dB} &= 10 \cdot \log_{10}{\left(\frac{P_V}{P_R}\right)} \unit{\dB}\\ \Rightarrow \frac{P_V}{P_R} &= 10^{\frac{\qty{25}{\dB}}{\qty{10}{\dB}}}\\ &= 316.2\\ \Rightarrow P_R &= \frac{P_V}{316.2}\\ &= \frac{\qty{189.7}{\watt}}{316.2}\\ &= \qty{0.6}{\watt}\end{split}$
</fragment>
</right>

---

[question:AG218]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $U_V = \qty{300}{\micro\volt\per\meter}$
* given: $U_R = \qty{20}{\micro\volt\per\meter}$
</left>
<right>
* given: $U_D = \qty{128}{\micro\volt\per\meter}$
* required: $g_D$, $\frac{Front}{Back}$
</right>

<left>
<fragment>
$\begin{split}g_D &= 20 \cdot \log_{10}{\left(\frac{U_V}{U_D}\right)} \unit{\dB}\\ &= 20 \cdot \log_{10}{\left(\frac{\qty{300}{\micro\volt\per\meter}}{\qty{128}{\micro\volt\per\meter}}\right)}\\ &= \qty{7.4}{\dB}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\frac{Front}{Back} &= 20 \cdot \log_{10}{\left(\frac{U_V}{U_R}\right)} \unit{\dB}\\ &= 20 \cdot \log_{10}{\left(\frac{\qty{300}{\micro\volt\per\meter}}{\qty{20}{\micro\volt\per\meter}}\right)}\\ &= \qty{23.5}{\dB}\end{split}$
</fragment>
</right>
