In amplitude modulation (AM), a modulating signal, e.g. a speech signal, is modulated onto the carrier by changing its amplitude. In AM, the frequency of the carrier is not affected but remains unchanged.

We have already met the simplest and at the same time most extreme case: the transmission of Morse characters by continuous wave (CW). Switching the carrier on and off in the rhythm in which the Morse key is operated can also be described as alternating between minimum and maximum amplitude.

To modulate a speech signal with AM, the range between minimum and maximum amplitude is used as well. In the waterfall display in Figure [ref:n_Wasserfall0] we see an amplitude-modulated speech signal. In the middle, the carrier can clearly be seen as a narrow line of constant frequency. To the left and right of the carrier, however, there is also something to be seen, even though the frequency of the carrier was not affected at all!

<margin>
[picture:716:n_Wasserfall0:Signal of an AM broadcast transmitter (speech / music)]
</margin>

This unexpected effect arises because changing the amplitude changes the shape of the carrier, so that it no longer corresponds to a pure sine wave. We call the additional frequencies *sidebands*. They contain the transmitted information, e.g. the speech. In Figure [ref:n_seitenband] we see a common symbolic representation of AM, with the carrier in the middle and the two sidebands to its left and right.

<margin>
[picture:476:n_seitenband:Symbolic representation of an amplitude-modulated signal with carrier and sidebands]
</margin>

<webindepth>
*Why does AM produce additional frequencies beside the carrier?* This can be explained once you understand exactly what an amplitude spectrum or waterfall display shows: it shows, for each frequency, how large the amplitude is. More precisely, we have to say: it shows, for all possible sine waves of different frequencies, how strong their amplitude is. So if the display shows a peak at, for example, $\qty{144.3}{\mega\hertz}$, then a pure sine wave with a frequency of $\qty{144.3}{\mega\hertz}$ is being measured. But if the display shows peaks at, say, $\qty{144.300}{\mega\hertz}$ and $\qty{144.301}{\mega\hertz}$ at the same time, then two sine waves have been measured.

With this knowledge, let us look again at the AM transmission in the waterfall display. We can now see that many different frequencies between $\qty{144.250}{\mega\hertz}$ and $\qty{144.350}{\mega\hertz}$ occur, with different amplitudes. So many different sine waves can be measured at the same time.

[picture:738:n_seitenband_frequenzen_einzeln:Several sine waves of different frequencies]

The question remains why a single sine wave, distorted by modulation, suddenly becomes several sine waves. To answer this, let us look at it the other way round. If you have several sine waves of different frequencies and add them up, the result is a "distorted" oscillation!

[picture:739:n_seitenband_frequenzen_addiert:Sum of several sine waves of different frequencies]

These are simply two different ways of looking at it. You can regard it either as a distorted oscillation or as the sum of several sine waves. And that is why changing the amplitude of a carrier means that further frequencies beside the carrier can be seen in the waterfall display.
</webindepth>

[question:NE202]
[question:NE206]

By the way, the bandwidth occupied by AM is twice the highest frequency of the modulating signal. In our example from the previous section, the highest frequency was $\qty{2700}{\hertz}$. Accordingly, this signal would occupy a bandwidth of $\qty{5400}{\hertz}$ as an AM transmission.
