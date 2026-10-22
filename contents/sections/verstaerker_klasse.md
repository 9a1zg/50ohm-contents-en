As we have seen in the previous sections, transistors have a characteristic that shows the relationship between the input signal (base-emitter or gate-source voltage) and the output signal (collector or drain current). Within the characteristic there are different regions in which the transistor behaves linearly or non-linearly. Regions of the characteristic in which a change in the control quantity produces a proportional change in the output quantity are called linear. On linear axes, these regions can be recognised by their straight course, without any curvature. Other regions of the characteristic, in which a change in the control quantity does **not** produce a proportional change in the output quantity, are called non-linear.

<margin>
[picture:1085:a_kennlinien_transistor_arbeitspunkt:Simplified input characteristic of a transistor with different operating points]  
</margin>

The bias at the base or at the gate first sets the quiescent operating point of the transistor. Together with the size of the input signal, this determines over which region of the characteristic the transistor is driven and for what proportion of a signal period current flows. This gives the amplifier classes A, AB, B and C, with different properties in terms of efficiency, linearity, conduction angle and harmonic content. Figure [ref:a_kennlinien_transistor_arbeitspunkt] shows the typical quiescent operating points of the different amplifier classes for class A, B, AB and C operation. Through the design of the amplifier circuit as a whole, their respective advantages and disadvantages can be deliberately exploited or partly compensated for. In what follows, we will look at the different amplifier classes. 

[question:AD416]

---

% A-Betrieb des Verstärkers:

In *class A operation*, the operating point is chosen so that the transistor remains conducting throughout the signal period (conduction angle $\qty{360}{\degree}$). For the largest and most symmetrical drive possible, the quiescent operating point is often placed roughly in the middle of the load line, that is, between cut-off and saturation, so that the transistor works entirely in the linear region. The input signal (see Figure [ref:a_eingangsspannung]) is then amplified around the desired operating point, which defines the centre of the working range. The choice of operating point results in a corresponding quiescent current ($I_\mathrm{A}$) of the transistor (see Figure [ref:a_ausgangsstrom_a]). This flows even when no input signal is present. The quiescent current has a major influence on how efficient an amplifier is, since it increases the power the amplifier dissipates as heat and so reduces its efficiency. In class A operation this typically gives an efficiency of approx. $\eta = \qty{40}{\percent}$, which is a good value for a linear amplifier. The harmonic content in class A operation is very low, since the transistor works entirely in the linear region.

All signals whose modulation information is contained in their amplitude must, as a rule, be amplified linearly so that the information is transmitted without distortion (SSB, AM etc.). There are, however, also circuit techniques that make linear class A operation not strictly necessary. Signals whose modulation information is contained not in the amplitude but only in the frequency can also be amplified in the non-linear region of an amplifier (FM etc.) and filtered afterwards.

Summary of class A operation:

- Efficiency approx. $\qty{40}{\percent}$
- very low harmonic content
- Well suited to AM and SSB
- An output current flows over the entire period (conduction angle $\Theta =\qty{360}{\degree}$) of the input signal

<margin>
[picture:1086:a_eingangsspannung:Example of an RF input voltage $U_\mathrm{BE}$ of a transistor]
[picture:1087:a_ausgangsstrom_a:Example of an RF output current $I_\mathrm{C}$ of a transistor in class A operation]
</margin>

[question:AD419]

% B-Betrieb des Verstärkers:

If the operating point is chosen for *class B operation*, the transistor ideally sits exactly at the cut-off point. Practically no quiescent current therefore flows when there is no input signal. With a sinusoidal drive, as shown in Figure [ref:a_eingangsspannung], the transistor only starts to conduct above a certain input voltage. A single transistor is therefore active only during one half cycle, that is, over a conduction angle of $\qty{180}{\degree}$.
Since almost no power is drawn in the quiescent state, the theoretical efficiency of an ideal class B amplifier can be up to around $\qty{80}{\percent}$. The current waveform of a single transistor, however, is no longer sinusoidal and therefore has a high harmonic content. 

To reduce or suppress harmonics, there are various solutions in practice:

- One possibility is a *push-pull* circuit with two transistors, as shown in Figure [ref:a_gegentakt]. Each transistor amplifies one half cycle, so that the two half cycles are put back together into a complete sine wave and the harmonic content is considerably reduced.
- Besides a push-pull stage, a tuned circuit can be used in narrowband RF amplifiers. The transistor supplies current pulses during one half cycle only. The tuned circuit stores energy and goes on oscillating between the current pulses, so that an almost sinusoidal signal over the complete period appears at the output again. Or, put another way: the tuned circuit acts like a filter that suppresses the harmonic components. This solution is suitable only for narrowband RF amplifiers, however, since a tuned circuit is resonant only over a narrow frequency range.

<margin>
[picture:1089:a_ausgangsstrom_b:Example of an RF output current $I_\mathrm{C}$ of a transistor in class B operation]
[picture:1091:a_gegentakt:Push-pull stage with two transistors, each amplifying one half cycle]
</margin>

