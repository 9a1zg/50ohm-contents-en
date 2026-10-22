## The process of sampling

* Analogue signals are converted into discrete samples  
* Sampling: taking values of a continuous signal at fixed intervals of time  
* Comparable to a camera that takes pictures at regular intervals

---

### Sampling – the camera example

* A camera takes, for example, $\num{24}$ pictures per second
* Fast movements can occur between the pictures that are not captured  
* As with the camera, a sudden event (e.g. a fly) can be lost between two pictures  
* This results in a loss of information in time

---

### Loss of information and the limit of reconstruction

* Fast changes in the signal can go undetected between the samples  
* For error-free reconstruction, there must be a sample before and after every change in the signal  
* If this is not the case, details are lost – aliasing occurs

---

## The Nyquist–Shannon sampling theorem

* For a signal with a maximum frequency $f_{\mathrm{max}}$, the sampling rate must be $\gt 2 \cdot f_{\mathrm{max}}$
* Only then can all changes in the signal be captured and reconstructed correctly  
* If the rate falls below this limit, aliasing effects occur

---

[question:AF617]

---

### Practical example: CD player

* CD players typically work at $\qty{44.1}{\kilo\sps}$ ($\num{44100}$ samples per second)
* It follows that frequencies up to about $\qty{22}{\kilo\hertz}$ can be represented correctly
* This corresponds to the hi-fi frequency range of good stereo systems  
* Remember: the sampling frequency should always be just above twice the highest frequency to be processed

---

[question:AF616]

---

[question:AF618]

---

[question:AF619]