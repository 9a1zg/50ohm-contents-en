The data rates achievable in practice differ considerably depending on the transmission method and the propagation conditions. Under optimum conditions, Wi-Fi and 5G support data rates up to the range of gigabits per second. FT8, on the other hand, can be used even under poor conditions, but transmits only a few bits per second.

Which data rate can be achieved depends on the usable bandwidth and the signal-to-noise ratio ($P_\text{S}/P_\text{N}$). From these two quantities, the Shannon–Hartley theorem can be used to calculate the theoretical maximum data rate achievable on a transmission channel:

$C=B \cdot \log_2 \left(1+{\dfrac{P_\text{S}}{P_\text{N}}}\right) \unit{\bit\per\second}$

[question:AE416]

---

An easily remembered value arises at a signal-to-noise ratio of $\qty{0}{\dB}$. Here the bandwidth in $\unit{\hertz}$ is exactly equal to the maximum achievable data rate in $\unit{\bit\per\second}$. Poorer signal-to-noise ratios allow correspondingly lower data rates, better signal-to-noise ratios higher data rates. With this memory aid, the corresponding examination questions can be answered quickly, without a long calculation.

<margin>
If we substitute $\frac{P_\text{S}}{P_\text{N}} = \qty{0}{\dB}$, that is, the factor $\num{1}$, we get:
  
$\begin{split} C&=B \cdot \log_2 \left(1+1\right) \unit{\bit\per\second}\\ C&=B \cdot \log_2 \left(2\right) \unit{\bit\per\second}\\C &= \qty{B}{\bit\per\second}\end{split}$
</margin>

---

If considerably more bits per second are to be transmitted than there is bandwidth available in $\unit{\hertz}$, the required signal-to-noise ratio rises sharply. Over narrowband links on HF, therefore, practically no high data rates can be achieved. Hamnet, for example, as a fast data network, is usually operated in the upper UHF and lower SHF ranges, where greater bandwidths are available.

<indepth>
Only the noise energy that lies within the bandwidth used is considered here. Some computer programs, on the other hand, use the noise energy of a $\qty{2.4}{\kilo\hertz}$ wide channel, even if the actual wanted signal is considerably narrower; this, however, is a different quantity, which cannot be substituted directly into the formula of the Shannon–Hartley theorem.
</indepth>

By lowering the data rate, on the other hand, methods can be developed that not only need a small bandwidth, but also still work at an extremely poor signal-to-noise ratio.  Examples of this are digital transmission methods such as WSPR or FT8, which exchange only a few characters per unit of time. This makes it possible, even in poor propagation conditions, to convey at least a short message.

[question:AE417]
[question:AE418]
[question:AE420]
[question:AE419]

Note that the Shannon–Hartley theorem only sets an upper limit for the achievable data rate. The data rates actually achievable are always below it. Only by means of good error correction methods, which we will meet later, is it possible to approach this upper limit. 
