*Converters* and *transverters* are used in amateur radio to open up additional frequency ranges with existing radios that these radios do not originally cover. A *converter* converts the signal in one direction only, either in the transmit path or in the receive path. A *transverter*, on the other hand, has internal transmit/receive switching and performs the frequency conversion both on transmit and on receive. In converters and transverters, the frequency conversion is always done by mixing in one or more mixers.

For example, with a suitable transverter and an existing HF transceiver you can also operate in the VHF/UHF/SHF range. Here you would, for example, use a transverter to convert the $\qty{10}{\meter}$ band of the HF transceiver to $\qty{2}{\meter}$/$\qty{70}{\centi\meter}$ or $\qty{23}{\centi\meter}$, in both directions.

[question:EF501]
[question:EF502]

---

As a first step, let us look at the block diagram of a converter in Figure [ref:e_konverter]. Such a converter could be used, for example, to convert a signal from a VHF radio for the amateur satellite QO-100, which needs an input frequency in the $\qty{2.4}{\giga\hertz}$ band. A transverter may not be necessary here, since reception is via an SDR stick and an LNB.

The block diagram shows that a defined input frequency range is converted to a different output frequency range with the help of at least one mixer. No transmit/receive switching is provided. A converter can therefore convert a signal in one direction only, either in the receive (RX) or in the transmit path (TX). Converters for transmitting often have a PTT control, which activates the converter's amplifier stages when transmitting.

The frequency band to which a converter converts the signal can be calculated from the oscillator frequency fed to the mixer and the input or output frequency. In this particular example, the target frequency results from the mixing product
$\qty{144}{\mega\hertz} + \qty{2.256}{\giga\hertz} = \qty{2.4}{\giga\hertz}$,
the desired product then being selected by suitable filters.

<margin>
[picture:651:e_konverter:Converter circuit, e.g. for QO-100]
</margin>

[question:EF504]

---

The circuit of a transverter is easy to tell apart from that of a converter. Figures [ref:e_transverter_rx] and [ref:e_transverter_tx] show the block diagram of a transverter that makes it possible to operate on the $\qty{2}{\meter}$ band with a $\qty{10}{\meter}$ HF transceiver. For this, transmit/receive switching is used together with two mixers and two separate signal paths – one for receive (RX) and one for transmit (TX).

When transmitting, the TX branch converts the output signal of the transceiver to the desired higher frequency band, while when receiving, the RX branch mixes the signal coming from the antenna down to the frequency band suitable for the transceiver. Between which frequency bands the transverter works can be calculated from the oscillator frequency fed to the mixers and the respective input and output frequencies. These relationships are shown in the figures.

The crystal-controlled oscillator ($G$) generates a frequency of $\qty{38.666}{\mega\hertz}$, which is raised to $\qty{116}{\mega\hertz}$ with the help of a 1:3 frequency multiplier. On receive, shown in Figure [ref:e_transverter_rx], the input signal from the frequency range $\qtyrange{144}{146}{\mega\hertz}$ is mixed down to the range $\qtyrange{28}{30}{\mega\hertz}$. On transmit, shown in Figure [ref:e_transverter_tx], the output signal of the radio from the range $\qtyrange{28}{30}{\mega\hertz}$ is mixed up to the frequency range $\qtyrange{144}{146}{\mega\hertz}$. As usual, suitable filters are used in both signal paths to select the desired mixing products; for clarity they are not drawn here.

[question:EF503]

<margin>
[picture:842:e_transverter_rx:Transverter in the RX path]
[picture:843:e_transverter_tx:Transverter in the TX path]
</margin>

Transverters and converters designed for high input or output frequencies (in the GHz range) must have a very stable oscillator. Because of the high output frequencies, errors in the oscillator frequency lead, through internal frequency multiplication, to unacceptable errors in the target frequency with narrowband modes or SSB. An error in the oscillator frequency is multiplied too when the frequency is multiplied. A so-called TCXO or OCXO is often used, which can additionally be synchronised to an external reference source (e.g. GPS), to stabilise the oscillator frequency as well as possible and keep errors in the target frequency small.

[question:EF505]