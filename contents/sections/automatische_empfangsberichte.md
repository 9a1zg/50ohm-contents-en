With digital transmission methods, and with CW too, received call signs can be passed on automatically to internet platforms. These platforms collect the reception reports of many radio amateurs and display them, for example, on maps that show from which locations and on which bands signals were received. In this way, current propagation conditions can be observed very clearly. Radio amateurs can use such automatic reception reports to check the range of their own transmissions or to gain a better understanding of current radio wave propagation. They also offer a simple way of comparing two antennas with each other. 

<margin>
[photo:322:e_wspr_reichweite:Test transmission by DL0JMU with a home-built FPGA-based WSPR transmitter in the $\qty{40}{\meter}$ band, at $\qty{10}{\milli\watt}$]
</margin>

WSPR stands for *Weak Signal Propagation Reporter Network* and is a special QRP data mode developed solely for investigating propagation conditions. Unlike conventional transmission methods, WSPR does not allow two-way QSOs. Instead, very short, heavily error-corrected signals are transmitted at extremely low power. Transmission is very slow: typically, a station transmits for about one minute and then receives for several minutes. The received data are passed on automatically to central servers and can then be evaluated graphically on the [WSPRnet](https://50ohm.de/wsprn) platform, for example in the form of world maps with reception reports.

For CW signals there is the [Reverse Beacon Network](https://50ohm.de/rbn). CW signals are received and analysed by automated receivers, known as "skimmer stations". As soon as a skimmer recognises your call sign, it creates a reception report, which is sent to the central RBN database. These data also include signal strength, frequency and location information.

Besides WSPRnet and the Reverse Beacon Network, [PSK Reporter](https://50ohm.de/psk) plays an important part in collecting and distributing automatic reception reports. PSK Reporter is a platform suitable not only for WSPR and CW but for a wide range of digital modes in amateur radio. Receiving stations worldwide can receive and decode signals and send their reports to PSK Reporter's central database. The supported modes include PSK31, FT8, FT4, RTTY and many more. Every receiving station that has installed and configured the appropriate software can analyse incoming signals and make its reports available online.

[question:EE405]
