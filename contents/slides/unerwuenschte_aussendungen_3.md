## Unwanted emissions from mixing products

<left>
[picture:243:a_unerwuenschte_aussendungen_bandpassfilter:Frequency response of a band-pass filter]
</left>
<right>
* Arise in the frequency generation of transmitters  
* Mixing products arise in mixers  
* Band-pass filters suppress unwanted signals  
</right>

---

[question:AJ208]

---

[question:AJ211]

---

[question:AJ209]

--- style="font-size: smaller;"

### Harmonics and overtones

<left>
[picture:868:a_harmonische: Overtones (OW), harmonics (Harm.) and spurious emissions (NA)]
</left>
<right>
* Multiples of the fundamental frequency of a signal  
* Differ in definition and in the way they are counted  
* 1st harmonic = fundamental frequency  
* 2nd harmonic = 1st overtone  
* 3rd harmonic = 2nd overtone  
</right>
  
---

[question:AJ204]

---
#### Solution
* given: $f = \qty{29.5}{\mega\hertz}$
* given: $n = 3$
* given: broadcast band: $\qtyrange{88.5}{108.0}{\mega\hertz}$

<fragment>
$f \cdot n = \qty{29.5}{\mega\hertz} \cdot 3 = \qty{88.5}{\mega\hertz}$
</fragment>

---

[question:AJ203]

---
#### Solution
* given: $f = \qty{7.20}{\mega\hertz}$
* given: $n = 4$
* required: 3rd overtone

<fragment>
$f \cdot n = \qty{7.20}{\mega\hertz} \cdot 4 = \qty{28.80}{\mega\hertz}$
</fragment>

---

### How harmonics arise

<left>
[picture:106:a_unerwuenschte_aussendungen_uebersteuerung:Overdriven signal]
</left>
<right>
* Cause: overdriving of amplifier stages  
* Limiting of the amplitude peaks leads to distortion  
* Harmonics occur when the sine shape is not ideal  
</right>

<note>
Overtones and harmonics always arise when there are departures from the ideal sine curve.
</note>

---

[question:AJ207]

---

## Rejector circuits for suppression

* Suppressing individual overtones or harmonics  
* Rejector circuit: attenuates exactly one frequency as strongly as possible  
* Other frequencies are passed almost unhindered  

---

[question:AJ210]

---

## Spurious emissions

* Occur in the immediate vicinity of the transmitted signal  
* Difficult to suppress with filters  
* Caused by overdriven microphone gain  
* Unintentionally widen the transmitted signal (spurious emissions, spurious products, "splatter")  

---

[question:AJ219]

---

## Interference from an unstable supply voltage

* Poor power supplies produce ripple voltage  
* Can lead to AM emissions  
* AF signals coupled in affect the transmitter  
* A particular problem with older transmitters  

---

[question:AJ222]

---

[question:AJ223]

---

## Legal limits for harmonics and spurious emissions

* Radio amateurs must comply with limits  
* Two frequency ranges with different requirements  

<note>
Further information in [Order 33](http://50ohm.de/vfg33) of 2007.
</note>

---

### HF range ($\qtyrange{1.7}{35}{\mega\hertz}$)

* Attenuation at least $\qty{40}{\dB}$
* Applies to signal powers above $\qty{0.25}{\micro\watt}$

---

[question:AJ224]

---

### VHF/UHF/SHF range ($\qtyrange{50}{1000}{\mega\hertz}$)

* Attenuation at least $\qty{60}{\dB}$
* Applies to signal powers above $\qty{0.25}{\micro\watt}$

---

[question:AJ225]
