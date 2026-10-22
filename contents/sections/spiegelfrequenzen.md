By the very nature of the concept, the mixing process that takes place in a superhet (see Figure [ref:spiegelfrequenzen_mischen1]) with the receiver's oscillator frequency always gives two possible receive frequencies:

$f_\text{ZF} = \left|f_\text{e} \pm f_\text{o}\right|$

Since in the superhet we want to mix down to a lower intermediate frequency, the difference frequency is of particular interest here:

$f_\text{ZF} = \left|f_\text{e} - f_\text{o}\right|$

The magnitude is what matters here: for a fixed oscillator frequency $f_\text{o}$ and intermediate frequency $f_\text{ZF}$ there are two possible receive frequencies, both of which produce the same intermediate frequency. One of them is the wanted receive frequency; the other is called the *image frequency*.

<margin>
[picture:807:spiegelfrequenzen_mischen1:Mixing with receive frequency $f_\text{e}$, oscillator frequency $f_\text{o}$ and the intermediate frequency $f_\text{ZF}$]
</margin>

---

<margin>
[picture:806:spiegelfrequenzen_fe1_fe2:Receive frequencies that both lead to the same $f_\text{ZF}$]
</margin>

Example: let us assume that our oscillator oscillates, as shown in Figure [ref:spiegelfrequenzen_fe1_fe2], at the frequency $f_\text{o}=\qty{3.955}{\mega\hertz}$. The intermediate frequency $f_\text{ZF}$ is to be $\qty{0.455}{\mega\hertz}$. Because of the magnitude in our formula, there are now two possible receive frequencies that can be heard, namely $f_\text{e1} = \qty{3.500}{\mega\hertz}$ and $f_\text{e2} = \qty{4.410}{\mega\hertz}$. For both values the formula gives the intermediate frequency $f_\text{ZF}$.

If $f_\text{e1}$ is the wanted receive frequency, $f_\text{e2}$ is called the image frequency of $f_\text{e1}$. If $f_\text{e2}$ is the wanted receive frequency, $f_\text{e1}$ is called the image frequency of $f_\text{e2}$.

The spacing between the wanted receive frequency and the image frequency is always twice the intermediate frequency (IF), as can easily be seen in Figure [ref:spiegelfrequenzen_fe1_fe2]. 

If the oscillator oscillates *above* the receive frequency ($f_\mathrm{E} < f_\mathrm{OSZ}$), the image frequency is also *above* the receive frequency, by twice the IF ($f_\mathrm{S} = f_\mathrm{E} + 2\cdot f_\mathrm{ZF}$).

If, on the other hand, the oscillator is *below* the receive frequency ($f_\mathrm{E} > f_\mathrm{OSZ}$), the image frequency is also *below* the receive frequency, by twice the IF ($f_\mathrm{S} = f_\mathrm{E} - 2\cdot f_\mathrm{ZF}$). This relationship can also be found in the formula sheet. 

Now try to answer the following questions with this knowledge.

[question:AF106]
[question:AF201]
[question:AF202]
[question:AF203]
[question:AF107]
[question:AF108]

---
<margin>
[picture:808:spiegelfrequenzen_mischen2:Additional band-pass filter for image rejection]
</margin>

If it is not sufficiently suppressed, the image frequency can cause interference to reception, since signals on the image frequency are also converted to the same intermediate frequency and can therefore become audible in the receiver. To avoid this, the wanted receive frequency is selected with a band-pass filter before the mixer, as shown in Figure [ref:spiegelfrequenzen_mischen2]. The image frequency is to be suppressed as strongly as possible.

For effective image rejection, the largest possible spacing between the wanted receive frequency and the image frequency is an advantage. This spacing becomes larger if a higher intermediate frequency is chosen.

This can also be seen from Figure [ref:spiegelfrequenzen_fe1_fe2]: as the IF increases, the two possible receive frequencies $f_\text{e1}$ and $f_\text{e2}$ lie further apart.

The larger this frequency spacing, the more easily the band-pass filter ahead of the mixer can let the wanted receive frequency pass and at the same time strongly attenuate the image frequency. With a very small spacing, on the other hand, the filter would need much steeper skirts or a higher selectivity. The demands on the receiver's preselection would then be considerably higher.

[question:AF109]
[question:AF110]
[question:AF111]
[question:AF204]