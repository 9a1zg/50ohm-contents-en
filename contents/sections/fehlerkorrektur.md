If the receiver detects a transmission error, for example with the help of check bits, it can ask the transmitter to transmit the data again. With *forward error correction* (FEC), on the other hand, a retransmission is often not necessary. For this, additional information is added to the user data, for example several check bits. Under certain conditions this enables the receiver not only to detect that an error has occurred, but also to determine which bit is faulty, and to correct it.

How this can work in detail is shown in the *In depth* box alongside, using a Hamming code as an example. The exact method is not required for the examination.

[question:AE413]
[question:AE414]

<indepth>
The Hamming code is an error correction method that uses several parity bits. Let us assume that we want to transmit the following $\num{11}$ data bits:

[picture:683:hamming1: ]

So that a single bit error can be not only detected but also corrected, we must be able to determine at which position the error occurred. To do this, we first look at the positions of the individual bits and name them alphabetically:

[picture:682:hamming2: ]

Now we arrange the data bits somewhat differently and add four extra parity bits, $p_1$ to $p_4$:

[picture:684:hamming3: ]

The four parity bits check different, overlapping groups of bits:

[picture:685:hamming4: ]

Each parity bit protects a particular group:

[picture:686:hamming5: ]

For each of these groups, we now calculate the corresponding parity bit with *even parity*:

[picture:687:hamming6: ]

If a single bit error occurs in the transmission, certain parity checks fail. From the combination of failed checks, it is possible to determine at which position the error occurred. The faulty bit can then be inverted and so corrected.

If, for example, bit $k$ becomes a $\num{0}$ during the transmission, all four parity checks, $p_1$ to $p_4$, fail. Only bit $k$ belongs to all four groups checked. The error must therefore be in bit $k$.

If, on the other hand, an error occurs in bit $a$, only the parity checks of $p_1$ and $p_2$ fail, while the checks of $p_3$ and $p_4$ succeed. From this pattern the receiver can tell that bit $a$ is faulty.

An error in a parity bit itself can also be detected and corrected. If, for example, $p_1$ is faulty, only the parity check belonging to $p_1$ fails, while the checks of $p_2$, $p_3$ and $p_4$ succeed. The error must therefore be in $p_1$.

The Hamming code shown here is designed to correct a single bit error. If several bit errors occur at the same time, the actual error position can no longer be inferred reliably from the parity checks. Extended Hamming codes can, for example, also reliably detect two bit errors occurring at the same time.
</indepth>