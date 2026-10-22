We humans are used to using the ten digits from $\num{0}$ to $\num{9}$. This is called a base-ten system or decimal system.

For computers, on the other hand, it is simpler to work with only $\num{2}$ digits: $\num{0}$ and $\num{1}$. These correspond to two states: for example off and on, "transistor cut off" and "transistor conducting", or $\qty{0}{\volt}$ and $\qty{5}{\volt}$. The result is a binary number system (in German also called *Dualsystem*).

[question:EA201]

Counting works the same way in all number systems (see Table [ref:binaer_zahlensysteme]): you start at $\num{0}$ and count up through the digits. When you run out of digits, you start again from the beginning and write a $\num{1}$ in front of each number. That is why $\num{10}$ follows $\num{9}$ in the decimal system. The digit on the far right has the value that it represents itself. This is called the place value $\num{1}$. 

---

In the decimal system, the second digit from the right is worth ten times its own value, so it has the place value $\num{10}$. Each position further to the left is worth ten times as much as the one to its right. For example, the decimal number $\num{5573}$ from Table [ref:binaer_stellenwert_dezimal] actually means $5 \cdot 1000 + 5 \cdot 100 + 7 \cdot 10 + 3 \cdot 1$.

<margin>
|c: |c: |c: |c: |
|$\num{1000}$ | $\num{100}$ | $\num{10}$ | $\num{1}$ |
| $\num{5}$ | $\num{5}$ | $\num{7}$ | $\num{3}$ |
[table:binaer_stellenwert_dezimal:Place values of the four-digit decimal number $\num{5573}$]

|r: Decimal | r: Binary |
| $\num{0}$ | $\num{0}$ |
| $\num{1}$ | $\num{1}$ |
| $\num{2}$ | $\num{10}$ |
| $\num{3}$ | $\num{11}$ |
| $\num{4}$ | $\num{100}$ |
| $\num{5}$ | $\num{101}$ |
| $\num{6}$ | $\num{110}$ |
| $\num{7}$ | $\num{111}$ |
| $\num{8}$ | $\num{1000}$ |
| $\num{9}$ | $\num{1001}$ |
| $\num{10}$ | $\num{1010}$ |
| $\num{11}$ | $\num{1011}$ |
| $\num{12}$ | $\num{1100}$ |
| $\num{13}$ | $\num{1101}$ |
| $\num{14}$ | $\num{1110}$ |
| $\num{15}$ | $\num{1111}$ |
[table:binaer_zahlensysteme:Numbers in the decimal and the binary system]
</margin>

The binary system has only two digits, namely $\num{0}$ and $\num{1}$. As can be seen in Table [ref:binar_stellenwert_dual], the first position from the right has the place value $\num{1}$, the second $\num{2}$, the third $\num{4}$, the fourth $\num{8}$ and so on. The place values double instead of increasing tenfold, because there are only two digits and not ten. A position in the binary system is also called a bit ($\unit{\bit}$).

|c: |c: |c: |c: |c: |c: |c: |c: |
| $\num{128}$ | $\num{64}$ | $\num{32}$ | $\num{16}$ | $\num{8}$ | $\num{4}$ | $\num{2}$ | $\num{1}$ |
| $\num{1}$ | $\num{0}$ | $\num{0}$ | $\num{0}$ | $\num{1}$ | $\num{1}$ | $\num{1}$ | $\num{0}$ |
[table:binar_stellenwert_dual:Place values of the eight-digit binary number $\num{10001110}$]

Once you know the place values, converting binary numbers into the decimal system is easy. Let us take an example from Table [ref:binar_stellenwert_dual]. The binary number $\num{10001110}$ is to be converted into a decimal number.

1. Write the place value above each digit of the binary number.
2. Add up all the place values that have a $\num{1}$ below them: $128+8+4+2=142$

[question:EA206]
[question:EA207]
[question:EA208]

On paper, you can write binary numbers with as many bits as you happen to need. In digital technology it is different. The hardware or software specifies a certain number of digits, which is also called the width. For example, microcontrollers or computers often have widths of $\num{8}$, $\num{16}$, $\num{32}$ or $\qty{64}{\text{bits}}$. When binary numbers are written out, they are often padded with zeros at the front until this width is reached. This does not change the value of the number.

[question:EA205]

A fixed width limits the range of values. With one bit, two values are possible ($\num{0}$ and $\num{1}$), with two bits already four ($\num{00}$, $\num{01}$, $\num{10}$ and $\num{11}$), and with each additional bit twice as many. With $n$ bits, $2^n$ different numbers can be represented.

[question:EA204]
[question:EA202]
[question:EA203]
