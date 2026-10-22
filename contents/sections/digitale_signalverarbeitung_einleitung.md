<margin>
[picture:911:e_digitale_signalverarbeitung_blockschaltbild:Principle of digital signal processing]
</margin>

Over the last 25 years the world has changed enormously in technological terms. The computing power of computers has increased many times over, and more and more tasks in technical equipment are carried out by microchips in the smallest of spaces. This development will continue at a rapid pace in the coming years as well. All this changes the way in which equipment, and in particular signal processing in modern radios, is implemented. Digital signal processing is now state of the art, and every modern device is based on this technology. Digital signal processors and the basic principle of digital signal processing play a particularly important part here.

Digital signal processing is not found only in radio engineering. Many devices, be they mobile phones, stereo systems or medical imaging systems, as well as practically all modern radio applications, benefit from this fascinating technology, which makes it possible to implement previously unknown possibilities and functions in these devices at low cost.

In radio engineering, equipment that processes signals by means of digital signal processing is known as SDR equipment. In such equipment, at least part of the signal processing is implemented in software.

[question:EF603]

To be able to process continuous analogue signals digitally, they must first be sampled by means of an analogue-to-digital converter (A/D converter) and converted into digital values. This is called digitisation of the analogue input signal.

[question:EF602]

---
<margin>
[picture:411:e_digitale_signalverarbeitung:Simple representation of a sine wave made up of $\num{16}$ samples and $\num{7}$ values]
</margin>

The analogue signal is sampled at fixed time intervals and mapped onto a digital range of values (e.g. from $\num{-128}$ to $\num{+127}$). Each value represents a particular measured signal voltage; as a rule, negative values are assigned to negative voltages and positive values to positive voltages. You can picture this roughly like a film camera, for example, which takes pictures of a scene at fixed intervals. Each picture taken is always a fixed time after the previous one and before the next, and together they show the scene as it is at each moment, at short intervals of time. This process is called sampling. The individual measured signal values are called samples. In the next section we will look at this process in a little more detail.

After the A/D conversion, the samples, which are now available as digital values, can be processed further in any way by means of digital signal processing.

After the digital signal processing, you will want to turn the digitally processed signals back into an analogue signal, e.g. for output through a loudspeaker or for transmission via an antenna. To turn the digital values back into an analogue signal, a digital-to-analogue converter (D/A converter) is needed at this point, which is in practice the counterpart of the A/D converter described above. The D/A converter converts digital values back into analogue voltage values and so makes it possible to reconstruct an analogue signal from the digital values.

[question:EF601]