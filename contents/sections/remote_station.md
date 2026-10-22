In Class N we have already learnt that remote operation is only permitted for Class A radio amateurs. So here we now want to look at some technical aspects of remote operation that are relevant to operating and using a remote station. 

A station for remote operation consists of several functional blocks that can be separated from one another logically. In modern equipment, parts of these functional blocks may also be integrated in a single unit (e.g. a transceiver with a network connection and remote interface).

An arrangement for remote operation can be represented logically by the following functional blocks.

---

<margin>
[picture:501:a_remotebetrieb:Block diagram of remote operation]
</margin>

* *Operator's computer and control unit (Block 1)*: This is used to control the remote station. Audio signals and control signals are converted locally into network packets and transmitted to the remote station. Control and audio signals received from the remote station (which are transmitted over the network) are made audible and visible again by the computer/control unit.
* *Network*: The connecting network or networks between the operator's location and the remote station. The internet can also serve as the network between the locations.
* *Computer or remote interface at the remote site (Block 2)*: This converts network packets received from the operator into control signals and audio signals for further control of the transceiver at the remote site and, on the return path, transmits the transceiver's received audio signals over the network to the operator. Transceiver settings and returning control signals are also transmitted over the network to the operator.
* *Transceiver/amplifier/tuner/antenna rotator (Block 3)*: These devices are controlled by the remote interface or a computer at the remote site, and report back to it, by means of signals that the operator transmits over the network to the remote interface.

[question:AF701]
[question:AF702]
[question:AF704]
[question:AF703]
[question:AF705]

---

In remote operation, transit times in the network and processing times for encoding and decoding audio signals cause delays. These must be taken into account when operating via remote stations.

<tip>
[photo:342:a_remote_station:Remote station of the DARC e. V.]

The DARC e. V. runs a number of remote club stations for its members, spread across the whole of Germany. On [mein.darc.de](https://mein.darc.de/), members can log in to the remote stations and operate over the internet if they hold a Class A licence. For Classes N and E, only SWL operation is possible.

[Become a DARC member now!](https://50ohm.de/mw)
</tip>

[question:AF709]
[question:AF710]

To make sure that a remote station does not fall into an uncontrolled state or uncontrolled operation if the data connection between user/control unit and remote interface is broken or disrupted, permanent monitoring and feedback between operator and remote station by means of what is called a watchdog is necessary. Here, for example, data packets are sent from the remote station to the operator's computer at intervals of a few seconds, and they must be acknowledged by a reply within a certain time. If this reply does not arrive, the remote station knows that the connection to the operator has been broken, and it can automatically put the transceiver into a defined safe state (e.g. receive mode) and interrupt any transmission in progress.

[question:AF708]

Since the transceiver itself can also get into an undefined state (e.g. through software or hardware faults in the unit), it should be possible to switch off the transceiver's supply voltage remotely. This can be done, for example, with an IP-controlled mains socket that the operator can control over the network.

[question:AF707]

When operating a remote station, you must also take into account, and expect, that components of the remote station may suffer interference from the transceiver at the remote station's location.

[question:AF706]