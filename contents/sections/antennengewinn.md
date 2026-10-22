%TODO ggf. das Kapitel wo anders hinschieben 

The chapter on decibels already touched on the suffixes $\unit{\dBd}$ and $\unit{\dBi}$, which are used when antenna gains are stated. In this case the decibel value does not refer to a power or a voltage, but to a particular reference radiator. The usual ones are $\unit{\dBi}$, relative to the isotropic radiator, and $\unit{\dBd}$, relative to the half-wave dipole.

The *isotropic radiator* (see Figure [ref:e_Kugelstrahler]) is an imaginary, hypothetical antenna that radiates equally strongly in all directions. If a real antenna has directional properties, its radiation is stronger in certain directions and weaker in other directions than it would be with the hypothetical isotropic radiator. 

<margin>
[picture:751:e_Kugelstrahler:Isotropic radiator at the centre of a sphere, producing the same radiated power at every point on the surface of the sphere]
</margin>

The gain in one direction (e.g. the direction of maximum radiation, which is the direction with the greatest antenna gain) relative to an isotropic radiator can be given in decibels, $\unit{\dB}$. Instead of $\unit{\dB}$, $\unit{\dBi}$ is written to make clear that the reference is the isotropic radiator.

[question:EG220]

Even a simple half-wave dipole has a gain, because at right angles to the conductor it radiates $\qty{2.15}{\dB}$ more strongly than an isotropic radiator would. Accordingly, a half-wave dipole has a gain of $\qty{2.15}{\dBi}$.

Sometimes what matters is the gain over and above that of a half-wave dipole, that is, the gain relative to a half-wave dipole. This is given in $\unit{\dBd}$, where the $\text{d}$ stands for dipole. Accordingly, a half-wave dipole has a gain of $\qty{0}{\dBd}$. Antennas with more gain than a half-wave dipole have a gain greater than $\qty{0}{\dBd}$, and antennas with less gain than a half-wave dipole, accordingly, less than $\qty{0}{\dBd}$.

Let us compare once more the gain of a half-wave dipole given in $\unit{\dBi}$ and given in $\unit{\dBd}$: the half-wave dipole has a gain of $\qty{2.15}{\dBi}$ in the direction of maximum radiation, since it radiates $\qty{2.15}{\dB}$ more strongly than the isotropic radiator. Given in $\unit{\dBd}$, however, it is $\qty{0}{\dBd}$. The figure in $\unit{\dBi}$ is always $\qty{2.15}{\dB}$ higher than the figure in $\unit{\dBd}$.

This is also in the formula sheet: 

$g_i = g_d + \qty{2.15}{\dB}$

[question:EG221]