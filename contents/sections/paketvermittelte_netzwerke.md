<margin>
[include:hamnet_map]
</margin>

HAMNET plays a special role in amateur radio – a network reserved exclusively for radio amateurs. HAMNET (Highspeed Amateurradio Multimedia Network) is an IP-based network developed and operated by radio amateurs. It works in a similar way to the internet, but mostly uses radio links for data transmission.

HAMNET was originally designed as a gradual replacement for the packet radio network that had existed since the 1980s, and it has now almost completely replaced it. The fast data links between the individual access points and nodes are mainly implemented on the 6 cm, 9 cm and 13 cm microwave bands. To access HAMNET you need a clear line of sight to a HAMNET node with user access, and a suitable Wi-Fi transceiver with a directional antenna.

---

<margin>
The *DARC* offers its members VPN access via what is known as the [HAMCloud](https://50ohm.de/hc). This makes it possible to access HAMNET even when no direct access by radio is possible.   

[Become a DARC member now!](https://50ohm.de/mw)
</margin>

Hamnet can be used just like the internet, in the simplest case with a web browser. This is possible because what is known as the Internet Protocol (IP), and everything built on it, can also be used for purposes other than the internet.

[question:EE414]

Like the internet, Hamnet is an interconnection of many individual networks. If two users cannot reach each other directly, the data packets are forwarded accordingly via other nodes.

[question:EE412]

In such large structures, order is created by numbering all the computers. The users' numbers are called IP addresses. There are two versions, IPv4 and IPv6. For our hobby it is usually enough to deal with the simpler version 4.

IPv4 addresses are binary numbers 32 bits long. They are written as four decimal numbers, each standing for 8 bits, with dots between them. The largest possible number is 255, corresponding to the binary number 11111111.

For all computers in the same network, the beginning of the IP addresses is the same. This network part has a variable length. Large networks need many of the 32 bits to number their computers at the end, in what is known as the host part. For this they use a shorter network part. With small networks it is exactly the other way round. This principle is familiar from the telephone network. The largest cities have three-digit area codes, for example 089, and small local exchanges five- or six-digit ones such as 038725.

---

The simplest way to give the length of the network part is with a slash after the IP address. 141.17.5.18/24, for example, means that the network part is 24 bits long. For all computers in the same network, the address begins with 141.17.5. Only 8 of the 32 bits are left for numbering all the stations. So it is a relatively small network.

<indepth>
Networks are sometimes assigned to a so-called class, although this system was abolished long ago. Class A meant /8, Class B /16 and Class C /24.
</indepth>


---

Most network devices require a different notation, namely the subnet mask (see Figure [ref:netzmaske]). This is 32 bits in the same notation as IP addresses. Bits that stand for the network part are marked with a 1, and bits of the host part with a 0. The netmask therefore begins with as many ones as the network part is long. The rest is filled up with zeros. Home networks and small company networks almost always use the netmask 255.255.255.0, which means the same as /24.

Network devices can communicate directly with each other only within their own local network. They recognise this by the fact that their own IP address and subnet mask give the same network part as those of the other device. In all other cases they send the data to a router. This is an intermediate station that connects two or more networks with each other. If a device is connected directly to several networks, it has its own IP address in each of them.

<margin>
[picture:699:netzmaske:IPv4 address and netmask in decimal and binary notation]
</margin>

<margin>
[picture:706:netzwerk:Part of a network infrastructure]
</margin>

All users of a network should be able to use the router practically simultaneously. That is why no fixed lines are switched through in IP networks. Instead, the computers split all data streams into packets, that is, into short sections. Forwarding these individual packets is called packet switching.

[question:EE413]