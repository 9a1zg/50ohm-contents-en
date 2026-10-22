*Direct digital synthesis*, or DDS for short [index:Direct digital synthesis] [index:DDS], is used to generate periodic signals whose frequency can be set very finely. Today it is often used in modern amateur radio equipment alongside frequency synthesis with PLL circuits. A major advantage of a DDS is that the output frequency can be set digitally with a very high resolution. In addition, it can switch very quickly between different frequencies, since no control loop has to lock on to a new frequency, as is the case with a classic PLL.

<margin>
[picture:1082:a_dds_aufbau:Block diagram of a DDS (direct digital synthesiser)]
</margin>

The basic structure of a DDS is shown in Figure [ref:a_dds_aufbau]. A clock generator produces a clock signal at a fixed frequency $f_\mathrm{Takt}$. With each clock cycle, a phase accumulator [index:DDS:Phase accumulator], also called an address counter for simplicity, increases its current phase value by the phase increment $K$:

$\varphi_{n+1} = \varphi_n + K$

The phase increment $K$ is also called the *tuning word*. It determines by how many phase steps the phase accumulator is advanced at each clock cycle. The current value of the phase accumulator serves as the address for a table of values, which is also called a *look-up table*. To generate a sine wave, this table contains the digital amplitude values of one complete period of a sine wave. For each phase value, the corresponding amplitude value is read out of the sine table. The size of the phase increment $K$ determines how quickly the sine table is stepped through, and hence the frequency of the output signal. The phase increment can be controlled by a microcontroller, for example. A register takes over the digital amplitude value in step with the clock signal and passes it on to a D/A converter. This converts the sequence of digital amplitude values into an analogue signal, which is stepped at first. A low-pass filter after it removes unwanted high-frequency signal components and smooths the output signal.

---

The following example illustrates this: with a phase increment of $K=1$, the phase value is increased by exactly one step with each clock cycle ($\varphi_{n+1} = \varphi_n + 1$). The sine table is thus stepped through entry by entry. Once a complete period has been generated, the address counter is reset and the phase accumulator starts again from the beginning. The resulting output signal is shown in Figure [ref:a_dds_phaseninkrement_k1].

<margin>
[picture:1083:a_dds_phaseninkrement_k1:Comparison signal]
</margin>

---

If the phase increment is doubled to $K=2$, the phase value increases by two steps with each clock cycle ($\varphi_{n+1} = \varphi_n + 2$). As a result, only every second phase value is called up and the sine table is stepped through twice as fast. The period of the output signal is halved and its frequency doubles. This is shown in Figure [ref:a_dds_phaseninkrement_k2].

<margin>
[picture:1084:a_dds_phaseninkrement_k2:Double the phase increment and double the output frequency]
</margin>

[question:AD620]

<indepth>
If the phase accumulator is $N$ bits wide, it can represent $2^N$ different phase values. When the largest value is exceeded, the counter overflows and starts again at the beginning:

$\varphi_{n+1} = \left(\varphi_n + K\right) \bmod 2^N$

This overflow corresponds to the transition from $\qty{360}{\degree}$ back to $\qty{0}{\degree}$. The phase increment $K$ can be chosen almost freely and need not be a power of two. This also makes it possible to generate output frequencies that are not the clock frequency divided by a whole number.

Moreover, a DDS is not limited to sine waves. If the table contains, for example, the amplitude values of a triangular or sawtooth wave, the DDS can also generate these waveforms.

The quality of the output signal depends mainly on the stability and the jitter [index:Jitter] of the clock generator, and on the resolution and linearity of the D/A converter. The limited number of phase and amplitude values gives rise to quantisation errors and additional spectral components. A low-pass filter after the converter suppresses a large part of these unwanted signal components.
</indepth>