In phase-shift keying (PSK), the different symbols are represented by different phases of a carrier. The amplitude and the frequency of the carrier stay the same. When the signal changes from one symbol to the next, however, the phase can change.

Figure [ref:a_psk] shows a PSK signal over time. At the symbol boundaries you can see that the oscillation continues with a different phase.

<margin>
[picture:705:a_psk:Phase-shift keying]
</margin>

---

The simplest form is binary phase-shift keying (BPSK). Here two different phases, and so two possible symbols, are available. For example, the phases $\qty{0}{\degree}$ and $\qty{180}{\degree}$ can be used and assigned to the bit values $0$ and $1$. Figure [ref:a_psk_mapping] shows a possible mapping of the two bit values to the two BPSK symbols.

Since the two symbols differ only in their phase and their amplitude is the same, the two points in the constellation diagram lie opposite each other on a circle.

<margin>
[picture:1101:a_psk_mapping:BPSK in the constellation diagram]
</margin>

<indepth>
Splitting hairs: strictly speaking, BPSK with the angles $\qty{0}{\degree}$ and $\qty{180}{\degree}$ can also be regarded as an ASK method in which the amplitude of the carrier signal is switched between a negative and a positive value. For a sine signal, multiplying by $-1$ results in a phase shift of $\qty{180}{\degree}$:

$-\sin(\omega t)=\sin(\omega t+\qty{180}{\degree})$

This is a special case. Other phase angles, such as $\qty{90}{\degree}$ and $\qty{270}{\degree}$, would also be possible, by the way; their two symbol phases would likewise be $\qty{180}{\degree}$ apart.
</indepth>

[question:AE401]

---

With more than two different phases, correspondingly more symbols can be represented. This allows several bits to be combined into one symbol.

---

In quadrature phase-shift keying (QPSK), four different phases, and so four possible symbols, are available. Since there are four possible combinations of two bits, two bits can be transmitted with each symbol.

For comparison:

* BPSK: $\num{2}$ symbols → $\num{1}$ bit per symbol
* QPSK: $\num{4}$ symbols → $\num{2}$ bits per symbol
* 8-PSK: $\num{8}$ symbols → $\num{3}$ bits per symbol

[question:AE402]

Let us now look at QPSK in the constellation diagram. The four possible symbols have the same amplitude but differ in their phase. All four signal points therefore lie on a circle. Figure [ref:a_qpsk] shows a possible mapping of the four bit combinations $00$, $01$, $10$ and $11$ to the four QPSK symbols.

<margin>
[picture:1059:a_qpsk:I/Q diagram for a QPSK mapping]
</margin>

---

In this example the following phases are used:

* $11$ corresponds to $\qty{45}{\degree}$
* $01$ corresponds to $\qty{135}{\degree}$
* $00$ corresponds to $\qty{225}{\degree}$
* $10$ corresponds to $\qty{315}{\degree}$

<margin>
The following applet illustrates digital QPSK modulation. In a real system, the signal is affected by noise and other interference. As a result, the received signal points do not lie exactly on the ideal positions, but deviate from them in both amplitude and phase. The applet simulates this by adding noise. The crosses mark the four ideal QPSK symbols. Each coloured dot is a noisy received value. The receiver assigns it to the nearest symbol. The coloured areas are the receiver's decision regions. As long as a noisy received value lies in the region of the symbol originally sent, the symbol is recognised correctly. If strong noise pushes a point across the boundary into a neighbouring region, the receiver decides on the wrong symbol. These errors can, however, be corrected by channel coding. We will deal with this in a later section.

[include:applet_qpsk]
</margin>

The four phases are each $\qty{90}{\degree}$ apart. From the phase it detects, the receiver can determine which symbol, and so which bit combination, was transmitted.

The assignment of the bit combinations to the individual phases is not fixed. To begin with, all that matters is that each symbol is assigned a unique bit combination.

In practice, the mapping is often chosen so that the bit combinations of neighbouring signal points differ in only one bit. Such an assignment is called a *Gray code*. If noise causes a neighbouring signal point to be detected by mistake, this then often leads to only a single bit error.

The constellation diagram thus makes an essential difference between ASK and PSK immediately visible: in ASK the symbols differ in their distance from the origin and usually lie only on the positive I axis, whereas in PSK they differ in their angle. In PSK the signal points therefore lie on a circle if the amplitude is the same.
