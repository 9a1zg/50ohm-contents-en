<margin>
[picture:1019:e_frequenzabhängiger_widerstand:Frequency dependence of a capacitor and an inductor compared with a conventional resistor]
[picture:1020:e_herleitung_tiefpass:Deriving the low-pass circuit from a potential divider]
</margin>

In the chapters on capacitors and inductors we have already learnt that both components have a frequency-dependent resistance. Figure [ref:e_frequenzabhängiger_widerstand] shows qualitatively that the resistance of an ohmic resistor does not depend on frequency, while the resistance of a capacitor falls hyperbolically as the frequency rises and the resistance of an inductor rises linearly as the frequency rises.

These components can be used to build so-called passive frequency filters, which we will now look at more closely. In the first part of this chapter we deal with simple filters, namely high-pass and low-pass filters. These filters can be used to suppress unwanted frequency ranges above or below a cut-off frequency. In the second part we then turn to more complex filters, such as band-pass filters.

We begin by deriving a low-pass filter as a so-called *RC network*. The starting point, in step (1), is the potential divider circuit shown in Figure [ref:e_herleitung_tiefpass], which we have already met. Remember that the following applies to a potential divider: 

$\frac{U_1}{U_2} = \frac{R_1}{R_2}$

This means, for example: if resistor $R_2$ is twice as large as resistor $R_1$, then the voltage $U_2$ is also twice as large as the voltage $U_1$.

In step (2) we replace resistor $R_2$ with capacitor $C_1$. Then, in step (3), we redraw the circuit a little so that we obtain the usual way of drawing a low-pass filter.

---

Let us note: a low-pass filter is, to begin with, nothing other than a potential divider. That is why we can look at it in exactly that way from now on. Figure [ref:e_widerstaende_tiefpass] shows once more how the resistances vary with frequency. Let us first consider low frequencies: here the resistance of the capacitor is high, so that a high voltage is present at the output. As the frequency rises, the resistance of the capacitor becomes smaller and smaller, and by the principle of the potential divider the output voltage also falls.

This gives the voltage curve shown in Figure [ref:e_tiefpass_frequenzgang]. It also explains the core idea of the low-pass filter: high frequencies are heavily attenuated, while low frequencies pass through the filter largely unimpeded. One application of a low-pass filter is after transmitter amplifiers, to filter out the harmonics produced by distortion. 

<margin>
[picture:1021:e_widerstaende_tiefpass:Qualitative behaviour of the resistances in the low-pass potential divider]
[picture:1024:e_tiefpass_frequenzgang:Qualitative curve of the voltage $U_\text{A}$ at the low-pass filter]
</margin>

[question:ED208]
[question:ED201]

<indepth>
The *cut-off frequency* ($f_\text{g}$) of a low-pass filter is the frequency at which the output signal just begins to be noticeably weakened. It therefore marks the transition between the frequency range that the filter passes largely unimpeded and the range in which the attenuation increases markedly. Formally, the cut-off frequency is defined as the frequency at which the output power has fallen to half the input power ($\qty{-3}{\dB}$). Since power is proportional to the square of the voltage, this corresponds to the output voltage falling to about $\qty{70}{\percent}$ of its original value ($\frac{1}{\sqrt{2}}$). In practice, the cut-off frequency can therefore often be recognised as the point at which the output voltage becomes noticeably smaller and the frequency response begins to "bend". Below the cut-off frequency, low frequencies are passed almost unchanged; above the cut-off frequency, higher frequencies are increasingly attenuated.
</indepth>

---

With a high-pass filter, on the other hand, the low frequencies are heavily attenuated, while the high frequencies pass through this filter with hardly any attenuation. This is achieved by swapping the capacitor and the resistor, as shown in Figure [ref:e_widerstaende_hochpass]. The frequency response of a high-pass filter is shown qualitatively in Figure [ref:e_hochpass_frequenzgang]. One application of a high-pass filter is in an antenna splitter, for example to filter out the HF range ahead of a VHF receiver so as to avoid interference from HF operation.

<margin>
[picture:1025:e_widerstaende_hochpass:Qualitative behaviour of the resistances in the high-pass potential divider]
[picture:1022:e_hochpass_frequenzgang:Qualitative curve of the voltage $U_\text{A}$ at the high-pass filter]
</margin>

