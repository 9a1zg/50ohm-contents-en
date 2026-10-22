We have already met the *MUF* (*maximum usable frequency*), the highest frequency that the ionosphere can still bend back for the distance between transmitter and receiver, in Class E. There it became clear that the MUF depends on the density of the free electrons in the refracting region. In Class A we will now look at this topic more closely, particularly with regard to the angle of radiation.

[question:AH206]
[question:AH207]

As we also know already, the range of sky waves depends on the angle of radiation. The lower the angle at which the wave strikes the ionosphere, the more easily it is refracted. This relationship also applies to the MUF: the frequency that is just still bent back, the *MUF*, is higher the lower the angle at which our signal enters the ionosphere. Figure [ref:e_muf_winkel2] shows a simulation of the skip distance for a summer day in 2024 for an amateur radio signal around $\qty{7}{\mega\hertz}$. At $\qty{45}{\degree}$ the MUF on that day was $\qty{7.5}{\mega\hertz}$. If you change the angle of radiation, the MUF changes too: if you radiate more steeply (e.g. $\qty{60}{\degree}$), the MUF falls and the radio wave is no longer refracted. If, on the other hand, you radiate at a lower angle (e.g. $\qty{30}{\degree}$), the MUF rises. In what follows we will look at this relationship more closely.

<margin>
[picture:998:e_muf_winkel2:Skip distance at 7 MHz in summer 2024]
</margin>

---

Ionospheric measuring stations measure what is known as the critical frequency $f_\text{c}$ (often also $f_\text{k}$, $f_\text{krit}$ or $f_\text{oF2}$). This is the highest frequency at which the sky wave entering the ionosphere vertically is still just reflected (see Figure [ref:e_muf_winkel]). If we radiate vertically upwards, so that our signal enters the ionosphere at an angle of $\qty{90}{\degree}$, the MUF is at its lowest, because our signal then has to "turn round" completely in the ionosphere, that is, make a 180° turn. This means that at $\qty{90}{\degree}$, $f_\text{c} = MUF$. 

<indepth>
The symbol used is $f_o$ (small subscript letter "o" for *ordinary wave*) followed by the ionospheric region to which this frequency applies, e.g. $f_\text{oF2}$ for the F2 region. However, $f_\text{c}$, $f_\text{k}$ or $f_\text{krit}$ are also often used as the symbol.
</indepth>

<margin>
[picture:870:e_muf_winkel:The angles for calculating the MUF]
</margin>

<indepth>
The critical frequency is therefore the highest frequency that comes back from the ionosphere when you radiate vertically upwards. A rule of thumb says that the highest frequency still returned at a *low* angle of radiation is about three times the critical frequency.
</indepth>

[question:AH204]
[question:AH205]

---

Figure [ref:e_muf_fof2] shows the variation of the MUF and $f_\text{c}$ over time on 08.09.2025, measured with the ionosonde at Juliusruh. MUF $\qty{3000}{\kilo\meter}$ here means radiating at a very low angle in order to achieve a skip distance of $\qty{3000}{\kilo\meter}$.

<margin>
[picture:999:e_muf_fof2:MUF and $f_\text{c}$ on 08.09.2025]
</margin>

For other angles of radiation, the MUF can be determined approximately from $f_\text{c}$ using the following formula from the formula sheet (valid for $\alpha > \qty{40}{\degree}$):

$MUF \approx \frac{f_\text{c}}{sin(\alpha)}$

where $\alpha$ is the angle of radiation (see Figure [ref:e_muf_winkel]). A closer look at the formula shows that the MUF is always higher than the critical frequency – and the more so, the lower the angle at which the transmitting antenna radiates or the receiving antenna receives.

[question:AH208]

---

For commercial frequency planning, where what matters is that a contact succeeds with high probability, there is also the term *FOT* (*frequency of optimum transmission*, optimum working frequency), or $f_\text{opt}$. This is the frequency that statistically allows a contact on a given signal path on 90% of all days; it is usually 15% below the monthly mean of the MUF. In the formula sheet we find this relationship as 

$f_\text{OPT} = MUF \cdot 0.85$

With this information we can now solve the following problem; a calculator will help.

[question:AH209]

<indepth>
For DX contacts in amateur radio, $f_\text{opt}$ plays no part, because there you usually choose the highest band that still allows a contact (that is, the one closest to the MUF), since that is where the lowest noise floor and so the best signal can be expected (highest signal-to-noise ratio, SNR).
</indepth>

In Class E we have already met the LUF (*lowest usable frequency*). It is determined by the D region and denotes the lowest usable frequency, below which the attenuation is too great. The D region *attenuates* our radio signal, after all, and on each hop the signal has to pass through this D region *twice*. At the same time, this attenuation is greater the lower the frequency (the relationship is quadratic: halving the frequency quadruples the attenuation). So if you keep reducing the frequency, you will likewise reach a point at some stage where the signal bent back is no longer usable; that is the LUF.

[question:AH210]
[question:AH211]
