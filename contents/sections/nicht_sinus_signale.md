An ideal, purely sinusoidal signal consists only of its *fundamental*, which is also called the *1st harmonic*. As soon as a signal no longer has the shape of a sine wave, even if it departs from it only slightly, the signal contains *integer multiples* of its fundamental, which are also called *overtones* (in German *Oberwellen* or *Oberschwingungen*). It is important here to distinguish between the two terms overtone and harmonic.

Figure [ref:zusammenhang_oberwellen_harmonische] and Table [ref:a_harmonische] show the relationship between overtones and harmonics, which you only need to memorise once. The 1st overtone corresponds to the 2nd harmonic of the fundamental and lies at twice the frequency of the fundamental. The 2nd overtone corresponds to the 3rd harmonic of the fundamental and lies at three times the frequency of the fundamental. On this principle, all harmonics and overtones are referred to the fundamental and numbered with an ordinal number $N$.

<margin>
[picture:869:zusammenhang_oberwellen_harmonische:Relationship between overtones and harmonics]

| l: Multiple of the fundamental frequency | l: Harmonic | l: Overtone |
| $f_0$ | 1 | ~ |
| $2 \cdot f_0$ | 2 | 1 |
| $3 \cdot f_0$ | 3 | 2 |
| $4 \cdot f_0$ | 4 | 3 |
[table:a_harmonische:Harmonics and overtones]
</margin>

<indepth>
Depending on the kind of distortion of a signal, relatively more even or more odd overtones appear in its frequency spectrum. Square-wave signals, which arise e.g. from overdriving amplifier stages (the peaks of the amplitude are limited and flattened), contain odd harmonics, that is, even overtones.

<webonly>
[include:applet_rectangle]

At the discontinuities the Fourier approximation shows what is known as the Gibbs phenomenon: even with a very large number of harmonics, a small overshoot and undershoot remains there.
</webonly>

Sawtooth signals contain mainly even harmonics, that is, odd overtones.
</indepth>

[question:AB403]
[question:AB401]
[question:AB402]

If the fundamental frequency of a signal is known, the frequency of the $N$th harmonic is found by multiplying the fundamental frequency by the ordinal number $N$:

$f_N = N \cdot f_0$

For the $N$th overtone, on the other hand:

$f_\mathrm{Oberwelle,N} = (N+1)\cdot f_0$

[question:AJ201]
[question:AJ205]
[question:AJ202]
[question:AJ206]

Even if a signal at first looks sinusoidal on the oscilloscope, it can still contain significant overtones (or harmonics of the fundamental). To assess the harmonic content of a signal quantitatively and qualitatively, you need a *spectrum analyser*, which can display the signal in the frequency domain and show the amplitudes of the individual harmonics on a logarithmic scale, so that their share of the total signal can be measured.

[question:AI615]
[question:AI614]
