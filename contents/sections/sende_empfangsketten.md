The following section describes the individual steps of a transmit and receive chain. Figure [ref:a_sdr_sender] shows, as an example, an SDR transmitter for voice communication. In the first step, the microphone signal is digitised by an analogue-to-digital converter. The digital signal is then compressed by a source encoder to reduce the bandwidth needed. In the next step, a channel encoder deliberately adds redundancy to the compressed signal, so that transmission errors can be detected and corrected. Finally, the encoded data are converted into symbols by a mapper and then modulated by an I/Q modulator. The transmit chain ends with a power amplifier and the antenna, from which the signal is radiated.

<margin>
[picture:1062:a_sdr_sender:SDR transmitter for voice communication]
</margin>

The blocks highlighted in blue in Figure [ref:a_sdr_sender] represent the signal processing steps, which can be implemented, for example, purely in software or with an FPGA. For a transmitter, the order of these processing steps is always as follows, and it should be memorised well for the examination questions:

1. Source encoder: compress the data
2. Channel encoder: add redundancy for error detection and correction
3. Mapper: map binary data onto symbols, e.g. amplitude and phase for QAM

[question:AF626]
[question:AF627]

---

For a receiver, the whole thing works in reverse: the antenna receives the signal, which is amplified by a power amplifier. Demodulation then takes place in an I/Q demodulator to extract the symbols. The de-mapper maps these symbols back to the original binary data. After that, the channel decoder takes on the task of detecting and correcting errors that may have arisen during transmission. Finally, the source decoder decompresses the data to restore the original signal, which can then be converted back into an analogue signal by a digital-to-analogue converter and output, for example, to a loudspeaker via an amplifier.

We sum up the digital signal processing in the receiver in the following three steps:

1. De-mapper: map the symbols onto binary data
2. Channel decoder: detect and correct errors
3. Source decoder: decompress the data

<margin>
[picture:1063:a_sdr_empfänger:SDR receiver for voice communication]
</margin>

[question:AF628]
[question:AF629]
