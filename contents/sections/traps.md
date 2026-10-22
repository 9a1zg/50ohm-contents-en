We have already met multiband antennas that are deliberately resonant on several bands, e.g. the end-fed antenna with a 1:49 transformer. Let us return to our example from the second section on current and voltage feeding: in principle, a centre-fed half-wave dipole can be resonant not only at its fundamental frequency but also at odd multiples of that frequency. For example, a dipole designed for the $\qty{80}{\meter}$ band with a fundamental frequency of $\qty{3.5}{\mega\hertz}$ has further resonances at approximately $\qty{10.5}{\mega\hertz}$ and $\qty{17.5}{\mega\hertz}$.

At even multiples of the fundamental frequency, on the other hand, for example at $\qty{7}{\mega\hertz}$ or $\qty{14}{\mega\hertz}$, there is a current minimum at the central feed point, and so a high impedance. These frequencies therefore cannot readily be used with a simple centre-fed dipole. One way of producing additional resonances on such frequencies deliberately is the *trap dipole*.

In a trap dipole, each half of the dipole contains at least one parallel tuned circuit made up of a coil and a capacitor. Such a tuned circuit is called a *trap*. A parallel tuned circuit has a high impedance at its resonant frequency (see Figure [ref:a_sperrkreis]). It then acts as a *rejector* and largely prevents current from flowing into the outer part of the dipole. This allows the same dipole to have different electrical lengths on several frequency bands.

<margin>
[picture:1036:a_sperrkreis:Qualitative frequency response of a parallel tuned circuit (rejector)]
</margin>

[question:AG109]
[question:AG110]

---

How a trap affects the dipole depends on where the operating frequency lies in relation to the trap's resonant frequency $f_\mathrm{res}$.

* At $f=f_\mathrm{res}$, the parallel tuned circuit has a high impedance and acts as a rejector. The outer part of the dipole is thereby largely separated from the inner part.
* At $f<f_\mathrm{res}$, the inductive effect of the trap predominates. It acts much like a loading coil and lengthens the radiator electrically.
* At $f>f_\mathrm{res}$, the capacitive effect of the trap predominates. This shortens the radiator electrically to some extent.

<margin>
In this applet you can explore the effect of a trap on a dipole at different frequencies:

[include:applet_traps]
</margin>

The resonant case is the easiest to picture first. If the dipole is operated at the resonant frequency of the trap (e.g. $\qty{7.05}{\mega\hertz}$ in our figure), the parallel tuned circuit has a high impedance. So only a little current flows into the outer part of the dipole. The dipole behaves approximately as if it ended at the position of the trap.

[question:AG112]

This relationship can be used in designing a dual-band dipole. For the higher-frequency band, the distance between the two traps essentially determines the effective length of the dipole. At this frequency, the blocking effect of the traps largely cuts off the outer wire sections, as if they were not there, and the dipole behaves like a shorter dipole.

[question:AG116]

---

If, on the other hand, the dipole is operated at a frequency *below* the resonant frequency of the trap (e.g. $\qty{3.5}{\mega\hertz}$ in our figure), the tuned circuit no longer has a high impedance. Its inductive effect predominates. The trap therefore acts much like a loading coil and lengthens the dipole electrically. As a result, the whole dipole, including the outer wire sections, can be used for a lower frequency band.

[question:AG111]

---

At a frequency *above* the resonant frequency, on the other hand, the capacitive effect of the trap predominates. The trap therefore shortens the antenna electrically, and it can even be resonant on, for example, $\qty{14}{\mega\hertz}$. This effect, too, should be taken into account when dimensioning a trap dipole.

[question:AG113]

---

With several pairs of traps, dipoles can be built for even more frequency bands. The traps for the highest frequencies are then furthest in, because these need the shortest effective dipole length.

The innermost trap is therefore tuned to the highest frequency intended. The next pair of traps further out is tuned to the next lower frequency, and so on. The lower the operating frequency, the larger the part of the dipole that is effective.

[question:AG115]
[question:AG114]

Traps are not used only in dipole antennas. In directional antennas such as Yagi antennas, too, traps can be used in the individual elements to make the antenna usable on several frequency bands.