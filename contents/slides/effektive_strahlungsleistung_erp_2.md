## Calculating the effective radiated power (ERP)

* Only take into account the energy that actually arrives at the antenna – cable losses are subtracted
* ERP is calculated as the product of the power supplied and the antenna gain (relative to a half-wave dipole)

---
[question:AG501]
---

### Notes on calculating ERP

* Losses are subtracted from the transmit power before the gain factor ($G_{Antenne}$) is applied
* The calculation must be relative to a half-wave dipole

---
[question:AG502]
---

### ERP in amateur radio – a practical example

* The frequency plan for the $\qty{630}{\meter}$ band specifies a maximum ERP of $\qty{1}{\watt}$
* At $\qty{630}{\meter}$ a half-wave dipole would be $\qty{315}{\meter}$ long – usually not feasible, so shortened antennas are used
* Shortened antennas have a lower efficiency, e.g. an antenna gain of $\qty{-20}{\dBd}$
* Power ratio: $\qty{-20}{\dB}$ corresponds to a factor of $\num{0.01}$; example: $\qty{50}{\watt} \cdot 0.01 = \qty{0.5}{\watt}$ ERP

--- style="font-size: 0.7em;"

### Power ratios on the formula sheet

This table is part of the formula sheet and is available during the examination.

| r:   | r: Power ratio | r: Voltage ratio |
| $\qty{-20}{\dB}$ | $\num{0.01}$ | $\num{0.1}$ |
| $\qty{-10}{\dB}$ | $\num{0.1}$ | $\num{0.32}$ |
| $\qty{-6}{\dB}$ | $\num{0.25}$ | $\num{0.5}$ |
| $\qty{-3}{\dB}$ | $\num{0.5}$ | $\num{0.71}$ |
| $\qty{-1}{\dB}$ | $\num{0.79}$ | $\num{0.89}$ |
| $\qty{0}{\dB}$ | $\num{1}$ | $\num{1}$ |
| $\qty{1}{\dB}$ | $\num{1.26}$ | $\num{1.12}$ |
| $\qty{3}{\dB}$ | $\num{2}$ | $\num{1.41}$ |
| $\qty{6}{\dB}$ | $\num{4}$ | $\num{2}$ |
| $\qty{10}{\dB}$ | $\num{10}$  | $\num{3.16}$ |
| $\qty{20}{\dB}$ | $\num{100}$ | $\num{10}$ |
[table:Pegel_Verhältnis:Power and voltage ratios for important values of loss and gain]

---
[question:AG503]
---
#### Solution
* given: $P_S = \qty{50}{\watt}$
* given: $a \approx \qty{0}{\dB}$
* given: $g_d = \qty{-20}{\dBd}$
* required: $P_{\textrm{ERP}}$

<fragment>
$\begin{split} P_{\textrm{ERP}} &= P_S \cdot 10^{\frac{g_d - a}{\qty{10}{\dB}}}\\ &= \qty{50}{\watt} \cdot 10^{\frac{\qty{-20}{\dBd} - \qty{0}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{50}{\watt} \cdot 10^{-2} = \qty{0.5}{\watt}\end{split}$
</fragment>
