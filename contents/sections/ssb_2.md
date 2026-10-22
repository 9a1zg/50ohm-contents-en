In Class N we learnt that amplitude modulation produces two sidebands beside the carrier, a lower (LSB) and an upper (USB) one, which contain all the information of the modulating signal, while the carrier itself carries no information. Since both sidebands contain the same information, it is enough to transmit only one of them and to suppress the carrier (see Figure [ref:e_ssb_am_modulation]). This method is called single-sideband modulation (SSB), which we also met in Class N. The advantage of SSB is that no transmit power is wasted on the carrier and the second sideband, so that all the power can be used efficiently to transmit the information, while at the same time the bandwidth needed is considerably smaller than with AM.


In single-sideband modulation (SSB), the transmitted signal – depending on the sideband selected on the transceiver – contains either the carrier frequency plus the AF modulating frequency (in USB) or the carrier frequency minus the AF modulating frequency (in LSB). Figure [ref:e_ssb_einzelsignal] shows two examples of this: if a transmitter with a carrier frequency of $\qty{7.100}{\mega\hertz}$ is modulated with an AF signal of $\qty{1}{\kilo\hertz}$ in USB, the transmitter radiates a frequency of $\qty{7.100}{\mega\hertz} + \qty{1}{\kilo\hertz} = \qty{7.101}{\mega\hertz}$. If, on the other hand, the transmitter is modulated in LSB, it radiates a frequency of $\qty{7.100}{\mega\hertz} -\qty{1}{\kilo\hertz} = \qty{7.099}{\mega\hertz}$.

<margin>
[picture:1056:e_ssb_einzelsignal:Sidebands in AM and SSB]
</margin>

The following questions can be solved in this way.

[question:EE203]
[question:EE204]

---

AM signals transmit both sidebands and the carrier, and so have a bandwidth of a little more than twice that of the modulating AF signal (see Figure [ref:e_ssb_einzelsignal]). The bandwidth of an SSB signal is roughly equal to the bandwidth of the modulating AF signal (after the AF signal has been filtered and its bandwidth limited). In SSB, signal components below $\qty{300}{\hertz}$ and the carrier ($\qty{0}{\hertz}$) are also not transmitted but suppressed. SSB therefore has a little less than half the bandwidth of AM.

<margin>
[picture:743:e_ssb_einzelsignal:Sidebands in AM and SSB]
</margin>

[question:EE202]
[question:EE201]

---

As we already learnt in Class N on the subject of Morse telegraphy with *continuous wave* (CW), a constant radio-frequency carrier is switched on and off in a certain rhythm. Compared with voice-modulated signals such as AM and SSB, CW signals need the smallest bandwidth. This is because in CW only a single frequency is keyed, and it is not necessary, as with speech signals, to transmit several frequency components of an AF signal at the same time.

<indepth>
The bandwidth of CW signals depends on the character speed (the keying speed) and, at average sending speeds of 20 words per minute (100 characters per minute), is approx. $\qty{300}{\hertz}$.
</indepth>

[question:EE207]

To avoid interference to neighbouring stations in the band, the occupied bandwidth of an SSB signal should be limited to a maximum of about $\qty{2.7}{\kilo\hertz}$. This bandwidth is entirely sufficient for good speech intelligibility. For this reason, the AF signal from the microphone is band-limited in the transmitter: frequency components below about $\qty{300}{\hertz}$ and above about $\qty{3}{\kilo\hertz}$ are suppressed, since they contribute little to speech intelligibility.

[question:EJ211]
[question:EJ210]

In practice, SSB filters for generating an SSB signal often have a bandwidth of only about $\qty{2.4}{\kilo\hertz}$. In many cases this smaller bandwidth is also sufficient for good speech intelligibility, and at the same time it makes even more efficient use of the available frequency spectrum.

[question:EF310]

Interference to neighbouring stations can also be caused by what is known as *splatter*, which can result from setting the microphone gain too high and so overdriving the AF stages. In the transmitted signal, the effect is that the bandwidth of the SSB transmission increases, which can cause interference to other stations.

[question:EJ215]

Too little microphone gain (AF amplitude) leads to less modulation of the SSB transmitter, which results in a lower output power. It is therefore important for good communication in SSB that the microphone gain is set to the optimum (neither too high nor too low). We will come back to this in more detail in the chapter on the compressor. 

[question:EE206]
[question:EE205]