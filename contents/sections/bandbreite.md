As we have learnt, the occupied transmission bandwidth depends on the mode and, in FM, also on the deviation. A maximum permitted bandwidth is laid down for each of the amateur bands. It can be found in [Annex 1](https://50ohm.de/a1) to the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV), from which we have already taken the band edges. These bandwidths must not be exceeded. Every radio amateur is personally responsible for complying with them.

<webmargin>
| l: Frequency ranges | l: Status | X: Add. conditions of use|
| $\qtyrange{135.7}{137.8}{\kilo\hertz}$| S | 1 2 10 |
| $\qtyrange{472}{479}{\kilo\hertz}$| S | 1 |
| $\qtyrange{3500}{3800}{\kilo\hertz}$ | P | 3 |
| $\qtyrange{10100}{10150}{\kilo\hertz}$ | S | 1 10 12 |
| $\qtyrange{28}{29.7}{\mega\hertz}$ | P | 4 13 |
| $\qtyrange{144}{146}{\mega\hertz}$ | P | 6 13 |
| $\qtyrange{430}{440}{\mega\hertz}$ | P | 7 13 |
[table:n_tab_afuv:Extract from Annex 1 to the AFuV]
</webmargin>

<webmargin>
The numbers under the additional conditions of use in the table above mean the following (the numbers not shown are irrelevant to the bandwidth):
* *1* Maximum permitted occupied bandwidth of an amateur radio emission: $\qty{800}{\hertz}$.
* *3* Maximum permitted occupied bandwidth of an amateur radio emission: $\qty{2.7}{\kilo\hertz}$.
* *4* Maximum permitted occupied bandwidth of an amateur radio emission below $\qty{29}{\mega\hertz}$: $\qty{7}{\kilo\hertz}$, above $\qty{29}{\mega\hertz}$: $\qty{40}{\kilo\hertz}$.
* *6* Maximum permitted occupied bandwidth of an amateur radio emission: $\qty{40}{\kilo\hertz}$.
* *7* Maximum permitted occupied bandwidth of an amateur radio emission: $\qty{2}{\mega\hertz}$; for amplitude-modulated television transmissions: $\qty{7}{\mega\hertz}$.
</webmargin>

The following questions can all be solved with the help of the footnotes in Annex 1 to the AFuV, which – as already mentioned – is available as an aid during the examination. We recommend that you familiarise yourself with the Annex before the examination!

[question:VD738]
[question:VD739]
[question:VD740]
[question:VD741]
[question:VD742]

---

Particular care is needed with transmissions near the edges of the amateur bands. An example: suppose an FM signal occupies a bandwidth of $\qty{15}{\kilo\hertz}$, and we set the transmitter to the lower band edge of the $\qty{70}{\centi\meter}$ band, i.e. to $\qty{430}{\mega\hertz}$. The transmitted signal lies around the carrier frequency, i.e. $\qty{7.5}{\kilo\hertz}$ below and above it. So it would extend from $\qty{429.9925}{\mega\hertz}$ to $\qty{430.0075}{\mega\hertz}$. Since half of the signal would then be outside the band, we must not press the PTT! So in FM, and also in AM, we must always keep a distance of at least half the occupied bandwidth from the band edge.

<indepth>
[picture:908:n_bandbreite_falsch:Wrong -- transmitting outside the band edges]
[picture:909:n_bandbreite_richtig:Right -- transmitting within the band edges]
</indepth>

<indepth>
With SSB, things are a little different at the band edge. Here the signal is found on only one side of the (suppressed) carrier frequency. In LSB the signal lies entirely below the carrier frequency, in USB entirely above it. So if, for example, you set the upper band edge as the transmit frequency, you could quite legitimately transmit in LSB, since the whole signal stays within the band. In USB, however, you could not transmit there, since the whole signal would be outside the band.
</indepth>

[question:NE305]

