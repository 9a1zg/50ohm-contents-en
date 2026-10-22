## Frequency measurement on receivers

* The receive frequency usually cannot be measured directly, as there is no measuring point  
* For checking, an accurate oscillator or signal generator is connected to the antenna socket  
* Comparison of the generator frequency with the receiver's display  
* GPS-synchronised oscillators/OCXOs offer greater accuracy

<note>
A signal generator connected directly can easily damage a receiver input. If in doubt, the measurement should be started with the generator's lowest voltage and an attenuator.
</note>

---

[question:AI511]

---

[question:AI504]

---

## Frequency measurement on transmitters

* Frequency measurement on transmitters is simpler  
* Frequency counter is connected to the antenna socket via an attenuator  
* Measurement only makes sense with an unmodulated carrier

<note>
SSB transmitters produce no signal without modulation. To measure their transmit frequency, an audio signal of known frequency can be fed into the microphone socket. With USB, the audio frequency is subtracted from the reading of the frequency counter at the transmitter output; with LSB it is added.
</note>

---

[question:AI502]

---

[question:AI501]

---

* Measuring frequency with an oscilloscope is only a makeshift, as these instruments seldom have as accurate a timebase as frequency counters.

---

[question:AI503]

---

* Simple frequency counters almost always work with a so-called *gate time*  
* The instrument switches the input on for a certain time, counts the periods and calculates the frequency from them  
* A gate time of $\qty{1}{\second}$ gives the frequency in $\unit{\hertz}$ directly  
* Short gate time: fast updating
* Long gate time: higher measurement accuracy

---

[question:AI505]


