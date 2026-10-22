## Remote operation of radio stations

* Consists of several functional blocks  
* Modern equipment partly integrates several blocks  
* Separation between operator and remote site  

---

### Block diagram of a remote station

<left>
[picture:501:a_remotebetrieb:Block diagram of remote operation]
</left>
<right>
* Logical representation of the functional blocks  
* Control, network connection, remote interface  
* Transceiver and connected equipment  
</right>

---

#### Operator's computer and control unit (Block 1)

<left>
[picture:501:a_remotebetrieb:Block diagram of remote operation]
</left>
<right>
* Converts audio and control signals into network packets  
* Received signals are made audible and visible  
</right>

---

#### Network

<left>
[picture:501:a_remotebetrieb:Block diagram of remote operation]
</left>
<right>
* Connects the operator with the remote site  
* The internet can be used  
</right>

---

#### Remote interface at the remote site (Block 2)

<left>
[picture:501:a_remotebetrieb:Block diagram of remote operation]
</left>
<right>
* Converts network packets into control and audio signals  
* Sends received audio signals back to the operator  
</right>

---

#### Transceiver/amplifier/tuner/antenna rotator (Block 3)

<left>
[picture:501:a_remotebetrieb:Block diagram of remote operation]
</left>
<right>
* Controlled via the remote interface  
* Feedback on the control commands comes over the network  
</right>

---

[question:AF701]

---

[question:AF702]

---

[question:AF704]

---

[question:AF703]

---

[question:AF705]

---

### Delays in remote operation

* Network and processing times lead to latency  
* Encoding and decoding of audio signals cause delays  
* Must be taken into account in radio operation  

---

[question:AF709]

---

[question:AF710]

---

### Watchdog for monitoring the remote station

* Prevents an uncontrolled state if the connection is lost  
* Regular exchange of data packets between station and operator  
* If there is no reply, the transceiver switches to a safe state  

---

[question:AF708]

---

### Switching off the power supply remotely

* The transceiver may get into an undefined state  
* It should be possible to switch off the supply voltage remotely  
* Solution: IP-controlled mains socket, controlled over the network  

---

[question:AF707]

---

### Interference from the transceiver

* The remote station can suffer interference from its own signals  
* Appropriate interference-suppression measures are needed  

---

[question:AF706]