Summary of class B operation:
- Small bias, up to the onset of collector current
- Quiescent current almost zero
- Efficiency up to approx. $\qty{80}{\percent}$
- Low harmonic content with a push-pull stage or a tuned circuit
- Conduction angle of $\Theta = \qty{180}{\degree}$, i.e. only one half cycle is amplified

[question:AD420]
[question:AD417]

---

% A/B-Betrieb des Verstärkers:

A further way of implementing an amplifier is class AB operation, in which the operating point lies between class A and class B operation. The quiescent current ($I_\mathrm{A/B}$) is larger than in class B operation, but considerably smaller than in class A operation, as shown in Figure [ref:a_ausgangsstrom_ab]. The efficiency is between $\qty{50}{\percent}$ and $\qty{80}{\percent}$, and with suitable circuit design the harmonic content is also low.

Summary of class AB operation of the amplifier
- Higher bias than in class B operation, but lower than in class A operation
- Quiescent current larger than in class B operation, but considerably smaller than in class A operation
- Efficiency between $\qty{50}{\percent}$ and $\qty{80}{\percent}$
- Low harmonic content
- Conduction angle: $\qty{180}{\degree} < \Theta < \qty{360}{\degree}$

Overdriving must be avoided, particularly in class AB or class B operation of an amplifier, since it can quickly lead to distortion of the signal. With SSB this shows itself as splatter on adjacent frequencies.
[question:AD423]

<margin>
[picture:1088:a_ausgangsstrom_ab:Example of an RF output current $I_\mathrm{C}$ of a transistor in class AB operation]
</margin>

---

% C-Betrieb des Verstärkers:

So-called *class C operation* is highly non-linear, because the transistor conducts only during a small part of the input cycle (see Figure [ref:a_ausgangsstrom_c]). The conduction angle is less than $\qty{180}{\degree}$, and ideally no quiescent current flows when there is no input signal. This makes high efficiencies of typically about $\qtyrange{80}{87}{\percent}$ possible.

Since the transistor produces only short current pulses, its output signal contains strong harmonic components. A tuned circuit or a filter following the stage selects the wanted output frequency and suppresses the unwanted harmonics. Since these harmonics can still carry considerable power inside the power amplifier and the filter, the circuit and its leads must be carefully constructed and screened so that no unwanted signals are radiated.

Class C operation is particularly suitable for signals with a constant envelope, for example FM and CW. Without additional measures it is unsuitable for AM and SSB, since the amplitude information would be distorted by the non-linear amplification. For this reason, class A, B or AB operation is normally used for AM and SSB amplifiers. With special techniques such as polar modulation, however, amplitude-modulated signals can also be produced with highly efficient, non-linear amplifiers. We will come back to this in more detail in a later section.

Summary: class C operation of the amplifier
- No bias
- Quiescent current zero
- Efficiency approx. $\qtyrange{80}{87}{\percent}$
- Produces the highest harmonic content of all the amplifier classes
- Conduction angle of $\Theta < \qty{180}{\degree}$, i.e. only a small part of the sine wave is amplified

<margin>
[picture:1090:a_ausgangsstrom_c:Example of an RF output current $I_\mathrm{C}$ of a transistor in class C operation]
</margin>

[question:AD418]
[question:AD425]
[question:AD421]
[question:AD422]
[question:AJ218]
[question:AF402]
[question:AF403]

Let us sum up the amplifier classes we have learnt once more in an overview:

| l: Property | X: Class A | X: Class B | X: Class AB | X: Class C |
| Quiescent current | $I_\mathrm{A}$ | 0 | $I_\mathrm{A/B}$ | 0 |
| Efficiency | $\qty{40}{\percent}$ | up to $\qty{80}{\percent}$ | $\qtyrange{50}{80}{\percent}$ | $\qtyrange{80}{87}{\percent}$ |
| Conduction angle | $\Theta = \qty{360}{\degree}$ | $\Theta = \qty{180}{\degree}$ | $\qty{180}{\degree} < \Theta < \qty{360}{\degree}$ | $\Theta < \qty{180}{\degree}$ |
| Measures against harmonics | Filter | Push-pull stage or filter | Push-pull stage or filter | Filter |

The output power of an amplifier can be roughly calculated from a knowledge of the operating point and hence of its approximate efficiency. To do this, you first calculate the DC power supplied to the amplifier as the product of voltage and current. You then multiply this power by the efficiency expressed as a numerical factor, where $\qty{100}{\percent}$ corresponds to an efficiency of $1$. An efficiency of $\qty{40}{\percent}$, for example, then corresponds to a factor of $0.4$. Now try to solve the following problems:

[question:AD424]

Besides the classic amplifier classes A, B, AB and C, there are other highly efficient amplifier classes, such as classes D, E and F. In class D and class E amplifiers, the transistor is deliberately operated as a switch, so that as little power as possible is lost in the transistor itself. Class F amplifiers additionally use networks tuned to the fundamental and to selected harmonics in order to shape the current and voltage waveforms at the transistor favourably. In this way very high efficiencies can be achieved. Such amplifiers, however, require careful circuit design and, at RF, are often suitable only for a limited frequency range. Other modes of operation, such as class J or class S, pursue similar aims but are not relevant to the amateur radio examination.