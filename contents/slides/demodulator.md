## Demodulation of signals

* Demodulation converts a modulated RF signal into an audible AF signal  
* A suitable demodulation method is chosen according to the modulation used  
* Aim: recovering the original AF

---
### AM demodulation

<left>
[picture:141:demodulator_huellkurvendemodulator_am:Envelope detector for demodulating AM signals]
</left>
<right>
* AM signals are processed with an envelope detector  
* RF signal is selected by a tuned circuit and rectified  
* Capacitor charges $\rightarrow$ resistor discharges it with a defined time constant
</right>

---

[question:AD501]

---

<left>
[picture:607:demodulator_huellkurvendemodulator_am_2:Envelope detector with IF input signal]

[picture:146:demodulator_huellkurvendemodulator_am_abbx:Demodulated signal at point X]
</left>
<right>
* Terminal X: shows the rectified peak voltage  
* Slight fall in voltage due to discharge through the parallel resistor  
* Envelope corresponds to the AF modulated onto the carrier, overlaid with a sawtooth signal  
* Subsequent filtering removes the carrier component
</right>

---

[question:AD502]

--- style="font-size: smaller;"
### FM demodulation

<left>
[picture:841:demodulator_flankendiskriminator:Tuned circuit as a slope detector]

[picture:149:demodulator_flankendiskriminator_schaltung:FM slope detector]
</left>
<right>
* FM demodulation by means of a slope detector  
* Signal from the intermediate frequency passes into a tuned circuit  
* Tuned circuit: resonant frequency $f_\text{res}$ slightly offset from $f_\text{ZF}$
* Frequency changes are converted into amplitude changes  
* Following AM demodulator delivers the AF
</right>

---

[question:AD504]

---

####  FM demodulation by means of a PLL  

<left>
[picture:77:a_fm_demodulation_pll:Block diagram of FM demodulation by means of a PLL]
</left>
<right>
* PLL uses a voltage-controlled oscillator (VCO) that follows the input signal  
* Control voltage corresponds to the frequency modulation (the AF modulated onto the carrier)
* Signal taken off for further AF processing
</right>

---

[question:AD505]

---
### SSB demodulation

* SSB demodulation by means of a product detector  
* Ring mixer mixes the intermediate frequency (IF) with a beat frequency oscillator (BFO)  
* The resulting mixing product is the desired SSB AF signal  
* BFO must be tuned exactly to the suppressed carrier

---

[question:AD506]

