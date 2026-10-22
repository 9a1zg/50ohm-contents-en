The simplest kind of error detection is achieved by adding an extra bit, the check bit. It is also called a *parity bit*. There are two variants of this method. With *even parity*, the value of this bit is chosen for each block so that the number of bits set to $\num{1}$ is always even. With *odd parity*, on the other hand, the number must always be odd. Before the transmission, the transmitter and the receiver must agree on which of the two variants is used.

<indepth>
Let us assume that we want to transmit the following byte with even parity:

[picture:677:byte:A byte]

We count 5 ones, that is, an odd number. The check bit must therefore be set to $\num{1}$, so that the result is an even number of ones:

[picture:678:even_parity:The byte with an even parity bit]

If a transmission error now changes *one* bit (from $\num{1}$ to $\num{0}$ or vice versa), the number of ones becomes odd. From this the receiver recognises that there is an error.

Here is a further example: 

[picture:679:even_parity:Byte with even parity]

In the original byte we count 4 ones, which is an even number. We therefore have to insert a $\num{0}$ as the check bit.
</indepth>

This method quickly reaches its limits, namely when more than one error occurs in the transmission. If two bits are changed in the transmission, the number of ones stays even. The receiver can no longer detect that errors have occurred. If three errors occur in the transmission, the result is again an odd number of ones, and the receiver detects the errors.

Odd parity works in basically the same way, with a single difference: the number of ones must be not even but always odd. For odd parity, just as for even parity, only an odd number of incorrectly transmitted bits is detected. An error-free transmission, on the other hand, cannot be distinguished from an even number of errors.

[question:AE411]
[question:AE412]

To detect multi-bit errors, further check bits can be added. This works very well for messages of a fixed length. If the length of the data is variable, special checksum methods are often used, such as the *cyclic redundancy check (CRC)*, which detect errors except for a certain residual probability. Similar methods are also found in everyday life, for example in identity card numbers or the IBAN.

[question:AE410]
