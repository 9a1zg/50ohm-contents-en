In wireless communication, various access methods play a central role in allowing several users to use a shared frequency spectrum at the same time. The common methods are frequency-division multiple access (FDMA), time-division multiple access (TDMA) and code-division multiple access (CDMA). Each of these methods divides up the frequency spectrum in a different way in order to minimise interference and ensure efficient transmission. The choice of method depends on the specific requirements for bandwidth, number of users and susceptibility to interference. The differences between these methods are described below.

---

In frequency-division multiple access (FDMA), the available frequency band is divided into several separate frequency channels (see Figure [ref:e_fdma]). Each of these channels is permanently assigned to a single user, so that several users can use the system at the same time. The users are separated solely by different frequencies, so the signals of the individual users do not interfere with one another as long as the channel spacing is maintained. FDMA is a technically simple method that has been established for many years and is particularly suitable for systems with few users and low interference requirements. One disadvantage, however, is the comparatively poor bandwidth efficiency with a large number of users, since each user keeps a frequency range of their own permanently reserved, even when they are not transmitting any data for a while. Typical applications of FDMA are early analogue mobile phone systems such as AMPS and various forms of satellite communication.

[question:EE410]

<margin>
[picture:845:e_fdma:Frequency-division multiplexing]
</margin>

---

In time-division multiple access (TDMA), several users use the same frequency channel by dividing up their access to it in time. Each user is given fixed, defined time intervals, known as time slots, in which they may transmit and receive (see Figure [ref:e_tdma]). This separation of the transmissions in time prevents the signals of the individual users from overlapping or interfering with one another.

TDMA allows comparatively efficient use of the available frequency resources, especially in systems with many users and a high volume of data. Smooth operation does, however, require very precise time synchronisation of all users, which increases the technical effort and the complexity of the system. Well-known applications of TDMA are the second-generation GSM mobile phone system, the DECT cordless telephone system and, in amateur radio, DMR.

[question:EE409]

<margin>
[picture:844:e_tdma:Time-division multiplexing]
</margin>

---

In code-division multiple access (CDMA), all users use the same frequency range at the same time. The individual users are separated not by frequency or time but by individual spreading codes (see Figure [ref:e_cdma]). Each user is assigned a code of their own, with which their signal is modulated. These codes are chosen so that the superimposed signals can be separated from one another again at the receiver, although they are transmitted at the same time in the same frequency band. CDMA is notable for high flexibility and a large system capacity, since many users can be active at the same time. The method is also very robust against interference and multipath propagation. Against this, however, stand comparatively complex signal processing and greater demands on the hardware, particularly with a large number of active users. Typical applications of CDMA are third-generation mobile phone systems such as UMTS and the satellite navigation system GPS.

[question:EE411]

<margin>
[picture:846:e_cdma:Code-division multiplexing]  
</margin>

In summary, FDMA is the simplest method, while TDMA and CDMA become increasingly efficient and complex, particularly where bandwidth is limited and user numbers are high. CDMA allows the greatest flexibility, but also requires the most elaborate technology to implement.