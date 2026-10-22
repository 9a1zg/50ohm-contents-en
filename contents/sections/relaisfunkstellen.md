A repeater provides a greater range than is often possible with a direct contact between two amateur stations. Repeaters are usually set up at exposed locations, e.g. on mountain tops, high-rise buildings, church towers and other towers. There are also repeaters in satellites orbiting the earth. Figure [ref:n_relaisfunkstellen_aufbau] shows how such a station is set up and how it works. 

[picture:648:n_relaisfunkstellen_aufbau:Schematic diagram of a repeater with users]

If, for example, there is a mountain between two radio stations, it is impossible to transmit through the mountain. A repeater on the mountain top still makes it possible to establish a contact, since both stations can reach the repeater directly.

In German, repeaters (*Relaisfunkstellen*) are also called *Relais* or *Repeater* for short. They can be recognised by the fact that they transmit their call sign regularly. According to the [Call Sign Plan](https://50ohm.de/rzp), a repeater's call sign usually begins with DB0, DM0 or DO0.

The official definition of repeaters reads somewhat more drily: *"Repeater": a remotely controlled amateur station (also in satellites) that transmits, when triggered remotely, received amateur radio transmissions, parts of them or other signals fed in or stored, and thereby serves to make amateur stations easier to reach*

The following question on this definition can, however, also be solved well by elimination if you know the following:
* Repeaters are not operated with personal call signs.
* Repeaters are usually not permanently attended.
* Repeaters do not necessarily have to be operated at geographically exposed locations.

[question:VD118]

---

A repeater receives the signal of an amateur station on its input frequency and transmits it simultaneously on its output frequency. So that the repeater's transmitter does not interfere with its own receiver, the transmit and receive frequencies are usually different. The spacing between the transmit and receive frequencies is called the repeater shift, or simply the shift. The shifts usually used in Germany are given in Table [ref:n_relaisfunkstellen_ablage].

<margin>
| r: Band | X: Shift |
| $\qty{10}{\meter}$ | $\qty{100}{\kilo\hertz}$ |
| $\qty{2}{\meter}$ | $\qty{600}{\kilo\hertz}$ |
| $\qty{70}{\centi\meter}$ | $\qty{7.6}{\mega\hertz}$ |
| $\qty{23}{\centi\meter}$ | $\qty{28}{\mega\hertz}$ |
[table:n_relaisfunkstellen_ablage:Repeater shift]
</margin>

For example, the frequency of a $\qty{70}{\centi\meter}$ repeater is given like this:
* Input frequency: $\qty{431.275}{\mega\hertz}$
* Shift: $\qty{+7.600}{\mega\hertz}$
* Output frequency: $\qty{438.875}{\mega\hertz}$

[question:BE401]
[question:BE402]
[question:BE403]

<indepth>
Some repeaters also work in what is called *crossband operation*. This means that one station transmits and receives on one band (e.g. $\qty{70}{\centi\meter}$), and another station on the same repeater, but on a different band (e.g. $\qty{2}{\meter}$). The repeater controller passes the conversations between the two bands. The mode can also be converted, for example from SSB to FM.
</indepth>

A repeater station that passes on data rather than voice is called a digipeater. A digipeater is able to receive data packets and transmit them again. Its special feature is that the transmission can take place only in parts or with a time delay. Data packets can also be repeated, or individual data fields changed.

[question:NF118]

---

Before you can start operating through a repeater, you must know its technical features and parameters. For certain repeaters, further settings on your transceiver besides the frequency are needed to ensure interference-free operation. Besides analogue FM (frequency modulation), digital modes such as DMR and D-Star are also used for voice transmission.

<tip>
Information on repeaters and their technical parameters and features is available from the nearest DARC local club, from the person responsible for the repeater, or from the internet.
</tip>

[question:NE309]
[question:NE308]

An important setting is the channel bandwidth in FM operation. Remember: the bandwidth states how much "space" a transmission occupies in the frequency spectrum. On the one hand there is wide FM, with a bandwidth of $\qty{25}{\kilo\hertz}$, shown on the display as *FM-W*, for example. On the other hand there is narrowband FM, which occupies a bandwidth of only $\qty{12.5}{\kilo\hertz}$ and is shown on the radio as *FM-N*, for example. Many repeaters really do not like signals that are too wide, because they can cause distorted signals and interference to adjacent repeater frequencies.

[question:BE407]

Operation through remotely controlled amateur stations must in principle be permitted to all radio amateurs with an assigned call sign. To ensure interference-free operation, however, the operator can exclude other radio amateurs from using the amateur station. The Federal Network Agency (Bundesnetzagentur, BNetzA) must be informed of this.

[question:VD504]

When operating through repeaters, overs should be kept as short as possible so that mobile and portable stations can use the repeater more easily, especially if they are within its coverage area only briefly. You should leave a pause between overs to give other stations an opportunity to join in.

[question:BE406]
[question:BE404]

If two different stations speak into the repeater at the same time, the repeater's transmission is disturbed to the point of being unreadable. To avoid this so-called doubling, there should always be a proper handover between the repeater users. This also means only starting to transmit once the previous station has finished its transmission.

[question:NE310]
[question:BE405]

Annex 1 to the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV), which we have already discussed, also contains requirements for the transmit power of repeaters. Above 30 MHz, an automatically operating station may be operated with a maximum of 50 W ERP.

[question:VD503]

There is one special point in assessing a contact through a repeater. Since the signal strength with which you receive the other station is the signal strength of the repeater and not that of the other station, it is not given. Only the readability (R) is assessed in the report.

[question:BE408]