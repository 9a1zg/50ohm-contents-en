Instead of a bridge rectifier, full-wave rectification can also be achieved with two diodes and a transformer with a centre tap.

<latexonly>
Figure [ref:a_vollweggleichrichter] shows such a so-called full-wave rectifier. 

<margin>
[picture:946:a_vollweggleichrichter:Full-wave rectification with two diodes]
</margin>
</latexonly>

<webonly>
The applet alongside [ref:a_vollweggleichrichter] shows such a so-called full-wave rectifier. 

<margin>
[include:applet_gleichrichter_1]
</margin>
</webonly>

---

To understand how it works, the positive and the negative half cycle have to be considered separately. If a positive half cycle with respect to the centre tap is present on the upper winding at the anode of diode $D_1$, then only this diode conducts and passes the half cycle on to the output marked +. At this moment a negative half cycle with respect to the centre tap is present at the anode of diode $D_2$. This diode stays blocked during this half cycle.

During the next half cycle, diode $D_1$ is blocked and diode $D_2$ conducts, since a positive half cycle with respect to the transformer's centre tap is now present there. Two half cycles now appear at the DC output, but always in the positive direction with respect to the centre tap. The centre tap forms the negative terminal of the DC output voltage.

<tip>
The same mnemonic as for the bridge rectifier: the two cathodes of the diodes are connected together to the positive terminal of the output voltage.
</tip>

[question:AD307]

If two anodes are connected together to one output terminal, the pulsating DC voltage there will be negative with respect to the transformer's centre tap. Both half cycles lie below the zero line.

[question:AD308]
