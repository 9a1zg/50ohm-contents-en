The frequency display of a receiver can also be checked. Unlike with a transmitter, however, the receive frequency set cannot normally simply be measured with a frequency counter at an output of the radio. The received RF signal is processed further early on in the receiver and, for example, converted to an intermediate frequency.

To check the frequency display, therefore, a reference signal that is as accurate as possible is used. For this, a signal generator or an accurate reference oscillator of known frequency is connected to the antenna input of the receiver. The receiver is then tuned to this signal, and its frequency display is compared with the known frequency of the reference signal.

The more accurate the reference used, the more accurately the frequency display of the receiver can be checked or calibrated. Particularly suitable are, for example, GPS-synchronised oscillators or high-quality temperature-stabilised crystal oscillators (OCXO).

<attention>
A signal generator connected directly can easily damage a receiver input. If in doubt, the measurement should be started with the generator's lowest voltage and an attenuator.
</attention>

[question:AI511]
[question:AI504]

---

With transmitters, frequency measurement is simpler. A frequency counter is connected to the antenna socket via an attenuator. Of course, this measurement only makes sense with an unmodulated carrier, i.e. as pure a sine wave as possible.

<indepth>
SSB transmitters produce no signal without modulation. To measure their transmit frequency, an audio signal of known frequency can be fed into the microphone socket. With USB, the audio frequency is subtracted from the reading of the frequency counter at the transmitter output to obtain the frequency of the carrier, which is not transmitted. With LSB it is added.
</indepth>

[question:AI502]
[question:AI501]

A frequency can also be determined with an oscilloscope. For accurate frequency measurements, however, an oscilloscope is usually less suitable than a dedicated frequency counter, as the latter's timebase and measuring method are designed specifically for high frequency accuracy and resolution.

[question:AI503]

---

Simple frequency counters often work with a so-called *gate time*. During this time the instrument counts the periods, or rather the edges or zero crossings, of the input signal. The frequency is then calculated from the number of oscillations counted and the known gate time. Example: with a gate time of one second, determining the frequency is particularly simple: if, for example, $\num{1000}$ periods are counted, the measured frequency is $\qty{1000}{\hertz}$.

<margin>
[picture:1126:a_frequenzmessung_torzeit:Counting a signal with a frequency of $\qty{1.1}{\kilo\hertz}$ with very short gate times]
</margin>

The *frequency resolution* $\Delta f$ states how small the frequency difference between two readings can be for the frequency counter still to distinguish or display it. In a simple direct-counting frequency counter, the frequency resolution is determined by the gate time $T_\mathrm{G}$:

$\Delta f = \frac{1}{T_\mathrm{G}}$

Figure [ref:a_frequenzmessung_torzeit] shows the effect of the gate time, or of the frequency resolution, on the result of the measurement. In both cases the same signal, with an actual frequency of $\qty{1.1}{\kilo\hertz}$, is measured.

With a gate time of only $\qty{1}{\milli\second}$, only one period is counted. From this the frequency counter determines a reading of $\qty{1}{\kilo\hertz}$. So here the short gate time only allows a frequency resolution of $\qty{1}{\kilo\hertz}$.

If the gate time is extended to $\qty{10}{\milli\second}$, as many as $\num{11}$ periods can be counted. This gives a reading of $\qty{1.1}{\kilo\hertz}$. The frequency resolution is now $\qty{100}{\hertz}$, so that the additional digit of the frequency can also be displayed.

The longer the gate time, the more periods are counted and the finer the frequency resolution. A short gate time, on the other hand, has the advantage that the display can be updated more often. In choosing the gate time there is thus a trade-off between fast updating and high frequency resolution. The accuracy of the frequency measurement must be distinguished from its resolution. It depends above all on the accuracy of the frequency counter's timebase.

[question:AI505]