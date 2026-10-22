The *automatic level control (ALC)* controls the drive to the radio's transmitter power amplifier and, when the power amplifier is overdriven, reduces the amplitude of the signal in the transmit path. The ALC must not be confused with the AGC (automatic gain control), which is in the receive path (see Figure [ref:e_alc]).

<margin>
[picture:914:e_alc:Automatic level control in a transmitter]
</margin>

The ALC senses the output power of the transmitter power amplifier and compares it with a preset maximum value. When this limit is exceeded, the ALC applies a corresponding control voltage to the preceding RF amplifier stage in the transmit path and so reduces the amplitude of the transmitted signal.

As long as the ALC indicator does not respond, you can assume that the control is not intervening and that the transmitter is not being overdriven by too strong an AF signal. As soon as the ALC indicator reacts, you can assume that the control is becoming active, at least in part.

With SSB transmissions, a slight response of the ALC is quite desirable, since it evens out variations in the loudness of the voice and makes optimum use of the available transmit power. Many transceivers have an ALC indicator for this, which usually shows up to what degree the ALC can respond (green zone) and from which point the drive is too high for the ALC to compensate without distortion (red zone).

<margin>
[picture:915:e_alc_trx:ALC in the display of a radio]
</margin>

<tip>
In practice, you can find the optimum point, at which the ALC is only just not yet acting, by slowly increasing the AF drive up to the point at which the ALC responds. You then turn the AF drive back down a little, so that the ALC only just no longer responds and the transmit power indicator still shows the desired output power (possibly a little less).
</tip>

---

With transmissions in digital modes such as FT8 or WSPR, a response of the ALC is often a sign that the audio signal from the PC is too strong and is overdriving the transmitter. This can lead to unwanted *splatter* on the band. The audio signal should therefore always be checked carefully with these modes.

<indepth>
The [user guide](https://50ohm.de/wsjtx) of the WSJTX software gives a good recommendation on this: as a first step, press the TUNE button to switch the transceiver to transmit and produce a steady tone. This tone can be checked by ear with the radio's monitor function, or visually on the waterfall display of the TRX. There should be no distortion, clicks or other interference. Then turn the PWR control slowly down from its maximum until the RF output of the transmitter drops slightly – this is generally regarded as a good level for the audio drive. The ALC indicator and the output power of the transceiver can also help to find the optimum AF signal level.
</indepth>

[question:EF305]