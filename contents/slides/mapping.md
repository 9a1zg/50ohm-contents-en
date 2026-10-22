## Mapping

* Bits have to be assigned to the possible symbols.
* This assignment is called *mapping*.
* The building block for it is called a *mapper*.
* It converts bit combinations into symbols.

[picture:1102:a_mapper:Block diagram of a mapper]

---

## Example: ASK

* In ASK, the symbols differ in their amplitude.
* Binary ASK uses two amplitudes.
* Example:
  * small amplitude → $0$
  * large amplitude → $1$

[picture:700:a_ask:ASK (amplitude-shift keying) over time]

---

## ASK in the constellation diagram

<left>
* Both symbols lie on the I axis.
* The phase stays the same.
* The distance from the origin describes the amplitude.
* The mapping assigns a bit value to each point.
</left>
<right>
[picture:1128:a_ask_mapping:ASK (amplitude-shift keying) in the constellation diagram]
</right>

---

## 4ASK

* ASK is not limited to two amplitudes.
* Four amplitudes give four symbols.
* Four symbols can transmit two bits per symbol: $00$, $01$, $10$, $11$

[picture:701:a_4_ask:Quaternary amplitude-shift keying]

---

## 4ASK in the constellation diagram

<left>
* With 4ASK, too, all points lie on the I axis.
* The points differ only in their distance from the origin.
* Each point is assigned a bit combination.
</left>
<right>
[picture:1129:a_4_ask_mapping:4ASK in the constellation diagram]
</right>