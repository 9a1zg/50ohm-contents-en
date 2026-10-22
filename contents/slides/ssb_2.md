## Bandwidth
<left>
* Compared with AM, less than half the bandwidth is used
* At most $\qty{2.7}{\kilo\hertz}$
* Equal to the AF signal
</left>
<right>
[picture:743:e_bandbreite_am_ssb:Bandwidth of AM, USB and LSB]
</right>

---
[question:EE201]
---
[question:EE202]
---
[question:EJ210]

---

## Modulation

<left>
* By mixing and filtering
* Preselecting USB or LSB selects the carrier frequency
* The mixer produces two frequencies
* The band-pass filter lets only one frequency through
</left>
<right>
[picture:500:e_ssb_modulation:Block diagram of SSB modulation by the filter method]
</right>

---
<left>
* The trick here is that the band-pass filter has only one resonant frequency
* Shifting the carrier frequency in the oscillator then lets the wanted sideband through
</left>
<right>
[picture:500:e_ssb_modulation:Block diagram of SSB modulation by the filter method]
</right>
---
<left>
Example LSB:
* Microphone: $\qty{300}{\hertz}$ - $\qty{3}{\kilo\hertz}$
* LSB oscillator: $\qty{9001.5}{\kilo\hertz}$
* DSB signal:<br/> a) $\qtyrange{8998.5}{9001.2}{\kilo\hertz}$<br/> b) $\qtyrange{9001.8}{9004.5}{\kilo\hertz}$
* Filter: $\qty{9000}{\kilo\hertz}\pm\qty{1.5}{\kilo\hertz}$
* SSB signal:<br/> $\qtyrange{8998.5}{9001.2}{\kilo\hertz}$
</left>
<right>
[picture:831:e_ssb_modulation_lsb:Frequencies with the filter method in LSB]
[picture:940:e_ssb_modulation_lsb_spektrum:Spectrum with the filter method in LSB]
</right>
<note>
* The switch in the picture should be set to LSB
* Only the signal from a) is let through
* The SSB signal can be mixed again for transmission in the amateur band
</note>
---
<left>
Example USB:
* Microphone: $\qty{300}{\hertz}$ - $\qty{3}{\kilo\hertz}$
* USB oscillator: $\qty{8998.5}{\kilo\hertz}$
* DSB signal:<br/> a) $\qtyrange{8995.5}{8998.2}{\kilo\hertz}$<br/> b) $\qtyrange{8998.8}{9001.5}{\kilo\hertz}$
* Filter: $\qty{9000}{\kilo\hertz}\pm\qty{1.5}{\kilo\hertz}$
* SSB signal:<br/> $\qtyrange{8998.8}{9001.5}{\kilo\hertz}$
</left>
<right>
[picture:832:e_ssb_modulation_usb:Frequencies with the filter method in USB]
[picture:941:e_ssb_modulation_usb_spektrum:Spectrum with the filter method in USB]
</right>
<note>
* Only the signal from b) is let through
* The SSB signal can be mixed again for transmission in the amateur band
</note>

---
[question:EE203]
---
[question:EE204]

---
### AF signal

<left>
* For speech, between $\qty{300}{\hertz}$ and $\qty{3000}{\hertz}$ is enough
* Corresponds to $\qty{2.7}{\kilo\hertz}$
* Narrower filters, e.g. $\qty{2.4}{\kilo\hertz}$, are also used
* On many transceivers the filters can be set
</left>
<right>
* If an AF signal with a larger bandwidth is used, the RF bandwidth increases
* Should be avoided, so as not to cause interference to neighbouring signals
* Keep to the maximum bandwidth in the band plan
</right>

---
[question:EJ211]
<note>
* If the bottom $\qty{300}{\hertz}$ of the AF are subtracted, it comes to $\qty{2.7}{\kilo\hertz}$ again
</note>
---
[question:EF310]
---
[question:EE207]

---
## Microphone gain
* The AF power controls the RF power
* Too quiet a microphone results in less output power from the transmitter
* Too much microphone gain can cause interference to stations on closely adjacent frequencies

---
[question:EE206]
---
[question:EE205]
---
[question:EJ215]












