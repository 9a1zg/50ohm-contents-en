A method that has been known for decades has for some time been used increasingly in amateur radio: *polar modulation* [index:Polar modulation].

There is no examination question on this topic. But polar modulation is an exciting method that will be used more and more in amateur radio equipment in the future. It is therefore briefly introduced here, as a look beyond the syllabus. If you only want to learn the examination material, you can safely skip this topic.

Polar modulation is based on the observation of what happens when you zoom in, in time, on any signal of reasonably narrow bandwidth: the individual cycle looks like a sine wave.

This sine wave is defined by a few numbers, namely frequency, phase and amplitude.  Frequency and phase, though, are coupled to each other: if you start with a particular base frequency but then shift the phase again and again in the same direction with every cycle, you end up at a different, offset frequency.

These considerations give rise to the method of *polar modulation*.  It can be used to generate any signal of reasonably narrow bandwidth, SSB signals for example. All that is needed is that, starting from a base frequency, the phase and amplitude of the signal can be controlled at the same time.

Figure [ref:polar_modulator] shows the block diagram with which this idea is usually implemented today. The two signal components $I(t)$ and $Q(t)$ (as described in the previous chapter) are converted into the instantaneous amplitude $A(t)$ and the instantaneous phase $\varphi(t)$:

$A(t)=\sqrt{I^2(t)+Q^2(t)}$

$\varphi(t)=\operatorname{atan2}\left(Q(t),I(t)\right)$

The phase information $\varphi(t)$ then modulates an RF carrier whose amplitude is, to begin with, constant. The resulting signal, still of constant amplitude, thus already contains the complete phase information. It can be amplified by a particularly efficient switching amplifier, for example a class E amplifier. In practice, such output stages often reach efficiencies of more than $\qtyrange{80}{90}{\percent}$.

But how does the amplitude modulation come into the picture? For this, the supply voltage of the output stage is simply manipulated accordingly. The amplitude information $A(t)$ is impressed on it by an envelope amplifier. As a result, the output amplitude changes in line with the amplitude needed at that moment, and the desired envelope results. At the output, the complete amplitude- and phase-modulated signal appears once more:

$s(t)=A(t)\cos\left(\omega_\mathrm{T}t+\varphi(t)\right)$

For the signal to remain as free from distortion as possible, the amplitude path and the phase path must be precisely aligned with each other in time.

A relatively slow AF amplifier is enough for the envelope amplifier. The frequency range it has to cover depends on the bandwidth of the signal to be generated. To keep the efficiency high, switch-mode power supply technology is usually used here ("class D" AF amplifiers).

Because of the high efficiency, little electrical power is converted into heat. This saves energy, reduces the need for cooling and makes smaller and lighter radios possible, without large metal heatsinks and with cheaper output transistors. Polar modulation is particularly suitable for battery-powered QRP radios, but is also used in more powerful commercial transceivers.

<indepth>
In amateur radio, the method was first used in the 1970s, under the name "HELAPS", on the AO-7 satellite. At that time everything was done by analogue means. Today the envelope amplifier and the output stage are still conventionally analogue, and SDR algorithms do the rest of the work. Powerful CPUs that handle the tasks involved with ease are cheaper than a pizza these days.
</indepth>

<margin>
[picture:1117:polar_modulator:Polar modulator]
</margin>
