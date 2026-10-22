The *frequency accuracy* states how far a generated, set or measured frequency can deviate from its actual value. It is often given in per cent ($\unit{\percent}$), in *parts per million* ($\unit{\ppm}$) or directly as a relative deviation.

The following applies:

$\qty{1}{\percent} = 1 \cdot 10^{-2}$

and

$\qty{1}{\ppm} = 1 \cdot 10^{-6}$

With a frequency counter, the achievable accuracy depends essentially on its *timebase*. The frequency counter determines the frequency of the input signal with the help of an internal reference frequency. If this reference deviates from its nominal value, the deviation affects the result of the measurement accordingly.

Oscillators that are as stable as possible are therefore used as the timebase. High-quality frequency counters use, for example, a TCXO or OCXO. For particularly accurate measurements, an external frequency reference can often be connected as well, for example a GPS-disciplined oscillator (GPSDO).

If the relative frequency accuracy is known, the maximum frequency error to be expected can be calculated from it:

$\Delta f = f \cdot a$

Here $f$ is the frequency in question and $a$ the relative frequency accuracy.

<indepth>
  Note on converting and writing powers of 10:
  
  $1 \cdot {\num{10^{-2}}} = \frac{1}{\num{10^2}}$
  $1 \cdot {\num{10^{-6}}} = \frac{1}{\num{10^6}}$
  
  and so on.
</indepth>
  
[question:AA115]

[question:AA116]

[question:AI508]

[question:AI509]

[question:AI510]

[question:AI506]

[question:AI507]
