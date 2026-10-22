In Class N we have already met unwanted emissions. Such emissions should be avoided at all costs, and this can be achieved by various technical measures – we look at these more closely in this lesson. In radio transmitters, unwanted emissions often arise from *harmonics*, that is, integer multiples of the fundamental frequency, and from what are called *spurious emissions*, as shown in Figure [ref:e_unerwuenschte_aussendungen_uebersicht]. We deal with harmonics first, since they can impair or interfere with other radio services. Interference is said to occur when an amateur station radiates unwanted frequency components so strongly that the permitted limits are exceeded. A typical example is the emission of a harmonic of a transceiver in the FM broadcast band (VHF), as shown in Figure [ref:e_unerwuenschte_aussendungen_oberwelle]. Here four times the fundamental frequency ($\qty{145.9}{\mega\hertz}\cdot 4 = \qty{583.6}{\mega\hertz}$) causes interference. We look at spurious emissions at the end of this lesson.

<margin>
[picture:1008:e_unerwuenschte_aussendungen_uebersicht:Unwanted emissions: harmonics (OW) and spurious emissions (NA)]
</margin>

<margin>
[picture:745:e_unerwuenschte_aussendungen_oberwelle:Interference to a television set's DVB-T2 reception from the harmonic of an amateur radio transmission]
</margin>

---

Unlike the PEP measurement, the measurement of a transmitter's unwanted emissions is always made at the transmitter output, including any SWR meter used, additional matching units and any low-pass filters fitted (see Figure [ref:e_unerwuenschte_aussendungen_trx]).
This ensures that only those unwanted emissions are measured that can actually reach the antenna. The best instrument for this is a spectrum analyser. How exactly such a check is carried out, what the frequency spectrum of harmonics looks like and which legal requirements apply, we will only look at in more detail in Class A.

<margin>
[picture:917:e_unerwuenschte_aussendungen_trx:Measuring unwanted emissions]
</margin>

[question:EJ209]

An ideal transmitted signal, transmitting only on one wanted frequency, should be an ideal sine wave. This contains no frequency components other than the fundamental frequency.

[question:EJ201]

<indepth>
Waveforms that are not sinusoidal, and in particular those with sharp "corners and edges", consist of many different sinusoidal frequency components and have a high harmonic content. Especially when transmitters are overdriven, signals that were sinusoidal before are often distorted or clipped in amplitude. This also produces massive harmonic content. Any departure from the ideal sine shape is therefore to be avoided in ideal transmitted signals. We will look at this subject more closely in Class A. With this applet, however, you can already try it out.

[include:fourier]
</indepth>

---

To suppress harmonics, *harmonic filters* are usually used in the HF range. Their response is designed so that frequencies below a certain cut-off frequency pass through the filter almost unattenuated, while frequencies above this limit are not passed at all or are passed only heavily attenuated. A *harmonic filter* is thus a *low-pass filter*, as we have already met in the chapter on tuned circuits. The frequency response of such a low-pass filter is shown in Figure [ref:e_ua_tiefpass]. Figure [ref:e_ua_tiefpass_selbstbau] shows a home-built low-pass filter made of capacitors and of inductors wound on toroidal cores. When you change band on a multiband transmitter, a suitable harmonic filter is usually selected at the same time. You can often hear the click of a relay that does this switching.

The importance of this topic is shown by the large number of examination questions on it. With what you know about harmonics and low-pass filters, however, they are very easy to answer.

<margin>
[picture:591:e_ua_tiefpass:Frequency response of a low-pass filter]
</margin>

<margin>
[photo:320:e_ua_tiefpass_selbstbau:Home-built low-pass filter]
</margin>

---

[question:EJ202]
[question:EJ204]
[question:EJ205]
[question:EJ206]
[question:EJ207]
[question:EJ208]
[question:EJ203]

<indepth>
[picture:593:bandpass:Frequency response of a band-pass filter]
  
Another way of suppressing harmonics is to use a band-pass filter. Band-pass filters are often used in single-band transmitters and in transmitters for the VHF/UHF/SHF range. In these, signal components that arise during the processing of the transmitted signal, and that may also lie below the transmit frequency, often have to be suppressed as well.
</indepth>

As already mentioned, sinusoidal signals are essential for avoiding harmonic content. This is achieved, among other things, by having the transmitter stages, especially the power amplifiers of a transmitter, work without distortion. If the operating point of a transmitter output stage is readjusted, its linearity and the quality of the emission must always be checked afterwards for low harmonic content.

[question:EF404]

Unwanted emissions can also occur in the immediate vicinity of the actual transmitted signal (see Figure [ref:e_unerwuenschte_aussendungen_uebersicht]) and therefore often affect other radio amateurs on the same band. Such interference is difficult or impossible to suppress with filters and should therefore be avoided by suitable measures right at the start of the signal processing. These *spurious emissions* – also called spurious products, and informally known as "splatter" – often arise from setting the microphone amplifier in the transmitter too high, which unintentionally widens the transmitted signal.

[question:EJ213]
[question:EJ214]

The same applies to digital transmission methods such as packet radio. To avoid spurious emissions and exceeding the permitted bandwidth, especially with AFSK-modulated FM transmitters, either the deviation can be limited or the AF drive reduced.

[question:EJ212]

The stability of the oscillator used in the transmitter can also lead to emissions lying outside the band edges, or to interference with stations on adjacent frequencies. This is possible particularly with older home-built equipment without crystal-controlled oscillators. Modern HF transceivers, but also current home-built equipment and kits, usually have very stable reference oscillators.

[question:EJ216]
