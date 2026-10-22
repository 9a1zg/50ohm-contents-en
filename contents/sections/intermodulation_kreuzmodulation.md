In a receiver with two strong RF signals present at its input, interference can be caused by intermodulation or cross-modulation.
With intermodulation, the effect is that additional unwanted frequencies are produced by non-linear behaviour of the receiver stage (operation at the edge of its range, in the non-linear region), much as in a mixer. These can be superimposed on wanted received signals and interfere with them.
With cross-modulation, the effect is that the wanted received signal is affected by the modulation of a strong AM signal close to it in frequency. As a result, the modulation of the adjacent transmitter becomes audible in the received signal and interferes with it.

[question:AF217]
[question:AF219]
[question:AF222]
[question:AF218]

To suppress a strong unwanted signal before it reaches the receiver input, an acceptor circuit, tuned to the exact frequency of the interfering signal and placed ahead of the receiver input, can for example provide a remedy.

[question:AF223]

The strong-signal performance of a receiver can be described by the so-called third-order intercept point (IP3). It is a measure of the point at which unwanted 3rd-order mixing products reach the amplitude of the input signal. The higher the IP3 of a receiver, the larger the signals it can still process without interference.

<indepth>
In this in-depth section we look at the IP3 as a parameter for the strong-signal performance of a receiver. In general, mixing products are produced by non-linearities in amplifiers, mixers or other receiver stages. With two input signals $f_1$ and $f_2$, intermodulation products of the form

$f_\text{mix} = \left| m \cdot f_1 \pm n \cdot f_2 \right|$

can be produced, where $m,n \in \mathbb{N}_0$ and the two coefficients must not both be zero at the same time. The order of such a mixing product is the sum of the coefficients:

$\text{order} = m+n$

The 3rd-order intermodulation products are particularly critical, because they often lie close to the original input signals again. They can therefore fall within the wanted receive range, and are then difficult or impossible to remove with subsequent filters.

Figure [ref:a_intermodulation] below shows the intermodulation of two signals $f_1$ and $f_2$. The 3rd-order intermodulation products are particularly highlighted:

[picture:1095:a_intermodulation:Intermodulation of two signals $f_1$ and $f_2$]

The important point is that these intermodulation products are not received from outside, but only arise in the receiver through non-linear behaviour. A two-tone test can be used to examine the linearity of a receiver. Two defined input signals are fed in for this. If, besides these two fundamental signals, 3rd-order intermodulation products also appear in the spectrum, for example on the waterfall display, this is an indication of non-linear behaviour.

Figure [ref:a_zweitontest] shows a two-tone test with a power sweep, in which the 3rd-order intermodulation products become clearly visible.

[picture:1096:a_zweitontest:Two-tone test with power sweep]

If the output power is plotted against the input power, the fundamental signals rise in the linear region with a slope of $1{:}1$. The 3rd-order intermodulation products, on the other hand, rise with a slope of $3{:}1$. If the linear regions of these two curves are extended, they meet at a theoretical point of intersection. This point is called the IP3, i.e. the 3rd-order intercept point.

The IP3 thus describes the extrapolated point at which the 3rd-order intermodulation products would, by calculation, reach the same output power as the fundamental signals. In practice this point is usually not reached, because the receiver goes into compression or saturation before then.

The higher the IP3 of a receiver, the better its strong-signal performance. A high IP3 means that even strong adjacent signals can be handled without interfering intermodulation products arising in the wanted receive range.
</indepth>

[question:AF221]

To reduce the formation of unwanted mixing products by strong signals at the receiver input, a switchable attenuator can be inserted ahead of the receiver input. This reduces intermodulation products and cross-modulation in the receiver. The wanted signal is reduced only by the factor of the attenuator – but, because of the mathematics of the mixing process, interfering mixing products are attenuated by a factor of $\num{3}$ (3rd order) in $\unit{\dB}$. For example, a $\qty{10}{\dB}$ attenuator reduces the wanted signal by only $\qty{10}{\dB}$, while unwanted mixing products are already attenuated by $\qty{30}{\dB}$.

[question:AF220]