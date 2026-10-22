## RF power amplifiers

* Amplify the RF signal from the preceding stages
* Aim: reaching the desired output power
* Two types: broadband and selective RF amplifiers

---
### Broadband RF amplifiers

<left>
[picture:491:a_verstaerker_breitband_gegentaktverstaerker:Broadband push-pull amplifier]
</left>
<right>
* Uniform gain over a wide frequency range (e.g. $\qtyrange{1}{30}{\mega\hertz}$)
* Recognisable by broadband coupling transformers
* No parallel or series capacitances forming a tuned circuit
</right>

---
[question:AF412]

---
### Selective RF amplifiers


<left>
[picture:778:a_verstaerker_selektiver_hf_verstaerker:Selective RF amplifier]
</left>
<right>
* Maximum gain only in a narrow range (e.g. one amateur band)
* Frequency-selective design
* Use of series or parallel tuned circuits in the RF signal path
</right>

---
[question:AF408]

---
# Multistage amplifiers


<left>
[picture:764:a_verstaerker_zweistufiger_breitband_hf_verstaerker:Two-stage broadband RF amplifier]
</left>
<right>
* Amplifiers can be built with several stages by chaining individual stages together
</right>

---
[question:AF413]

---
## Impedance matching between amplifier stages

* Necessary for maximum gain, minimum distortion and optimum efficiency
* Prevents reflections and non-linearities

---
### Methods of impedance matching

* Broadband matching with a transformer with a suitable transformation ratio
* Frequency-selective matching with a tapped tuned circuit

---

[picture:765:a_anpassung_breitbandige_anpassung:Broadband matching between two stages using a transformer with a suitable transformation ratio]

---
[question:AF414]

---

[picture:786:a_anpassung_mosfet:Broadband input and output matching to low-impedance MOSFETs using transformers]

---
[question:AF417]

---

[picture:779:a_anpassung_induktiver_spannungsteiler:Frequency-selective matching with an inductor as an inductive potential divider]

---
[question:AF409]

---

[picture:780:a_anpassung_kapazitiver_spannungsteiler:Frequency-selective matching with capacitors as a capacitive potential divider]


---
[question:AF410]

---

[picture:768:a_anpassung_eingang_schwingkreis:Tuned circuit with variable capacitors for matching the input impedance]

---
[question:AF407]

---

[picture:769:a_anpassung_ausgang_schwingkreis:Tuned circuit with variable capacitors for matching the output impedance]

---
[question:AF406]

---
### Pi filter for impedance matching

* Matches input and output impedances through the ratio of the capacitances
* Inductor and capacitances determine the design frequency
* Low-pass characteristic suppresses harmonics

---
[question:AF405]

---
### LC circuit after an RF power amplifier

* Used for impedance matching and, at the same time, for suppressing harmonics

---
[question:AF404]

---
## Efficiency of an RF power amplifier

* Ratio of the RF output power delivered to the DC supply power supplied

---
[question:AF401]

---
## Bias voltage in power amplifiers

<left>
[picture:786:a_verstaerker_bias_arbeitspunkt:Adjusting the operating point of an amplifier with a potentiometer]
</left>
<right>
* Operating voltage set by potential dividers
* Fine adjustment with preset potentiometers
* DC analysis: ignore capacitors, treat inductors as short circuits
</right>

---
[question:AF420]

---
[question:AF423]

---
[question:AF424]

---
### Calculating the bias voltage

* Applying Ohm's law
* Taking into account parallel and series connections of resistors
* Gate terminals of the transistors are capacitive and can be neglected in the DC analysis

---
[question:AF421]

--- style="font-size: smaller;"
#### Solution
<left>
* given: $U_Z = \qty{6.2}{\volt}$
* given: $R_2 = \qty{270}{\ohm}$
* given: $R_3 = \qty{220}{\ohm}$
</left>
<right>
* given: $R_4 = \qty{6.8}{\kilo\ohm}$
* given: $R_6 = \qty{150}{\ohm}$
* required: $U_{GS}$
</right>

<left>
<fragment>
$\begin{split}R_E &= \frac{(R_3+R_6) \cdot R_4}{(R_3 + R_6) + R_4}\\ &= \frac{(\qty{220}{\ohm} + \qty{150}{\ohm}) \cdot \qty{6.8}{\kilo\ohm}}{\qty{220}{\ohm} + \qty{150}{\ohm} + \qty{6.8}{\kilo\ohm}}\\ &= \frac{\qty{2.516}{\mega\ohm}^2}{\qty{7170}{\ohm}}\\ &= \qty{351}{\ohm}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\frac{U_Z}{U_{GS}} &= \frac{R_2 + R_E}{R_E}\\ \Rightarrow \frac{\qty{6.2}{\volt}}{U_{GS}} &= \frac{\qty{270}{\ohm}+\qty{351}{\ohm}}{\qty{351}{\ohm}}\\ &= 1.77\\ \Rightarrow U_{GS} &= \frac{\qty{6.2}{\volt}}{1.77}\\ &= \qty{3.50}{\volt}\end{split}$
</fragment>
</right>

---
## RF decoupling of the supply voltage

* Prevents interaction between amplifier stages (e.g. tendency to oscillate)
* Implemented with series inductors and decoupling capacitors
* Low-pass characteristic: the DC voltage is passed, RF is blocked

---

[picture:781:a_entkopplung_drossel:Choke for decoupling the RF from the supply voltage]

---
[question:AF411]

---
[question:AF422]

---

[picture:786:a_entkopplung_abblock_kondensatoren:Decoupling capacitors for decoupling the RF from the supply voltage, with a low-pass characteristic]

---
[question:AF419]

---
[question:AF418]

---
## RF properties of capacitors

* Large capacitances (e.g. electrolytic capacitors) can only be used at low frequencies
* For RF applications, a combination of different capacitance values to cover a wide frequency range

---
[question:AF415]

---
## Total gain of a power amplifier

<left>
[picture:470:a_verstaerker_gesamtverstaerkung:Block diagram of an amplifier with gain and loss per stage]
</left>
<right>
* Found from the difference between output and input power
* Calculated by subtracting the dBm values with the correct signs
</right>

---
[question:AF428]
---
#### Solution

* given: $P_1 = \qty{0.3}{\milli\watt}$ or $\qty{-5}{\dBm}$
* given: $P_2 = \qty{20}{\watt}$ or $\qty{43}{\dBm}$
* required: $g$

<left>
<fragment>
$\begin{split}g &= P_2 - P_1\\ &= \qty{43}{\dBm} - (\qty{-5}{\dBm})\\ &= \qty{43}{\dBm} + \qty{5}{\dBm}\\ &= \qty{48}{\dB}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}g &= \qty{10 \cdot \log_{10}{\left(\frac{P_2}{P_1}\right)}}{\dB}\\ &= \qty{10 \cdot \log_{10}{\left(\frac{\qty{20}{\watt}}{\qty{0.3}{\milli\watt}}\right)}}{\dB} \\ &\approx \qty{48}{\dB}\end{split}$
</fragment>
</right>