### Semiconductor diodes in modulators

* Known so far as rectifiers
* AF voltage changes the diode resistance
* AF signal controls the diode current
* RF signal is modulated in step with the AF signal
* Simplest version has a carrier and two sidebands

---
### Diode in an amplitude modulator
<left>
[picture:772:a_modulatoren_am_modulator:AM modulator]
</left>
<right>
* A diode is fed with an AF and an RF signal at the same time
* An LC tuned circuit filters the output signal
</right>

---
[question:AD507]

---
### Balanced mixer for carrier suppression
* Four diodes in a ring arrangement suppress the carrier
* A push-pull circuit cancels the carrier signals
* Only the sidebands remain
* Already shown as the balanced mixer in the second chapter on mixers

---
### Balanced modulator in the SSB modulator
* The balanced modulator generates a double-sideband (DSB) signal
* A band-pass filter lets only one sideband through
* This produces an SSB signal
* Two stages are needed
 
---
[question:AE206]

---
[question:AF302]

---
### Recognising a balanced mixer
<left>
[picture:759:a_modulatoren_dsb:Modulator for AM signals with suppressed carrier]
</left>
<right>
* A diode ring identifies the balanced mixer
* There is no complete push-pull drive
* A transformer provides the equivalent of a centre tap
</right>

---
[question:AF308]

<note>
* AF modulation is fed into the bridge diagonal between the T2 centre tap and chassis
* The oscillator signal is fed into the diode ring via T1
* The DSB signal is coupled out via T2
* Without modulation the potential dividers are at chassis potential
* In this way the carrier is suppressed
* With modulation the potential shifts and current flows in T2
* The output signal is produced
</note>

---
### Carrier suppression and balancing

* Carrier suppression cancels unwanted signals
* The modulator circuit must be balanced

---
[question:AD510]

---
### Adjustment in the modulator

<left>
[picture:762:a_modulatoren_rc_traegerunterdrueckung:$R_1$ and $C_1$ for adjusting the carrier suppression in magnitude and phase]
</left>
<right>
* Amplitudes are adjusted with potentiometers
* Phases are set with trimmer capacitors
</right>

---
[question:AF309]

---
### Balancing the modulator

* The modulator is balanced to suppress the carrier
* The modulation sidebands are retained

---
[question:AF304]

---
[question:AF303]

---
### Second stage of the SSB modulator

<left>
[picture:98:a_modulatoren_blockschaltbild_sender:Block diagram of a transmitter]
</left>
<right>
* The balanced modulator is followed by the second stage
* Filtering selects the wanted sideband
</right>

---
[question:AF305]

---
### Crystal frequency and sideband position

<left>
[picture:500:a_modulatoren_quarzfilter:Crystal filter for selecting the sideband]
</left>
<right>
* Crystals determine the frequency of the suppressed carrier
* For LSB the carrier lies $\qty{1.5}{\kilo\hertz}$ above the $\qty{9}{\mega\hertz}$ centre
* With at most $\qty{3}{\kilo\hertz}$ of AF, the LSB lies $\qty{1.5}{\kilo\hertz}$ below the centre
* For USB it is the other way round
</right>

---
[question:AF306]

---
[question:AF307]
---
#### Solution
* given: $f_Q = \qty{9}{\mega\hertz}$
* given: $f_{LSB} = \qty{9.0015}{\mega\hertz}$
* required: $f_{USB}$

<fragment>
$\begin{split}f_{USB} &= f_Q - (f_{LSB} - f_Q)\\ &= \qty{9}{\mega\hertz} - (\qty{9.0015}{\mega\hertz} - \qty{9}{\mega\hertz})\\ &= \qty{9}{\mega\hertz} - \qty{0.0015}{\mega\hertz}\\ &=\qty{8.9985}{\mega\hertz}\end{split}$ 
</fragment>

---
### Varactor diodes in FM modulators

<left>
[picture:951:a_modulatoren_fm_modulator:FM modulator with varicap]
</left>
<right>
* FM modulators use varactor diodes
* The diode is part of an oscillator tuned circuit
* The reverse voltage sets a fixed diode capacitance
* An AF signal changes the oscillator frequency in step with it
</right>

---
[question:AD508]

---
### Influence of the varactor diode

<left>
[picture:158:a_modulatoren_fm_varicap:Varicap for varying the oscillator frequency]
</left>
<right>
* The varactor diode affects the oscillator frequency
* It is connected in parallel with the tuned circuit
</right>

---
[question:AF310]

---
### FM deviation limiting
* High AF voltages lead to excessive frequency changes
* Deviation limiting is necessary
* Diodes connected in inverse parallel limit the voltage to the knee voltage

---
[question:AD509]

---
### Signal analysis of a diode circuit
<left>
[picture:142:a_modulatoren_regelspannung:Circuit with an output for an AGC voltage]
</left>
<right>
* A single signal does not point to a modulator
* An electrolytic capacitor at the output indicates a DC voltage
</right>

---
[question:AD503]

