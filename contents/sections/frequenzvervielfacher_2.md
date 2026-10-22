In Class E we have already met frequency multipliers at block-diagram level. In Class A we want to understand how they work.

Diodes and transistors have a non-linear characteristic. If they are driven with a sinusoidal signal, the signal is distorted as a result. As we have already learnt, such non-linear processes produce harmonics. A frequency multiplier makes deliberate use of this effect: the input signal is first distorted non-linearly, so that numerous harmonics are produced. The desired harmonic is then selected with a tuned circuit or filter and used as the output signal.

Technically, a frequency multiplier is implemented by first feeding the input signal to a non-linear distorting stage. This can be, for example, a class C amplifier, which we will discuss later in this chapter. The desired harmonic of the signal is then selected from the mixture of signals by means of filters and passed on to the next stage. Since frequency multiplication is based on harmonics, only integer multiples of the fundamental frequency are possible. In practice (with a few exceptions) only the 2nd harmonic or the 3rd harmonic of the fundamental frequency is used (doubling, tripling).
To achieve higher multiplication factors, doubling or tripling stages are therefore connected one after the other, so that their factors multiply.

[question:AF311]

Frequency multiplication, possibly in several stages connected one after the other, produces frequency products that can often lead to interference. Frequency multiplier stages must therefore be very well screened, to reduce unwanted radiation as far as possible.

[question:AF313]

A typical multiplier circuit (see Figure [ref:a_frequenzvervielfacher_schaltung]) contains an amplifier stage that is deliberately operated without base bias. This produces an amplifier in class C operation, which heavily distorts the input signal and at whose output the signal is taken off by means of filters. The filters used for this are tuned circuits that resonate on the desired frequency and are usually tunable.

<margin>
[picture:489:a_frequenzvervielfacher_schaltung:Example of a frequency multiplier circuit with a class C amplifier without base bias]
</margin>

[question:AF312]

If several multiplier stages are connected one after the other in a piece of equipment, interference can occur on the frequencies produced between the individual multiplier stages. To determine these frequencies, you have to trace the path of the signal through the individual stages and calculate the frequencies present after each of them. The order of the multiplier stages is therefore crucial in determining interference frequencies, because only certain frequencies are mathematically possible.

[question:AF314]
