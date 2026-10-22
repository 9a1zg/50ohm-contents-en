The frequency of a VFO depends directly on its operating voltage (DC voltage). This is caused mainly by the way the operating point of the transistor in its oscillator depends on that voltage.
To make the frequency of a VFO as stable as possible against fluctuations in the operating voltage, this voltage must be *stabilised* as well as possible by suitable circuit design measures. The operating voltage of a VFO should therefore be independent of the operating voltages of other stages (stabilised) and be *filtered and decoupled* as well as possible. This can be achieved, for example, with a fixed voltage regulator (see Figure [ref:a_osc_stab]).

[question:AD612]
[question:AD608]
[question:AD607]

<margin>
[picture:200:a_osc_stab:Fixed voltage regulator]
</margin>

---

If the operating voltage is poorly stabilised, very simple CW transmitters can suffer from a pitch defect known as *chirp*: at the start of each individual dit or dah, the pitch is at first slightly higher or slightly lower and then approaches the actual pitch. The English word "chirp" means the short, high call of a small bird. When the pitch approaches from above, the sound really does have something of a bird's chirp about it.

[question:AD609]

<margin>
Here is an example of such a chirp signal:

[include:applet_chirp_1]

Another example, a QSO between RA1OW and OM3YCY, in which the chirp can be heard clearly in the second over:

[include:applet_chirp_2]

</margin>