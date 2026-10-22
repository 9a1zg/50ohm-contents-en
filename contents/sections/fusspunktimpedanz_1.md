For a resonant, centre-fed half-wave dipole in free space, the feed-point impedance is, in the ideal case, about $\qty{73.1}{\ohm}$ and so approximately $\qty{75}{\ohm}$. Although this value is already of the same order as the desired $\qty{50}{\ohm}$, it does not match it exactly. If such a dipole is fed directly with a $\qty{50}{\ohm}$ feeder, there is therefore a slight mismatch. For the best possible power transfer, or the lowest possible SWR, matching can therefore make sense even for a dipole. In principle this also applies at heights of about one wavelength or more, although the actual feed-point impedance can differ slightly depending on the wire thickness, the surroundings and the height, as we shall see in a moment.

<margin>
[picture:788:e_fusspunktimpedanz_dipol:Feed-point impedance of a dipole as a function of height (simulated with NECPP)]
</margin>

[question:EG207]

When there is interaction with the ground because the antenna is installed lower, the feed-point impedance of a centre-fed dipole lies in the range from $\qty{40}{\ohm}$ to $\qty{90}{\ohm}$, as shown in Figure [ref:e_fusspunktimpedanz_dipol]. 

[question:EG208]
[question:EG209]

If a dipole is built as a folded dipole, the sections of the antenna are connected in series but partly run in parallel, so the applied voltage doubles and the current needed halves. This corresponds to a fourfold increase in the feed-point impedance. A folded dipole therefore has a feed-point impedance of $\qtyrange{240}{300}{\ohm}$.

[question:EG210]

---

In a ground-plane antenna, on the other hand, one leg of the dipole is omitted and replaced by an earth with the lowest possible resistance. Here, then, the feed-point impedance comes to $\frac{\qty{73.1}{\ohm}}{2} \approx \qty{37}{\ohm}$, which is half the feed-point impedance of a dipole in free space. In ground-plane antennas whose radials slope downwards at $\qty{45}{\degree}$, the additional radiation from the radials gives a feed-point impedance of exactly $\qty{50}{\ohm}$, so that no further matching to common coaxial cables is needed. The feed-point impedance of a ground plane therefore lies between $\qtyrange{30}{50}{\ohm}$.

<indepth>
With a poor earth or interaction with the ground, a ground-plane antenna can have a feed-point impedance of more than $\qty{37}{\ohm}$ even with horizontal radials (e.g. laid on the earth's surface). The additional resistance then comes from ground losses.
</indepth>

[question:EG211]
