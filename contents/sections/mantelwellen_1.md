When connecting antennas, we want only the antenna to radiate or pick up signals, not the feeder itself, which may be run inside the house. Screened lines such as coaxial cable are suitable for this, because ideally they neither radiate nor pick up electromagnetic waves themselves, but carry the signal through the cable screened from the outside world (e.g. the house wiring).

<indepth>
For the screening of a coaxial cable to do its job, one *condition* must be met: the current in the inner conductor must be exactly opposite to the current in the outer conductor, and both currents must have the same magnitude. In this case a field exists only between the two conductors, and the surroundings of the cable are not affected. Precisely then, the outer conductor has no RF voltage to earth.

Conversely, however, this also means: if the outer conductor has an RF voltage to earth, then the currents in the inner conductor are not balanced and the coaxial cable radiates.

The currents in the coaxial cable should therefore be balanced (same magnitude but opposite sign, i.e. opposite direction), and the voltages to earth should be *unbalanced* (only the inner conductor carries a voltage to earth).
</indepth>

---

If, however, a balanced antenna such as a half-wave dipole is connected to a coaxial cable, the coax can still radiate despite its screening! This is because RF currents can flow on the surface of the outside of the metal outer conductor, accompanied by an electromagnetic field around the outer insulation (see Figure [ref:e_mantelwellen]). We call this effect *common-mode currents* (in German *Mantelwellen*, literally "sheath waves"). When transmitting, they can cause interference to other equipment in the house, and they can also cause reception problems, since the coaxial cable becomes, as it were, part of the antenna, so that interference from within the house is more easily picked up by the radio. The additional sheath currents are then "missing" from one of the two dipole legs, which also distorts the radiation pattern.

[question:EG405]
[question:EG406]

Figure [ref:e_mantelwellen] shows how part of the current that should actually flow into the dipole leg flows back on the coax screen.

<margin>
[picture:633:e_mantelwellen:Common-mode currents]
</margin>

Sheath currents do in fact flow largely on the surface of the outer conductor. This is due to what is called the *skin effect*, which causes RF currents to flow largely on the surface of metal conductors. In this sense a coaxial cable can also be thought of as a three-conductor system:
  
1. Outside of the inner conductor
2. Inside of the outer conductor
3. Outside of the outer conductor
  
The current on the outside of the inner conductor and the current on the inside of the outer conductor always have the same magnitude and flow in opposite directions ($I_1$). The current on the outside of the outer conductor ($I_3$) is the sheath current.

[question:EG404]

---

Common-mode currents can be prevented, for example, by using a *balancing device*, a balun, to connect the coaxial cable to the antenna.

<indepth>
The word *balun* is made up of the words "balanced" and "unbalanced", because a balanced side (e.g. a balanced antenna) is to be connected to an unbalanced side (the coaxial cable, in which ideally only the inner conductor has a voltage to earth).
</indepth>

[question:EG407]

---

Another form of balun is made by winding a coaxial cable on a ferrite core. This is what is called a *current-compensated choke*, and it is also known as a *common-mode choke*. To differential-mode signals it presents a low impedance because, when the current in the inner conductor is the reverse of that in the outer conductor, there is no appreciable interaction with the ferrite material. To common-mode currents, however, the arrangement acts like a (lossy) inductor.

<margin>
[photo:325:e_mantelwellendrossel:Common-mode choke]
</margin>

[question:EG408]