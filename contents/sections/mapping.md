In digital transmission methods, the bits to be transmitted have to be assigned to the various possible symbols. This assignment is called *mapping*. The building block that carries out this assignment is called a *mapper*. The block symbol of a mapper is shown in Figure [ref:a_mapper]. The mapper takes in a digital bit stream and assigns the bit combinations it contains to the corresponding symbols in a constellation diagram.

<margin>
[picture:1102:a_mapper:Block diagram of a mapper]
</margin>

---

To get to know the principle of mapping, let us first consider *amplitude-shift keying* (ASK), already familiar from Class E. Figure [ref:a_ask] shows binary ASK in the time domain. Here the amplitude of the carrier signal is switched between two values. For example, a large amplitude can represent the bit $1$ and a small amplitude the bit $0$.

<margin>
[picture:700:a_ask:ASK (amplitude-shift keying) over time]
</margin>

---

The two possible symbols can also be shown in the constellation diagram we met earlier. Since in this example only the amplitude changes and the phase stays the same, both signal points lie on the I axis. The different distances from the origin correspond to the two different amplitudes. Each of the two signal points is now assigned a bit value by the mapping.

<margin>
[picture:1128:a_ask_mapping:ASK (amplitude-shift keying) in the constellation diagram]
</margin>

---

Amplitude-shift keying is not limited to two possible amplitudes. If, for example, four different amplitudes are used, four different symbols are available. Since two bits can form four different bit combinations, each symbol can be assigned one of the combinations $00$, $01$, $10$ or $11$.

Figure [ref:a_4_ask] shows such a *4-ASK* with four different amplitudes in the time domain. For example, $\qty{25}{\percent}$, $\qty{50}{\percent}$, $\qty{75}{\percent}$ and $\qty{100}{\percent}$ of the maximum amplitude can be used. Two bits can therefore be transmitted with each symbol.

<margin>
[picture:701:a_4_ask:Quaternary amplitude-shift keying]
</margin>

The constellation diagram now also has four possible signal points. Since still only the amplitude changes, in this example all four points lie on the I axis. Each point is assigned a particular bit combination.

<margin>
[picture:1129:a_4_ask_mapping:Quaternary amplitude-shift keying in the constellation diagram]
</margin>
