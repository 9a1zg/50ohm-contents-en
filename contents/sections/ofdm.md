It is also possible to spread a data stream over several carriers that lie on different but closely spaced frequencies. The carriers cannot, however, lie arbitrarily close together, since the sidebands that inevitably arise give them a certain width.

In orthogonal frequency-division multiplexing (OFDM), the individual carriers are placed at exactly the spacing at which mutual interference between them (what is known as "crosstalk") is avoided as far as possible.

The higher the symbol rate per carrier, the larger the carrier spacing has to be. For this reason, a lower symbol rate is often chosen for each individual carrier, so that correspondingly more carriers fit in. The amount of information transmitted stays the same: although less information can be transmitted per carrier, more carriers can be used side by side. A larger carrier spacing is helpful, for example, to make the signal more tolerant of frequency errors, whether these come from frequency deviations between transmitter and receiver or from Doppler shift with moving transmitters or receivers.

One advantage of this approach is that narrow-band interference affects only one or a few carriers. Combined with the error correction methods with redundant data transmission that we met a few chapters ago, it is thus possible to achieve error-free transmission despite narrow-band interference.

<margin>
[picture:704:ofdm:Frequency spectrum of a simple OFDM signal]
</margin>

[question:AE421]

A further advantage arises from the lower symbol rate of each individual carrier. Because of the lower symbol rate, each symbol lasts longer. If there are time shifts due to multipath propagation, the proportion of overlap between the signals (known as intersymbol interference, or crosstalk between symbols) is then correspondingly smaller. It can also happen that individual frequencies are cancelled out, or at least strongly attenuated, by multipath propagation (this is called frequency-selective fading). This can be compensated for by the same mechanisms as the narrow-band interference mentioned above. OFDM is therefore particularly advantageous where there is multipath propagation.

[question:AE422]