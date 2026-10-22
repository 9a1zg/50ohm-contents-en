## Forward error correction (FEC)

* If the receiver detects an error (e.g. by means of check bits), it can ask for a retransmission  
* In forward error correction, additional redundancy (e.g. further check bits) is added  
* This shows not only that an error is present, but also where $\rightarrow$ the faulty bit can be corrected

---

[question:AE413]

---

[question:AE414]

---

## Hamming code – error correction in detail

* The Hamming code uses several parity bits, not only to detect errors but also to correct them  
* Aim: a single bit error is to be located and corrected

---

<left>
[picture:683:hamming1:Transmission of 11 bits]
</left>
<right>
* Example: transmission of an 11-bit data word  
* Aim: error detection and correction for one bit error
</right>

---

<left>
[picture:682:hamming2:Naming the bit positions alphabetically]
</left>
<right>
* The positions of the bits are named alphabetically, to identify the individual areas
</right>

---

<left>
[picture:684:hamming3:Rearrangement with additional bits]
</left>
<right>
* Arrangement of the data bits with additional bit positions for parity bits
</right>

---

<left>
[picture:685:hamming4:Four parity bits in the Hamming code]
</left>
<right>
* Instead of a single check bit, four parity bits ($p_1$–$p_4$) are used  
* These cover different areas of the data bits – similar to a crossword puzzle
</right>

---

<left>
[picture:686:hamming5:Assignment of the parity areas]
</left>
<right>
* Each parity bit protects a particular area of the data
</right>

---

<left>
[picture:687:hamming6:Calculating the parity bits (even parity)]
</left>
<right>
* For each area, the parity bit is calculated using even parity  
* If an error occurs, the faulty areas can be identified and corrected
</right>

---

<left>
[picture:687:hamming6:Calculating the parity bits (even parity)]
</left>
<right>
* The combination of the parity areas makes it possible to determine the position of the faulty bit  
* Example: if a particular bit (e.g. bit $k$) is changed during the transmission, all the parity checks belonging to it fail – so the error is in bit $k$
</right>

