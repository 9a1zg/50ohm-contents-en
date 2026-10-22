A major advantage of processing signals digitally is that information in digital form can be manipulated in almost any way. A sequence of input samples is converted into a sequence of output samples by means of mathematical functions. Simple digital filters, such as low-pass, band-pass or high-pass filters, can be implemented in two different ways: as FIR and as IIR filters. FIR stands for *finite impulse response* and IIR for *infinite impulse response*.

The main feature of FIR filters, as the name "finite" already says, is that only a limited number of input samples is used to compute an output sample. IIR filters, on the other hand, also use output samples that have already been computed, which are fed back to the input of the computation. Because of this feedback, a single input sample can in theory influence the following output samples for an unlimited length of time.

Digital filters can be implemented either in software on a DSP or in programmable hardware on an FPGA. In addition, there are what are known as mixed-signal front ends, which implement various signal processing functions, such as decimation filters, together with A/D and D/A converters on one chip, in order to carry them out as energy-efficiently as possible and to relieve the load on the following signal processing stages.

[question:AF631]

<indepth>
[picture:1133:a_fir:FIR filter]

Figure [ref:a_fir] shows the structure of an FIR filter schematically. An input sample is written into an input memory. With each clock cycle the stored values are shifted on by one memory location, as in a shift register. The taps of the individual memory locations are multiplied by the corresponding filter coefficients and then added up. The result is output as the output sample.

Assuming that the four filter coefficients each have the value $\frac{1}{4}$, the last four input samples are each multiplied by $\frac{1}{4}$ and then added up. The output sample is thus the mean of the last four input samples. Such a filter is also called a *moving average*.

An input sequence $0,0,0,4,0,0,0,0$ thus leads to the output sequence $0,0,0,1,1,1,1,0$.

The filter thus smooths fast changes, i.e. high-frequency components of the input signal. Slow changes, or low frequencies, are largely passed, while fast changes, or high-frequency components, are attenuated. A moving average therefore acts as a very simple digital low-pass filter.

The filter carries out what is known as a convolution, which, incidentally, is also the basis of many of the neural networks that drive artificial intelligence.
</indepth>