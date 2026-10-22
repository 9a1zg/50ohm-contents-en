* Hamnet, the network for radio amateurs only, is based on the Internet Protocol (IP).
* That is why Hamnet can be used with the same software as is used for the internet.
* In the simplest case, this is a web browser.

---

* The Internet Protocol (IP) assigns IP addresses to the computers involved, so that they can reach each other.
* IP addresses are written as four decimal numbers with a dot between them. Example: 141.17.5.18
* Each decimal number is 8 bits long, so the largest possible number is 255 (binary: 11111111).

<note>
There are two versions, IPv4 and IPv6. Here we deal with version 4.
</note>

---

* IP addresses are divided into a network part and a host part.
* For all computers in the same network, the beginning of the IP addresses is the same; this beginning is called the network part.
* The size of the network part varies, depending on how many computers (hosts) are to be managed in the network.

---

Examples:

     *10*.100.234.22 (small network part, large host part)
     
     *192.168.1*.252 (large network part, small host part)
     
This principle is familiar from the telephone network. Large cities have shorter area codes than small towns.

---

[picture:699:netzmaske:IPv4 address and netmask in decimal and binary notation]

* A subnet mask indicates how an IP address is divided into network part and host part, by showing all the bits of the network part as 1.

---

* There are two ways of writing this down; example for a network part of 24:
* 255.255.255.0, which is 11111111.11111111.11111111.00000000 in binary.
* The notation with the slash, for example 192.168.111.90/24

<note>
The number after the slash gives the number of ones in the subnet mask.
</note>

---

[picture:706:netzwerk:Part of a network infrastructure]

* Network devices can communicate directly with each other only within their own local network.

--- data-transition="none"

[picture:706:netzwerk:Part of a network infrastructure]

* They recognise this by the fact that their own IP address and subnet mask give the same network part as those of the other device.

--- data-transition="none"

[picture:706:netzwerk:Part of a network infrastructure]

* In all other cases they send the data to a router. This is an intermediate station that connects two or more networks with each other, in order to forward the data packets.

---
[question:EE412]

---
[question:EE414]

---
[question:EE413]