[question:ED211]
[question:ED202]

---

Simple RC networks have the disadvantage that their slopes are rather shallow around the cut-off. In addition, the lowest impedance of an RC low-pass filter is set by the resistor $R$. The resistor $R$ can, however, be replaced by an inductor, which behaves in the opposite way to a capacitor with frequency. It therefore makes sense to combine inductors and capacitors into high-pass and low-pass filters. 
At *high frequencies the resistance of the inductor is high*, while that of the capacitor is low.
At *low frequencies the resistance of the inductor is low*, while that of the capacitor is high. 
Depending on which component the output voltage is measured across, you get a high-pass or a low-pass filter. If you remember that the inductor's resistance $X_\text{L}$ is likewise high at high frequency, you can quickly identify a circuit as a high-pass or a low-pass filter by looking at which component the output voltage is measured across.

<tip>
For circuits with a capacitor and an inductor, too, the following simple rule applies: if the upper branch of the potential divider contains an upright *H* – as in *H*igh-pass – it is a high-pass filter. If, on the other hand, the upper branch contains a resistor or an inductor, it is a low-pass filter.
[picture:1023:e_hochpass_tipp:Memory aid]
</tip>

[question:ED209]
[question:ED212]

---

The following questions are about a practical application of our filters. Several frequency-dependent components can of course also be used in one circuit, so that the transition around the cut-off frequency becomes steeper. With the tip given above, you should now easily recognise which circuit is used in the following two questions. 

[question:ED210]
[question:ED213] 

Another practical example of inductors and capacitors chained together as a filter is the diplexer explained in the margin. 

<indepth>
*Practical example, the diplexer:* Passive high-pass and low-pass filters are also used in frequency splitters. The example below shows a circuit for a so-called diplexer for $\qty{2}{\meter}$ and $\qty{70}{\centi\meter}$. It can be used, for example, to operate a $\qty{2}{\meter}$ radio and a $\qty{70}{\centi\meter}$ radio on a shared dual-band antenna. Conversely, separate antennas for $\qty{2}{\meter}$ and $\qty{70}{\centi\meter}$ could be used with a VHF/UHF dual-band radio, for example an omnidirectional antenna for direct contacts on $\qty{2}{\meter}$ and a directional antenna for repeater operation on $\qty{70}{\centi\meter}$. 
Ahead of the $\qty{2}{\meter}$ output there is a low-pass filter, and ahead of the $\qty{70}{\centi\meter}$ output a high-pass filter, each made up of 5 frequency-dependent components. 
[picture:939:e_circuit_diplexer:Circuit diagram of a $\qty{2}{\meter}$/$\qty{70}{\centi\meter}$ diplexer]
[photo:171:e_example_diplexer:Example of a build]
</indepth>

<indepth>
[photo:320:e_tiefpass_selbstbau:Home-built low-pass filter]
The filters described above can of course be calculated and built yourself for any frequency range. The formula sheet contains the formulas you need, and there are of course also many construction designs and calculation programs. The inductors required can often be made easily yourself. For small inductance values, a small stock of $\qty{0.8}{\milli\meter}$ enamelled copper wire for rigid air-cored inductors is enough. For large inductance values, e.g. for the HF bands, you can manage with $\qty{0.2}{\milli\meter}$ enamelled copper wire and core material with suitable $A_\text{L}$ values, so that you can make the right values yourself at any time. The sizes, windings and so on that you need can usually also be worked out easily from the formula sheet, construction designs or calculation programs.
</indepth>  

---

We have now met simple RC and LC networks as high-pass and low-pass filters. Capacitors and inductors can, however, be used to make further types of filter that go beyond plain high-pass and low-pass filters. We now want to look at these more closely in the second part, namely the so-called *tuned circuits*.

<margin>
[picture:1026:e_rp_schwingkreis:(a) Series (b) parallel tuned circuit]
</margin>

In tuned circuits, the inductor and the capacitor are arranged – depending on the filtering effect wanted – so that a particularly high or particularly low resistance occurs at one particular frequency. In this way, frequencies above or below this frequency are deliberately attenuated or passed.

