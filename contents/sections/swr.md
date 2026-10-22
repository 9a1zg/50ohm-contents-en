As we learnt earlier, amateur radio equipment and the transmission lines common in amateur radio mostly use a characteristic impedance of $\qty{50}{\ohm}$. We also learnt that unwanted reflections occur at junctions between transmission lines if the characteristic impedances do not match.

Antennas, too, have a property similar to characteristic impedance, which depends on the exact arrangement of the antenna elements. This property is called the feed-point impedance. As with connecting two transmission lines of different characteristic impedance, the same applies here: if the feed-point impedance of the antenna does not match the characteristic impedance of the feeder, unwanted reflections occur. Part of the transmit power is reflected back to the radio and cannot be radiated by the antenna.

If, on the other hand, the feed-point impedance of the antenna and the characteristic impedance of the feeder are the same, so that the transmit power is transferred into the antenna in the best possible way, the antenna is said to be *matched*.

<margin>
[photo:144:swr_meter:A simple SWR meter for determining the standing wave ratio]
</margin>

How well the antenna is matched can be measured. Put simply, this is done by determining how much of the transmit power is reflected by the antenna. The value shown by the meter is called the *standing wave ratio*, usually abbreviated to SWR. To determine the SWR, an *SWR meter* is used.

% TODO: Editionsspezifisch machen
<indepth>
An SWR meter measures at the same time the forward power that the transmitter sends to the antenna and the reflected power that has come back. This can be seen clearly on the SWR meter in Figure [ref:swr_meter_kreuzzeiger], which shows forward and reflected power separately. The SWR, however, is not simply the ratio of these two readings; it is worked out in a slightly more complicated way as $\text{SWR} = \frac {\sqrt{P_\text{V}}+\sqrt{P_\text{R}}} { \sqrt{P_\text{V}}-\sqrt{P_\text{R}}}$, where $P_\text{V}$ is the forward and $P_\text{R}$ the reflected power. You do not need to know this formula for the Class N examination.
</indepth>

<margin>
[photo:143:swr_meter_kreuzzeiger:SWR meter with cross-needle display, left needle for the forward and right needle for the reflected power; to read the SWR, follow the green line downwards from the point where the two needles cross]
</margin>

[question:NI201]

---

<margin>
[photo:67:n_swr_display:Display of a transceiver]
</margin>

Modern transceivers already have a built-in SWR meter. Its reading is usually found on the display, see [ref:n_swr_display].

<attention>
SWR meter and S meter sound similar but are different: the SWR meter measures the standing wave ratio when transmitting, and the S meter measures the signal strength when receiving.
</attention>

% TODO Big Picture: Im Bild Trx_Display "SWR" kennzeichnen
[question:NF101] 

---

If no SWR meter is built into the transceiver, an external SWR meter can be used. It is connected between the radio and the antenna, as in Figure [ref:n_trx_kabel_swr_antenne]. This is also described as "inserting the SWR meter in the line between transceiver and antenna".

[question:NI202]

If an antenna is perfectly matched to the feeder (e.g. the coaxial cable), the SWR meter shows a value of $\num{1}$. This is the best value that can be achieved. All the power is then taken up by the antenna. No power is reflected back into the transmitter.

<margin>
[picture:670:n_trx_kabel_swr_antenne:Schematic of an SWR meter between transceiver  and antenna]
</margin>

[question:NG301]
[question:NI203]

---

If no antenna at all is connected to the transceiver, or if the transmission line is either broken or short-circuited, the SWR is almost infinite ($\infty$). This is because an open or short-circuited cable reflects all the transmit power. In the worst case this can even destroy the transmitter in the radio.

<indepth>
Besides the two *SWR* values $\num{1}$ and infinity ($\infty$), the values $\num{2}$ and $\num{3}$ on the right also stand out. With an SWR of $\num{2}$, $\qty{11}{\percent}$ of the transmit power is reflected back into the transmitter; with an SWR of $\num{3}$, $\qty{25}{\percent}$. In modern transceivers, damage to the transmitter is prevented by the radio reducing the transmit power automatically.
</indepth>

A very poor SWR, for example close to infinity, can also result if the antennas are very poorly matched or the transmission line is damaged.

[question:NG302]
[question:NG303]

If an antenna that is poorly matched is connected through a long coaxial cable to a radio with an SWR meter, the SWR reading can be considerably better than the poor match would lead you to expect. The reason for this is a high cable loss, which reduces not only the signal travelling to the antenna but also the reflected signal.

[question:NG208]
