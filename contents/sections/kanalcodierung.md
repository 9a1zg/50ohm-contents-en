Figure [ref:kanal] shows a transmitter and a receiver connected to each other by a channel. Interference on the channel can arise, for example, from the weather, other atmospheric influences or transmissions from other stations. This can lead to errors in the transmission. 

<margin>
[picture:674:kanal:Channel]
</margin>

Unlike source coding, channel coding deliberately adds redundancy to the information to be transmitted, for example repetitions or checksums. In contrast to the redundancy removed in source coding, this systematically added redundancy can be used to detect or correct transmission errors automatically.

---

Figure [ref:kanalcodierer] shows a symbol for a channel encoder. The block shows that redundancy is added to the data.

<margin>
[picture:676:kanalcodierer:Channel encoder]
</margin>

[question:AE409]

We distinguish two kinds of channel coding:

* Error detection: it is possible to detect that an error has occurred in the transmission, and then, for example, to request a retransmission.
* Forward error correction: errors that arise in the transmission are corrected at the receiver with the help of the redundancy. 

In the following we will look at these two kinds more closely.