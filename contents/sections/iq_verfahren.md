In the previous section we saw that the information in a symbol can be represented, for example, by different amplitudes or frequencies. A further possibility is to change the phase of a signal. To show signal states with different amplitude and phase clearly, what is known as the *I/Q representation* is often used.

Let us first consider a signal state at the time $t=0$. An amplitude $A$ and a phase $\varphi$ are defined for the symbol. In a phasor representation, the amplitude determines the length of the phasor and the phase its angle to the horizontal axis.

The phasor can be split into a horizontal and a vertical component. The horizontal component is called $I$, for *in-phase component*, the vertical component $Q$, for *quadrature component*. For the signal state shown:

$I=A\cdot\cos(\varphi)$

$Q=A\cdot\cos(\varphi-\qty{90}{\degree})=A\cdot\sin(\varphi)$

If we let time run on, the phasor belonging to the oscillation rotates. Its projections on the two axes vary sinusoidally and are $\qty{90}{\degree}$ out of phase with each other. The applet shows this relationship between the oscillation and its I/Q representation.

[include:applet_iq_zeiger]

[question:AF633]

It helps to picture it like this: at the start of each symbol interval, the symbol value to be transmitted fixes a point in the I/Q plane, and with it the amplitude and the initial phase of the oscillation for this symbol. With the next symbol, the signal changes over to the signal state of the next point.

So, to represent the symbols, we are not interested in the continuous rotation of the phasor, but in the starting state fixed for each symbol. When the possible starting states are drawn as points in the I/Q plane (see [ref:a_iq_ebene]), this is called a *constellation diagram* (see Figure [ref:a_konstellationsdiagramm]). Each point corresponds to one possible symbol. The distance of a point from the origin describes the amplitude of the signal. Its angle to the I axis describes the phase.

<margin>
[picture:1060:a_iq_ebene:I/Q plane with one signal point]
[picture:1059:a_konstellationsdiagramm:Constellation diagram with 4 constellation points]
</margin>

<indepth>
For the mathematically minded: a sinusoidal oscillation can also be described mathematically as a *complex phasor* rotating at the angular frequency $\omega_\mathrm{c}$:

$s(t) = \Re\left\{A \cdot e^{j(\omega_\mathrm{c}t+\varphi)}\right\} = A\cos(\omega_\mathrm{c}t+\varphi)$

Here $A$ describes the amplitude and $\varphi$ the initial phase of the signal. The complex expression can be split into two parts:

$A \cdot e^{j(\omega_\mathrm{c}t+\varphi)} = \underbrace{A \cdot e^{j\varphi}}_{\text{amplitude and phase}} \cdot \underbrace{e^{j\omega_\mathrm{c}t}}_{\text{carrier}}$

In a constellation diagram we are interested in the first part, $A \cdot e^{j\varphi}$. It describes the amplitude and phase of the signal state. The continuous rotation of the actual carrier is not shown.
</indepth>

We will use this representation again and again in the following sections: it shows the possible symbols of digital modulation methods clearly, and later it will also be used to describe how bit combinations are assigned to these symbols.