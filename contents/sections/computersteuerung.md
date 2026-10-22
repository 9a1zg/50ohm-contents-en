The basic idea behind Morse telegraphy, transmitting the individual characters of a text, is called telegraphy and has been developed steadily. One milestone was connecting teleprinters to radios by means of a modem. This was the invention of the radio teleprinter, for sending and receiving texts automatically by radio. The abbreviation RTTY, for radio teletype, is still in use as a name. Today the job of the radio teleprinter has generally been taken over by the computer. Besides the classic RTTY method, this makes it possible to use many other digital transmission methods, which are also called data modes.

<indepth>
A *teleprinter* is a device for transmitting messages in text form by means of electrical signals.
</indepth>

<margin>
[photo:92:n_computersteuerung_funkfernschreiber:Radio teleprinter]
</margin>

---

For this, a suitable computer must first be connected to the radio. In the simplest case, the connection can be made directly via the audio socket or the USB interface. Basically you need an audio connection and, where necessary, control signals. Figure [ref:n_computersteuerung_verbindungen] shows some variants. A connection for control signals often found on transceivers is what is known as the CAT interface. CAT stands for Computer Aided Tuning or Computer Aided Transceiver. Through this interface you can control the transceiver and query values, for example frequency, transmit power and PTT status.

<margin>
[picture:630:n_computersteuerung_verbindungen:Examples of connections between computer and radio]
</margin>

However, the connection between computer and transceiver can lead to interference to the transmitted signals, or to the radio having an effect on the PC. Various data mode interfaces, as a hardware solution, make the connection easier and include measures against such problems. Such interfaces can also be used for other purposes, for example for remote operation or for recording radio communication with suitable software. For some methods there are also hardware modems, in which the conversion between data and audio signals takes place in a separate unit.

[question:NF114]
[question:NF116]

There are other unintended effects too. The computer could unexpectedly switch to transmit, or transmit notification sounds from other programs that are running. Sometimes, for example, you hear other radio amateurs accidentally transmitting the start-up sound of their operating system. If the radio transmits unexpectedly, people who are working on the antenna installation at the time, or who happen to be in its immediate vicinity, may be endangered.

[question:NF117]

---

For some transmission methods, the radio's microphone socket is unsuitable, because the amplifier and filter stages that follow it are optimised for speech and treat high and low tones differently. Radios therefore often have a separate analogue data port, labelled DATA or 9600, for example. Using this special port bypasses certain amplifier and filter stages and transfers signals with as little distortion as possible.

<indepth>
The name *9600* comes from the fact that this port was introduced for packet radio, which used to be widely used, so that data could be transmitted at $\qty{9600}{\baud}$. Today the port is used, for example, for digital voice transmission, and in some cases at higher speeds too.
</indepth>

[question:NF115]
