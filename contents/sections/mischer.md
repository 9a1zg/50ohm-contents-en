With the help of a mixer, a particular frequency (or a frequency range of defined bandwidth) can be converted to a higher or lower frequency. To do this, the signals are multiplied together. 

<indepth>
Multiplying signals in the time domain leads to an addition (or subtraction) in the frequency domain. This relationship can be explained clearly with the following trigonometric identity (slightly simplified: the factors $2\pi\cdot t$ have been left out for clarity):  
  
$\sin(f_1)\cdot\sin(f_2) = \frac{1}{2}\left(\cos(f_1-f_2)-\cos(f_1+f_2)\right)$
  
If two sine signals are multiplied together – one at the frequency $f_1$ and one at the frequency $f_2$ – two new cosine signals are produced in the frequency domain (a cosine being nothing other than a phase-shifted sine). These lie at the frequencies $f_1 - f_2$ and $f_1 + f_2$. You can think of it as one frequency component being shifted down and another being shifted up. This is exactly the principle that the mixer makes use of.

In principle, two frequency components are always produced. In practice, however, usually only one of them is wanted, which is why suitable filters are used after the mixer to select the desired mixing product. Strictly speaking, negative frequencies can also occur when the difference is taken, which is why the magnitude $| f_1 \pm f_2 |$ is generally considered.
</indepth>

---

A mixer uses non-linear components, such as diodes, to multiply signals together. This produces so-called mixing products, whose frequencies correspond mathematically to the sum and the difference of the frequencies of the input signals.

Because of this property, mixers are used specifically to convert signals into other, desired frequency ranges – for example for up-conversion or down-conversion in transmitters and receivers. In block diagrams, a mixer is represented, as shown in Figure [ref:e_mischer], by a circle containing a multiplication sign, which indicates the multiplicative action of this module.

<margin>
[picture:903:e_mischer:Mixer]
</margin>

---

The frequencies produced at an output of a mixer consist mainly of the two mixing products of the signals fed in: $f_\text{e}$, the input signal, and $f_\text{o}$, the signal that comes from an oscillator. This gives two wanted mixing products, the sum and the magnitude of the difference of the signals fed in:

$f_\text{z}=|f_\text{e}\pm f_\text{o}|$

Because of the $\pm$, two cases have to be distinguished: this gives $f_\text{z1} = f_\text{e}+f_\text{o}$ and $f_\text{z2}=|f_\text{e}-f_\text{o}|$.

The vertical bars $|x|$ mean that only the numerical value without its sign is considered. If $x$ is negative, it is made positive. If $x$ is already positive, it stays as it is.

Normally only one of the wanted mixing products is used for further signal processing. The other mixing product (and any further unwanted mixing products – see the in-depth section) must then be removed from the mixture of signals by filtering.

<indepth>
Besides the wanted mixing products, a real mixer also produces higher-order mixing products such as $2 * f_\text{in1} + f_\text{in2}$ etc. These unwanted mixing products must also be removed afterwards by suitable filters. In real mixers, the two input frequencies are not completely suppressed in the output signal either, and must be taken into account in further signal processing. By using a balanced ring mixer, the two input signals can be suppressed very strongly in the output signal, which is why this type of mixer is widely used.
</indepth>

[question:EF201]

In this question we simply have to add the oscillator frequency once and subtract it once, taking the magnitude into account.

$f_\text{z1} = f_\text{e}+f_\text{o} = \qty{21}{\mega\hertz} + \qty{31.7}{\mega\hertz} = \qty{52.7}{\mega\hertz}$

$f_\text{z2}=|f_\text{e}-f_\text{o}| =|\qty{21}{\mega\hertz} - \qty{31.7}{\mega\hertz}| = |\qty{-10.7}{\mega\hertz}| = \qty{10.7}{\mega\hertz}$

The following questions work on the same principle.

[question:EF202]
[question:EF203]
[question:EF204]
[question:EF205]

Since all kinds of frequencies are produced in mixers by the mixing process, *mixer stages must always be very well screened*, so that they cannot radiate into other stages or equipment and, above all, do not cause interference to other radio services!

[question:EF206]