## Error detection: parity bit

* An extra check bit (parity bit) is appended to the data  
* Two variants:  
* *Even parity*: the number of ones is set to an even number  
* *Odd parity*: the number of ones is set to an odd number  
* The transmitter and the receiver must agree on the method used

---

## Even parity: example 1

<left>
[picture:677:byte:A byte]
</left>
<right>
* Byte to be transmitted  
* 5 ones are counted → odd number  
* The check bit must be set to $\num{1}$ to give an even number
</right>

---

<left>
[picture:678:even_parity:The byte with an even parity bit]
</left>
<right>
* The check bit has been set to $\num{1}$  
* The resulting byte has an even number of ones
* If an error occurs in the transmission, the check bit no longer matches
</right>

---

## Even parity: example 2

<left>
[picture:679:even_parity:Byte with even parity]
</left>
<right>
* Original byte: 4 ones (even)  
* The check bit is set to $\num{0}$
</right>

---
## Error detection with bit errors

* With a one-bit error, the parity is reversed → error detected  
* With two errors, the parity stays the same → error undetected  
* With three errors, the parity changes again → error detected

---

[question:AE411]

---

[question:AE412]

---

## Extended error detection

* Additional check bits can detect multi-bit errors  
* For messages of variable length, checksum methods such as the *cyclic redundancy check (CRC)* are often used  
* CRC detects errors except for a certain residual probability

<note>
Used for the IBAN or for identity card numbers
</note>

---

[question:AE410]
