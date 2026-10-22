<margin>
[picture:804:mischer_linear_vs_nichtlinear:Linear resistor and non-linear diode]
</margin>


Components and modules can behave *linearly* or *non-linearly*. In a linear component, the output quantity follows the input quantity according to a fixed relationship. An ideal resistor, for example, has a linear characteristic. The characteristic of a diode, on the other hand, is non-linear (see Figure [ref:mischer_linear_vs_nichtlinear]).

Purely linear behaviour is not enough for a mixing process. When several signals pass through a linear circuit, they can be amplified, attenuated or added together, but they do not influence one another. No new frequency components are produced.

For mixing to take place, the input signals must be combined with one another. This can happen, for example, through the non-linear characteristic of a diode or a transistor. Another frequently used way is to switch the input signal on and off rapidly, or to reverse its polarity, with the help of the oscillator signal. Such a switching process is not a linear process either, and it causes the two signals to be combined.

It is precisely this property that is deliberately exploited in a mixer. That is why mixer stages work with non-linear components, or with circuits in which transistors or diodes are switched by the oscillator signal.
In practice, however, many unwanted higher-order mixing products are also formed, which have to be suppressed deliberately by technical measures such as filtering.

[question:AF212]

The aim of a mixer is that ideally only the wanted mixing products appear at its output, and that unwanted mixing products and the input signals are suppressed as far as possible.

This aim is best achieved with a so-called balanced mixer. It is built with 4 diodes or transistors in a ring circuit (see Figure [ref:mischer_ringmischer]). Because of the resulting balanced design, the input signals are suppressed as far as possible at the output. Other types of mixer, such as two-diode mixers, dual-transistor mixers and additive diode mixers, always pass one of the input signals through to the output as well, because of their unbalanced design.

<indepth>
How a ring mixer works:

The local oscillator ($U_2$ in the diagram) always switches two opposite diodes into conduction during one half cycle, while the other two diodes are cut off. In the next half cycle of the local oscillator, the situation is exactly reversed. For this, the amplitude of the local oscillator ($U_2$) must be high enough for the diodes to be driven sufficiently into conduction during the positive and negative half cycles.

As a result, the diode ring acts as a polarity reverser for the signal applied to the input ($U_1$).
To achieve a good mixing result in terms of unwanted mixing products and suppression of the input signal, its amplitude must be considerably smaller than the amplitude of the local oscillator.
Optimum values are achieved by so-called high-level ring mixers, whose LO input levels can be in the range of up to $\qty{10}{\milli\watt}$.

<webonly>
[include:applet_ringmodulator]
</webonly>
<latexonly>
[picture:805:mischer_ringmischer:Balanced mixer, ring mixer or ring modulator]
</latexonly>
</indepth>

<tip>
It is important to be able to tell the ring mixer apart from the circuit of a diode rectifier, which looks very similar: in the ring mixer the diodes are connected one after the other to form a ring (each cathode connected to the anode of the following diode). In the rectifier, on the other hand, 2 cathodes and 2 anodes are always connected together.
</tip>
  
The balanced mixer, which is also called a ring mixer or ring modulator, is the best suited for suppressing unwanted output signals.

[question:AF213]
[question:AF214]