The inductor and the capacitor can be connected either in series or in parallel. Accordingly, a distinction is made between series tuned circuits (a) and parallel tuned circuits (b), as shown in Figure [ref:e_rp_schwingkreis]. 

---

If an inductor and a capacitor are connected in parallel and, for example, a square pulse is applied to this arrangement, it starts to oscillate. The charged capacitor now has energy stored in its electric field, which, however, discharges through the inductor. The current through the inductor builds up a magnetic field in it, which at first still opposes the flow of current. As soon as the magnetic field has built up, however, the capacitor discharges completely. The energy is now stored in the magnetic field of the inductor. But since the capacitor cannot discharge any further and cannot keep a current flowing, the magnetic field cannot be maintained. The magnetic field of the inductor collapses and produces a voltage in the opposite direction. This voltage now charges the capacitor in the opposite direction until the magnetic field in the inductor has collapsed and can no longer oppose the electric field in the capacitor. The process then starts again. 

<margin>
[include:applet_schwingkreis]
</margin>

---

This is why it is called a tuned circuit (in German *Schwingkreis*, literally "oscillating circuit"). The frequency at which this circuit oscillates is called the resonant frequency ($f_0$). It is comparable to the resonant frequency of a tuning fork that is set vibrating by a knock. At resonance, the resistances of the inductor, $X_\text{L}$, and of the capacitor, $X_\text{C}$, are equal. Such tuned circuits can be used, on the one hand, to generate oscillations, which we will look at more closely in the chapter on oscillators. On the other hand, they can also be used as filters – and that is exactly the subject of this chapter.

<margin>
[picture:1037:e_rsk_frequenzgang:Qualitative frequency response of a series tuned circuit]
</margin>

---

In a *series tuned circuit*, as in Figure [ref:e_rp_schwingkreis]a, the total resistance is lowest at resonance. Figure [ref:e_rsk_frequenzgang] shows the frequency response. At frequencies above the resonant frequency the resistance of the inductor becomes larger, so that the total resistance of the series tuned circuit also rises. The same happens at frequencies below the resonant frequency, but here it is the resistance of the capacitor that is high. In series tuned circuits the resistance is therefore lowest at the resonant frequency. Because of the series connection, at frequencies away from the resonant frequency the component with the higher resistance determines the impedance of the tuned circuit.

<indepth>
The magnitude response of a series tuned circuit made up of a resistor, an inductor and a capacitor is calculated with the following formula:
  
$Z = \sqrt{R^2+\left(X_\text{L} - X_\text{C}\right)^2}$
  
At resonance, when $X_\text{C}$ = $X_\text{L}$, only the resistance $R$ remains. In the ideal case, when the resistance $R=\qty{0}{\ohm}$, the resistance is even zero. If we insert the values for $X_\text{L}$ and $X_\text{C}$, we obtain:
  
$Z = \sqrt{R^2+\left(2\pi f \cdot L~-~\frac{1}{2\pi f \cdot C} \right)^2}$
  
The formula shows the frequency response from Figure [ref:e_rsk_frequenzgang] very nicely: if the frequency is allowed to approach $\qty{0}{\hertz}$, the inductor's contribution drops out and only the capacitor has an effect. If, on the other hand, the frequency is allowed to approach infinity, only the inductor has an effect and the capacitor's contribution disappears.
  
The resonant frequency can even be calculated. When $X_\text{L} = X_\text{C}$, the formula can be solved for $f$:
  
$2\pi f \cdot L = \frac{1}{2\pi f \cdot C}$
  
This gives the formula: 
  
$f_0 = \frac{1}{2\pi \sqrt{L\cdot C}}$
  
