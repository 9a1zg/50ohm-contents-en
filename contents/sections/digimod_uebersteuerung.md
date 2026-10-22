Everyone has surely heard an overdriven amplifier or an overdriven sound recording at some point. If the volume is turned up too far when recording or playing back, distortion can occur.

If, for example, too strong an audio signal is applied to the input of a transmitter, harmonics can be produced and transmitted. Figure [ref:uebersteuerung_ft8] shows such an overdriven FT8 signal in the waterfall display: on the left, in yellow, is the wanted signal, and to its right are the unwanted harmonics.

<margin>
[picture:720:uebersteuerung_ft8:An overdriven FT8 signal, on the far left the wanted one, to its right the unwanted harmonics]
[photo:328:uebersteuerung_ft8_wsjtx:An overdriven FT8 signal in the waterfall of the WSJTX software]
</margin>

Distortion due to overdriving can also occur in the transmit amplifier. To prevent this, many radios have an automatic level control (ALC). It can intervene by turning down the gain.

---

With transmissions in digital modes with a constant amplitude, such as FT8, WSPR or RTTY, a response of the ALC is often a sign that the audio signal from the PC is too strong and is being overdriven. This can lead to unwanted *splatter* on the band. The audio signal should therefore always be checked carefully with these modes. The ALC turning the level down would not in itself be critical at first, since with these modes the information lies in the frequency-shift keying. Nevertheless, the ALC being triggered is a strong indication that the AF signal is already overdriven.

<indepth>
The [user guide](https://50ohm.de/wsjtx) of the WSJTX software gives a good recommendation on this: as a first step, press the TUNE button to switch the transceiver to transmit and produce a steady tone. This tone can be checked by ear with the radio's monitor function, or visually on the waterfall display of the TRX. There should be no distortion, clicks or other interference. Then turn the PWR control slowly down from its maximum until the RF output of the transmitter drops slightly – this is generally regarded as a good level for the audio drive. The ALC indicator and the output power of the transceiver can also help to find the optimum AF signal level.
</indepth>

With digital modes with a varying amplitude (e.g. PSK31, QPSK, 16-QAM), however, the ALC can lead to new problems. Depending on volume or frequency, the signal could trigger the ALC to different degrees at different times and so change the amplitude over time in an unwanted way. This means that our actual wanted signal is additionally amplitude-modulated. This produces additional frequency components, which are radiated as spurious emissions. On the one hand, this can cause interference to other radio amateurs or radio services on adjacent frequencies. On the other hand, it makes decoding at the receiver more difficult.

Whether the ALC causes problems, and how severe they are, depends on many factors. Besides the transmission method used, the specific implementation of the ALC in the transceiver, e.g. with regard to its response and hold times, also plays a part. The way the ALC is indicated also differs from radio to radio. A look at the manual can show when the level control intervenes and how this is indicated. In general, however, it can be said: if the ALC does not intervene, it does not cause any problems either.

Remember: with digital modes using an AF signal, take care to keep the AF level low enough that no overdriving occurs and the automatic level control does not intervene.

[question:EJ218]
[question:EJ217]
[question:EJ219]