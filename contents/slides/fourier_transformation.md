## Fourier transform and breaking signals down

* Signals can be represented both in the time domain and in the frequency domain  
* In the time domain: X axis $\rightarrow$ time, Y axis $\rightarrow$ voltage or power  
* In the frequency domain: X axis $\rightarrow$ frequency, Y axis $\rightarrow$ amplitude or power

---

### Breaking signals down

* Every signal can be represented as a superposition of sine waves  
* Every sine wave has a particular amplitude and phase  
* This principle makes it possible to break complex signals down into their components

---

### Fourier transform

* A mathematically complex method that analyses a signal in time  
* Shows which sine waves (frequencies) the signal contains  
* The result is shown as a frequency spectrum (X axis: frequency, Y axis: amplitude/power)

---

### Fast Fourier transform (FFT)

* Efficient computation of the discrete Fourier transform (DFT)  
* Reduces the computing effort considerably  
* Widely used in software and hardware for signal processing

--- style="font-size: smaller;"

## Spectra of typical waveforms

* *Sine wave*: only one frequency: $f$
* *Square wave*: only odd multiples: $f$, $3f$, $5f$, $7f$, ...
* *Sawtooth*: all integer multiples: $f$, $2f$, $3f$, $4f$, ...
* *Triangular wave*: only odd multiples: $f$, $3f$, $5f$, $7f$, ... (high harmonics fall off faster than with the square wave)

In the examination you only need to be able to tell a sine wave from a square wave. 

<note>
Square-wave and triangular-wave signals both contain only odd harmonics. The difference lies in how the amplitudes fall off: with the triangular-wave signal the higher harmonics become smaller much faster.
</note>

---

[question:AF630]

---

[question:AB404]

---

[question:AB405]

---

[question:AB406]

---

[question:AB407]