The full derivation of the formulas can be found, for example, on [Wikipedia](https://50ohm.de/schwk). It should be mentioned at this point that all the frequency responses are drawn qualitatively and may look somewhat different in reality.
</indepth>

[question:ED205]

---

If, on the other hand, the capacitor and the inductor are combined into a *parallel tuned circuit*, as in Figure [ref:e_rp_schwingkreis]b, the behaviour is exactly the other way round: the resistance *$Z$* is very high at the resonant frequency, see Figure [ref:e_psk_frequenzgang]. At frequencies above the resonant frequency, however, the capacitor has a low resistance, so that the resistance of this tuned circuit falls. At frequencies below the resonant frequency, on the other hand, the inductor has a low resistance, so that the resistance of the tuned circuit also falls at lower frequencies. 
In parallel tuned circuits the resistance is therefore highest at the resonant frequency. At frequencies away from the resonant frequency, the component with the lower resistance determines the impedance of the parallel tuned circuit. 

<margin>
[picture:1036:e_psk_frequenzgang:Qualitative frequency response of a parallel tuned circuit]
</margin>

[question:ED206] 
[question:ED207]

% TODO ////

Depending on how parallel and series tuned circuits are placed in the signal path, frequency ranges can now either be attenuated or filtered out. For this we will again use our potential divider approach.

---

Let us begin with the circuits for *band-stop filters*. There are two ways of building them as a potential divider: first the *acceptor circuit* (see Figure [ref:e_saugkreis]) and second the *rejector circuit* (see Figure [ref:e_sperrkreis]). Each figure shows the frequency-dependent resistance and the output voltage. With our familiar rules for the potential divider, these relationships can be derived and understood just as for the RC networks covered earlier. Because parallel tuned circuits have a high resistance at resonance, they are well suited for use as a rejector circuit in series in the signal path. Alternatively, the low resonant resistance of a series tuned circuit is used as an acceptor circuit in parallel with the signal path. Often, though, both are used in combination here too. One application of band-stop filters is, for example, suppressing individual parts of a band, for instance when a nearby VHF FM broadcast transmitter interferes with reception.

[question:ED204]
[question:ED214] 
[question:ED215]

<margin>
[picture:1038:e_saugkreis:Qualitative frequency responses of an acceptor circuit]
[picture:1040:e_sperrkreis:Qualitative frequency responses of a rejector circuit]
</margin>

---

The second category of circuits that can be developed from tuned circuits is *band-pass filters*. Here again there are two ways of building them as a potential divider: first the *series pass circuit* (in German *Leitkreis*, see Figure [ref:e_leitkreis]) and second the *band-pass filter* (see Figure [ref:e_bandpass]). Here too, the derivation follows, as usual, from the behaviour of a potential divider. For a band-pass filter, parallel tuned circuits are placed in parallel with the signal path, because they have a low resistance at frequencies away from resonance and so, as it were, "short-circuit" them. A series tuned circuit in series in the signal path provides additional attenuation away from resonance, while it has a low resistance at the wanted frequency.

[question:ED203]

<margin>
[picture:1039:e_leitkreis:Qualitative frequency responses of a series pass circuit]
[picture:1041:e_bandpass:Qualitative frequency responses of a band-pass filter]
</margin>

An obvious application of band-pass filters is in receivers where certain frequency bands have to be pre-filtered. In this case a filter is used that passes only a wanted frequency band, while all other frequencies are attenuated. Such band-pass filters are therefore found in almost every receiver, often even separately for each individual HF band. Designed for correspondingly high power, band-pass filters are also used when transmitting, for example at joint contests or Field Days, to minimise mutual interference between neighbouring stations.

So both series and parallel tuned circuits can be used to build band-pass and band-stop filters. What matters is to bear in mind how each tuned circuit behaves at resonance. According to their behaviour, they can be placed in series in the signal path or in parallel across it – possibly even several of them combined with one another. 

Only certain suitable types of capacitor can be used in filters.
Electrolytic capacitors, for example, are not suitable for RF circuits, on the one hand because their capacitance depends strongly on frequency, and on the other because they have a high internal resistance at high frequencies. Film capacitors, on the other hand, are not suitable because their windings (self-inductance) make them strongly frequency-dependent, especially from the HF range upwards, and they have a poor Q. 
Ceramic capacitors, by contrast, have only small losses, and their capacitance depends only a little on frequency and temperature. They are also easy to obtain for high voltages.
Capacitors made of plates with air as the insulator are also suitable; they are most often found as variable capacitors. Variable capacitors are also used for high voltages in antenna tuners.

[question:ED216]