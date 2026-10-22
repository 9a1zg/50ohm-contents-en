The transmit power generated in the transmitter should be radiated by the antenna as completely as possible and without losses. For this reason, special antenna feeders are needed, which in technical language are called transmission lines.

<margin>
[photo:65:n_Koax_Detail:Coaxial cable in detail]
</margin>

The most widespread is the *coaxial cable* (Figure [ref:n_Koax_Detail]). In everyday speech it is often shortened to coax. Coaxial cables consist of an inner and an outer conductor, insulated from each other. They are tubular and surrounded by a protective sheath. Coaxial cables come in a wide variety of designs:
* thick or thin
* with a flexible or rigid inner conductor
* with outer conductors of wire braid and/or foil, or even of solid copper tube

% Nach Ticket #20292449 erstmal entfernt
%<margin>
%Die *Dämpfung* kann mit dem Wasserstrahl aus einem Gartenschlauch veranschaulicht werden: Ist der Schlauch %kurz, so tritt am Ende ein kräftiger Wasserstrahl aus. Ist der Schlauch hingegen sehr lang, so ist der austretende %Wasserstrahl schwach.
%</margin>

<margin>
[photo:66:n_Koaxialkabel:Examples of common coaxial cables]
</margin>

But even in the best coaxial cable there is a loss, because part of the transmit power is converted into heat. How high the losses of a transmission line are is given by what is called the *cable loss*, which data sheets usually state in decibels ($\unit{\dB}$) per $\qty{100}{\meter}$. The longer a coaxial cable is, the higher the loss due to attenuation. The frequency of the electrical oscillation also plays a part: the cable loss increases with increasing frequency.

[question:NG207]

Another important characteristic of transmission lines is the *characteristic impedance*, which is stated in ohms ($\unit{\ohm}$). It is a property that depends on how the line is constructed, among other things on the spacing between the inner and outer conductors. The length of the line has no effect on the characteristic impedance.

If transmission lines with different characteristic impedances are connected together, unwanted reflections of radio-frequency oscillations occur at the junction. As a result, part of the transmit power is reflected back into the transmitter, so it cannot be radiated, and in the worst case it can even damage the transmitter.

The antenna connector of amateur radio equipment is almost always designed for a characteristic impedance of $\qty{50}{\ohm}$. Accordingly, the coaxial cables common in amateur radio have a characteristic impedance of $\qty{50}{\ohm}$. In television engineering, coaxial cables with a characteristic impedance of $\qty{75}{\ohm}$ are also common. Coaxial cables of $\qty{60}{\ohm}$ are found less often.

[question:NG201]
