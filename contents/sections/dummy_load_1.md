If you want to check the transmit power of a transmitter, you connect what is called a *dummy load* in place of the antenna (Figure [ref:n_antennenanpassung_dummy_load]). A dummy load is also called a *termination* or an artificial antenna. It consists of a load resistor (see the chapter on components and circuits) and a heatsink.

<margin>
[photo:68:n_antennenanpassung_dummy_load:Dummy load]
</margin>

A dummy load is used for alignment work and measurements on transmitters. Unlike a real antenna, it converts almost all of the transmit power into heat. This prevents signals from being radiated. Unnecessary emissions and possible interference to other contacts are thus avoided.

It is important that, whenever you transmit, either an antenna that is as well matched as possible or a dummy load is connected to the transceiver. Otherwise the entire transmit power is reflected at the antenna socket and can, for example, damage the RF amplifier (output stage).

<indepth>
From the transmitter's point of view, a dummy load cannot be distinguished from a well-matched antenna, since the transmit power is not reflected.
</indepth>

[question:VD111]
[question:NJ202]
[question:NF107]

---

Transmissions for tuning cannot be avoided altogether, for example when automatic antenna tuning units are used. If transmissions of this kind are kept as short as possible, however, they are permitted, even if only a carrier without modulation is transmitted.

<attention>
When you tune your antenna tuning unit, you should only do so on frequencies that are not in use. Otherwise you may interfere with other contacts.
</attention>

[question:VD112]
