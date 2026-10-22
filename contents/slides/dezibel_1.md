--- style="font-size: 0.7em;"
## Decibels explained simply

| l:What | r:Power in $\unit{\milli\watt}$ |
| Effective radiated power, EME station | 100 000 000 | 
| Standard transceiver | 100 000 |
| Small handheld | 1 000 |
| Loudspeaker signal (normal room volume) | 100 |
| Headphone signal | 1 |
| Loud HF signal | 0.000 001 |
| Quiet HF signal (RX antenna input) | 0.000 000 000 001 |
[table:e_dezibel_leistungen_mw:Powers in $\unit{\milli\watt}$]

Anyone dealing with these numbers automatically starts counting the zeros.

--- style="font-size: 0.7em;"
We count the zeros (and call the result "bels")

| l:What | r:Power in $\unit{\milli\watt}$ | r:Bels |
| Effective radiated power, EME station | 100 000 000 | 8 |
| Standard transceiver | 100 000 | 5 |
| Small handheld | 1 000 | 3 |
| Loudspeaker signal (normal room volume) | 100 | 2 |
| Headphone signal | 1 | 0 |
| Loud HF signal | 0.000 001 | -6 |
| Quiet HF signal (RX antenna input) | 0.000 000 000 001 | -12 |
[table:e_dezibel_leistungen_bel:Powers in $\unit{\milli\watt}$ and bels]

<note>
After Alexander Graham Bell
</note>
--- style="font-size: 0.7em;"
$\unit{\dBm}$ = decibels relative to $\unit{\milli\watt}$

| l:What | r:Power in $\unit{\milli\watt}$ | r:Bels | r:$\unit{\dBm}$ |
| Effective radiated power, EME station | 100 000 000 | 8 | 80 |
| Standard transceiver | 100 000 | 5 | 50 |
| Small handheld | 1 000 | 3 | 30 |
| Loudspeaker signal (normal room volume) | 100 | 2 | 20 |
| Headphone signal | 1 | 0 | 0 |
| Loud HF signal | 0.000 001 | -6 | -60 |
| Quiet HF signal (RX antenna input) | 0.000 000 000 001 | -12 | -120 |
[table:e_dezibel_leistungen_bel:Powers in $\unit{\milli\watt}$ and bels]

<note>
* Factor 10
* deci as in decimetre
</note>
---
### Power gain

*Receiver*
* Input signal: $\qty{0.000000000001}{\milli\watt}$
* Output signal: $\qty{100}{\milli\watt}$
* Gain required: $\num{100000000000000}$
 
*Transmitter*
* Frequency-generating stage (oscillator): $\qty{10}{\milli\watt}$
* Output signal: $\qty{100000}{\milli\watt}$
* Gain required: $\num{10000}$
 
---
### Power gain in dB
*Receiver*
* Input signal: $\qty{0.000000000001}{\milli\watt} = \qty{-120}{\dBm}$
* Output signal: $\qty{100}{\milli\watt} = \qty{20}{\dBm}$
* Gain required: $\num{100000000000000} = \qty{140}{\dB}$
 
*Transmitter*
* Frequency-generating stage (oscillator): $\qty{10}{\milli\watt} = \qty{10}{\dBm}$
* Output signal: $\qty{100000}{\milli\watt} = \qty{50}{\dBm}$
* Gain required: $\num{10000} = \qty{40}{\dB}$

<note>
* The difference is the gain
* Gain is a factor and is not relative to the $\unit{mW}$, hence just $\unit{\dB}$
</note>

--- style="font-size: 0.7em;"
## Important power ratios

| c:$\unit{dB}$ | c:≈ Power ratio |
| $0$ | $1$ |
| $1.5$ | $\sqrt{2} = 1.41$ |
| $2.15$ | $1.64$ |
| $3$ | $2$ |
| $5$ | $\sqrt{10} = 3.16$ |
| $6$ | $4$ |
| $10$ | $10$ |
| $20$ | $100$ |
[table:e_dezibel_leistungsfaktoren:Important power ratios in $\unit{\dB}$]

<note>
* Reminder: 1.64 is the factor between the dipole and the isotropic radiator
</note>

---
### Calculating with a calculator

Older models
* Factor value $\rightarrow$ *log* key $\rightarrow\times 10 \rightarrow\unit{\dB}$
* $\unit{\dB}$ value $\rightarrow\div 10 \rightarrow$ *$10^x$* key $\rightarrow$ factor

Newer models
* *log* key $\rightarrow$ factor value $\rightarrow$ *)* key $\rightarrow\times 10 \rightarrow$ *=* key $\rightarrow\unit{\dB}$
* *$10^x$* key $\rightarrow$ $\unit{\dB}$ value $\rightarrow \div 10 \rightarrow$ *=* key $\rightarrow$ factor

---
[question:EA107]