In Class N we learnt that if an antenna is perfectly matched to the feeder (e.g. a coaxial cable), the SWR meter shows a value of 1. This is the best possible case, since all the transmit power is taken up by the antenna and no power is reflected back to the transmitter. If, on the other hand, no antenna at all is connected or the transmission line is broken or short-circuited, the SWR rises towards infinity ($\infty$). In these cases the transmit power is reflected almost completely. In the worst case, such complete reflection can damage the output stage of the transmitter. In Class E we now go into the subject a little more deeply and also meet values between $\num{1}$ and $\infty$.

The standing wave ratio (SWR), with the symbol $s$, can be calculated from the forward power $P_\text{V}$ and the reflected power $P_\text{R}$. We find the relationship on the formula sheet:

$s = \frac{\sqrt{P_\text{V}}+\sqrt{P_\text{R}}} { \sqrt{P_\text{V}}-\sqrt{P_\text{R}}}$

If, for example, the transmitter delivers a power of $P_\text{V}=\qty{100}{\watt}$, and $P_\text{R}=\qty{25}{\watt}$ is reflected from the antenna back towards the transmitter, this gives:

$s = \frac{\sqrt{100}+\sqrt{25}}{\sqrt{100}-\sqrt{25}} = \frac{10+5}{10-5} = \frac{15}{5} = 3$

This means that an SWR of $\num{3}$ corresponds to a reflection of $\frac{\qty{25}{\watt}}{\qty{100}{\watt}}=\qty{25}{\percent}$. Further equivalents are shown in Table [ref:e_swr_werte].

<margin>
| l: SWR | l: Reflected power |
| $\num{1}$ | $\qty{0}{\percent}$ |
| $\num{1.5}$ | $\qty{4}{\percent}$ |
| $\num{2}$ | $\qty{11.1}{\percent}$ |
| $\num{2.5}$ | $\qty{18.4}{\percent}$ |
| *$\num{3}$* | *$\qty{25}{\percent}$* |
| $\num{4}$ | $\qty{36}{\percent}$ |
| $\num{6}$ | $\qty{51}{\percent}$ |
| $\num{10}$ | $\qty{66.9}{\percent}$ |
| $\num{20}$ | $\qty{81.9}{\percent}$ |
| $\infty$ | $\qty{100}{\percent}$ |
[table:e_swr_werte:SWR values and the corresponding reflected power]
</margin>

---

<tip>
To answer the following questions, it is enough to know that a standing wave ratio of $\num{3}$ corresponds to a reflection of $\qty{25}{\percent}$ of the energy, i.e. the reflected wave carries a quarter of the energy of the forward wave. Accordingly, only $\qty{75}{\percent}$ of the energy is delivered at the end of the line, e.g. to an antenna or a loss resistance (that is, not reflected). 
</tip>

[question:EG401]
[question:EG402]
[question:EG403]
