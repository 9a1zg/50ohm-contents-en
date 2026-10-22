A power supply unit converts the $\qty{230}{\volt}$ AC voltage from the mains socket into a lower DC voltage. In amateur radio we often use power supply units that provide a DC voltage of $\qty{13.8}{\volt}$ at their output, for example to run a transceiver.

<margin>
[picture:740:n_netzgeraet:Power supply unit]
</margin>

<indepth>
To *monitor the operating state* of a power supply unit there are illuminated switches, indicator LEDs or illuminated meters. The meters can show the operating voltage in volts and the current flowing at the moment in amperes separately. There are also switchable digital displays for this purpose.
</indepth>

[question:ND101]
[question:ND102]

---

A power supply unit is often connected to the mains socket with a *Schuko plug* (earthed plug). With the Schuko plug it does not matter which way round it is plugged in, since with AC the polarity changes all the time. The plug and the socket each have 3 poles, as can be seen in Figure [ref:n_schutzkontakt]. The pins of the plug fit into the openings of the socket and make the connection to the so-called L and N conductors, between which the dangerous AC voltage of $\qty{230}{\volt}$ is present.

<margin>
[photo:86:n_schutzkontakt:Earthing contact on a mains socket, and a Schuko plug]
</margin>

The outer sliding contact of the Schuko plug is called the *earthing contact* (marked in red in Figure [ref:n_schutzkontakt]). When the plug is inserted, the earthing contact connects to the so-called *PE conductor* of the socket. "PE" stands for "protective earth". So when the plug is inserted, the metal case of the power supply unit is earthed. This rules out a dangerous voltage on the case.

[question:ND109]

---

The output of the power supply unit and the lead to the transceiver have two conductors, so that a closed circuit can be formed. This is the prerequisite for the current to flow from the power supply unit to the transceiver, through it and back to the power supply unit. 

<webmargin>
[picture:680:n_Netzgeraet_TRX:Connecting the power supply unit and the transceiver]
</webmargin>

The output terminals for the DC voltage are coloured: red stands for positive and black for negative. When connecting the lead to the transceiver, this polarity must always be observed. Otherwise there may be a short circuit or, in the extreme case, even the destruction of the transceiver. The power supply unit should only be switched on once all the leads are connected and the polarity has been checked. 

[question:ND104]
[question:ND103]
[question:ND105]
[question:ND106]
[question:ND107]

---

In the power supply unit and in the lead to the transceiver there are so-called miniature fuses. They can detect a fault (short circuit or overload) and interrupt the flow of current. These are often wire fuses, in which a thin wire melts when too much current flows. The circuit is then no longer closed and no more current can flow. This is called a *blown fuse* or, in technical language, a *thermal shutdown*.

<margin>
[photo:88:n_feinsicherungen:Miniature fuses]
</margin>

<indepth>
*In depth:* Miniature fuses measure $\qty{5}{\milli\meter} \times \qty{20}{\milli\meter}$ and are available in different versions. They differ in their current ratings and tripping characteristics. Time-lag fuses are always used when the inrush current is considerably higher than the rated current, e.g. in power supply units. The tripping time of the fuse depends on the current and on how long it flows. Table [ref:n_feinsicherung] lists typical values of the tripping time. Manufacturers give more precise information in characteristic curves in their data sheets.
</indepth>

Once a fuse has blown and the cause has been found and put right, the fuse has to be replaced. Faulty fuses may only be replaced by fuses of the same type, though! Both the current rating and the so-called tripping characteristic have to be taken into account; it states how quickly a fuse blows (fast-acting, medium time-lag, time-lag).

<webmargin>
| l: Tripping characteristic | l: Marking | X: Breaking time |
| fast-acting | F | max. $\qty{30}{\milli\second}$ |
| medium time-lag | MT | max. $\qty{90}{\milli\second}$ |
| time-lag | T | max. $\qty{300}{\milli\second}$ |
[table:n_feinsicherung:Characteristics of miniature fuses, breaking time at ten times the rated current]
</webmargin>

<danger>
*WARNING:* Bridging a faulty fuse, e.g. with aluminium foil, as is sometimes done, is not permitted and is very dangerous. There is a risk of fire!
</danger>

High-quality power supply units often also have electronic current limiting. In the event of a short circuit it makes sure that the current is limited. This is called *short-circuit current limiting*. Once the fault has been put right, no fuse has to be replaced.

[question:ND108]
[question:NK305]
