In phase modulation, the phase of a carrier wave is changed in accordance with the modulating signal. This means that the phase shift of the carrier wave varies in direct proportion to the amplitude of the modulating signal. This change in phase is kept as the signal goes on and varies in a particular pattern relative to the original carrier wave. The result is a sinusoidal signal whose "offset" (phase) is continuously adjusted, without the amplitude of the signal changing.

Phase modulation can be pictured as shifting the sine curve along the time axis, with every change in phase controlled by the modulating signal. The larger the amplitude of the modulating signal, the more the phase of the carrier signal shifts.

Phase modulation and frequency modulation both belong to the group of angle modulation techniques, since both affect the angle of the carrier wave. The difference is that frequency modulation directly affects the frequency, and phase modulation the phase.

This is particularly clear with a square-wave signal as the information signal: in phase modulation, each edge of the square wave causes an immediate phase jump in the carrier signal, whereas in frequency modulation the edge of the signal only triggers a change of frequency – the resulting change in phase arises only indirectly, by accumulating continuously over time.

<margin>
[picture:907:a_phasenmodulation:Phase modulation with reversal of the phase]
</margin>

<webonly>
<margin>
[include:applet_pm]
</margin>
</webonly>

<indepth>
For the mathematically minded: in phase modulation, the information signal $m(t)$ has a direct influence on the phase, e.g.: 

$\varphi(t) = m(t)$

The carrier signal is generated as a sine wave of the form

$s(t) = A_c \cos(2\pi f_c t + \varphi(t))$

where $A_c$ is the amplitude, $f_c$ the carrier frequency and $\varphi(t)$ the modulated phase.

The two types of modulation, FM and PM, are closely related: phase modulation of a signal indirectly results in a change of frequency, and conversely frequency modulation produces a change of phase. Mathematically, the relationship between frequency and phase can be expressed as follows:

$f_i(t) = \frac{1}{2\pi} \cdot \frac{d\varphi(t)}{dt}$

This means that the frequency is the time derivative of the phase.

So it is possible to achieve frequency modulation by means of phase modulation, by integrating the information signal $m(t)$:

$\varphi(t) = 2\pi \int m(t) \, dt$

The result is then substituted into the carrier function as $\varphi(t)$.
</indepth>

[question:AE313]