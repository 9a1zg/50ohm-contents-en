In amplitude modulation (AM) and in SSB, the information to be transmitted is conveyed by changing the amplitude of the radio-frequency carrier. In Class N we have already learnt that in frequency modulation (FM), on the other hand, the amplitude of the carrier remains constant – here the information is conveyed by changing the instantaneous frequency of the carrier.

Figure [ref:e_frequenzmodulation_t] shows an FM signal of constant amplitude over time. An FM signal can therefore be recognised by the fact that the amplitude of the carrier (ideally) remains constant, while its instantaneous frequency changes continuously in accordance with the modulating signal.

<margin>
[picture:906:e_frequenzmodulation_t:An FM signal over time]
</margin>

[question:EE301]

---

Figure [ref:e_frequenzmodulation_frequenzhub] shows, as an example, a sinusoidal AF signal that causes a corresponding frequency excursion (frequency deviation) of a radio-frequency carrier in the spectrum. This means that in an FM signal the volume information is transmitted by the *deviation of the carrier frequency (frequency deviation)*. A louder AF signal would lead to a greater deviation of the carrier frequency and so to a larger bandwidth of the FM signal.

<margin>
[picture:827:e_frequenzmodulation_frequenzhub:Carrier deviation in frequency modulation]
</margin>

<indepth>
The occupied bandwidth of an FM emission is determined by the deviation and the maximum modulating frequency. As a first approximation, for small deviation and a low modulating frequency, *Carson's rule* can be applied. It gives the bandwidth that contains $\qty{99}{\percent}$ of the transmit power.

$B\approx2 \cdot \left(\Delta f_{\textrm{T}} + f_{\textrm{mod max}} \right)$
  
This topic is discussed in more detail in Class A. 
</indepth>

[question:EE306]
[question:EE304]

To comply with the legal requirements on the occupied bandwidth of an FM signal, FM transmitters first limit the amplitude of the microphone signal (with a limiting amplifier) and then modulate it onto the carrier by FM. The frequency deviation of the modulator at maximum volume is either fixed or can be set with a deviation control.

[question:EE305]

Because the information modulated onto them is contained not in the amplitude but only in the frequency, FM signals are relatively insensitive to amplitude interference (e.g. from lightning, ignition systems, motors) compared with AM or SSB. This gives them advantages in susceptibility to interference, especially when operating in motor vehicles and in noisy environments.

[question:EE302]
[question:EE303]