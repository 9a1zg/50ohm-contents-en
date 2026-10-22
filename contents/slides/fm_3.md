### Generation

<left>
[picture:951:a_frequenzmodulation_schaltung:Modulator for generating FM]
</left>
<right>
* The AF changes the capacitance of an oscillator
* E.g. with a varactor diode
* The modulating frequency determines how often the RF carrier changes
</right>
<note>
Will be looked at again later in the chapter on transmitters
</note>

---
[question:AE303]
---
[question:AE301]
---
### Susceptibility to interference

* The information to be transmitted is contained in the change in the signal
* Amplitude fluctuations have no effect
* A limiting amplifier is often used internally
* Insensitive to impulse interference from ignition sparks, electric motors or the like

---
[question:AE302]
---
### Deviation

* Determines the amount by which the frequency of the oscillator changes, depending on the amplitude of the modulated signal
* Larger amplitude in the AF signal $\leftrightarrow$ greater excursion of the carrier
* Greater deviation $\rightarrow$ higher volume in the demodulated signal

---
[question:AE305]
--- style="font-size: smaller;"
### Bandwidth

<left>
[picture:910:a_bandbreite_fm:Bandwidth in FM]
$B \approx 2 \cdot \left(\Delta f_{\textrm{T}} + f_{\textrm{mod max}}\right)$
</left>
<right>
* Occupied bandwidth: deviation and maximum modulating frequency
* With small deviation and a low modulating frequency $\rightarrow$ *Carson's rule*
* Higher modulating frequency or greater deviation $\rightarrow$ larger bandwidth
* Adjacent-channel interference is possible
</right>

<note>
About 99% of the transmit power lies within the bandwidth
</note>
---
[question:AE306]
---
[question:AE307]
---
[question:AE304]
---
[question:AE309]
---
#### Solution
* given: $f_{\textrm{mod max}} = \qty{2}{\kilo\hertz}$
* given: $\Delta f_{\textrm{T}} = \qty{1.8}{\kilo\hertz}$
* required: $B$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ &= 2 \cdot (\qty{1.8}{\kilo\hertz} + \qty{2}{\kilo\hertz}) = \qty{7.6}{\kilo\hertz} \end{split}$
</fragment>
---
[question:AE308]
---
#### Solution
* given: $f_{\textrm{mod max}} = \qty{2.7}{\kilo\hertz}$
* given: $\Delta f_{\textrm{T}} = \qty{2.5}{\kilo\hertz}$
* required: $B$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ &= 2 \cdot (\qty{2.5}{\kilo\hertz} + \qty{2.7}{\kilo\hertz}) = \qty{10.4}{\kilo\hertz} \end{split}$
</fragment>
---
[question:AE311]
---
#### Solution
* given: $B = \qty{10}{\kilo\hertz}$
* given: $\Delta f_{\textrm{T}} = \qty{2.5}{\kilo\hertz}$
* required: $f_{\textrm{mod max}}$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ \Rightarrow f_{\textrm{mod max}} &= \frac{B}{2} - \Delta f_T\\ &= \frac{\qty{10}{\kilo\hertz}}{2} - \qty{2.5}{\kilo\hertz} = \qty{2.5}{\kilo\hertz} \end{split}$
</fragment>
---
[question:AE312]
---
#### Solution
* given: $B = \qty{10}{\kilo\hertz}$
* given: $f_{\textrm{mod max}} = \qty{2.7}{\kilo\hertz}$
* required: $\Delta f_{\textrm{T}}$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ \Rightarrow \Delta f_T &= \frac{B}{2} - f_{\textrm{mod max}}\\ &= \frac{\qty{10}{\kilo\hertz}}{2} - \qty{2.7}{\kilo\hertz} = \qty{2.3}{\kilo\hertz} \end{split}$
</fragment>
---
[question:AE310]