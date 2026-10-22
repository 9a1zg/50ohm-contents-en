In Class N we already met the concept of power as the product of current and voltage ($P = U \cdot I$). In Class E we go further into this topic, among other things by looking at how to rearrange formulas.

---

To do this, we look at the circuit in Figure [ref:e_leistung_r]. It shows how electrical power is converted into heat in a resistor. Assuming the quantities $P$ and $R$ are known, the voltage $U$ can be determined with the help of the power formula ($P = U \cdot I$) and Ohm's law ($U = R \cdot I$).

<margin>
[picture:1013:e_leistung_r:Power is converted into heat in the resistor $R$]
</margin>
  
---

<tip>
The formulas derived here can also be found, clearly set out, in the [formula sheet](https://50ohm.de/hm). 
</tip>
  
First, we rearrange the Ohm's law equation for the current:

$\begin{align*} U &= R \cdot I &\quad\quad\quad &|~: R\\ \frac{U}{R} &= \frac{\cancel{R} \cdot I}{\cancel{R}}\\[1.5ex] I &= \frac{U}{R}.\end{align*}$

Substituting this expression for $I$ into our power formula gives:

$\begin{split} P &= U \cdot \frac{U}{R}\\P&=\frac{U^2}{R}.\end{split}$

We solve this equation for $U^2$ by multiplying both sides by R:

$\begin{align*} P &= \frac{U^2}{R} &\quad\quad\quad &|~\cdot R\\ U^2 &= P \cdot R.\end{align*}$

Now we want to determine the voltage $U$. To do so, we apply the inverse operation of squaring, namely taking the square root. This gives us:

$\begin{align*} U^2 &= P \cdot R &\quad\quad\quad &|~\sqrt{~~}\\ U &= \sqrt{P \cdot R}.\end{align*}$

In some examination questions it is important to recognise the correct relationships. With the help of the formula sheet, the correct solution can always be derived.

[question:EB504]
  
For the current $I$, too, the relationship between current $I$, resistance $R$ and power $P$ can be derived by substituting Ohm's law into the power formula.

We start with the two equations $P = U \cdot I$ and $U = R \cdot I$. Substituting the second equation into the first for $U$ gives:

$\begin{split} P &= R \cdot I \cdot I\\ P &= I^2 \cdot R.\end{split}$

We solve for $I^2$ by dividing both sides by R: 

$\begin{align*} P &= I^2 \cdot R &\quad\quad\quad &|~:~R\\ I^2 &= \frac{P}{R}.\end{align*}$

In the last step we then take the square root:

$\begin{align*} I^2 &= \frac{P}{R} &\quad\quad\quad &|~\sqrt{~~}\\ I &= \sqrt{\frac{P}{R}}\end{align*}$

[question:EB505]

If the power $P$ and the current $I$ or the voltage $U$ are known, the resistance $R$ can always be calculated from them as well.

We already know:

$P=\frac{U^2}{R}$

We solve for R by multiplying both sides of the equation by R and then dividing by P:

$R = \frac{U^2}{P}$

On the other hand, $P = I^2 \cdot R$. We divide both sides by $I^2$ and obtain the expression we are looking for:

$R = \frac{P}{I^2}$

[question:EB506]

All the relationships between power, current and voltage presented above for DC also apply to alternating current. However, the RMS values of current and voltage must be used. In an earlier chapter we already learnt how to calculate the RMS value from the peak value: 

$U_\text{eff} = \frac{\hat{U}}{\sqrt{2}}\text{ or }\hat{U} = U_\text{eff} \cdot \sqrt{2}$

[question:EB503]

This means that, with all the formulas derived above, we can now also work out the following questions from the world of radio frequency – that is, of AC voltage.

%%%%%

[question:EB507]

Here the RMS value is $U_\text{eff} = \qty{100}{\volt}$. The terminating resistor is $\qty{50}{\ohm}$ (pure resistance). What we want is the power in the load.

$P = \frac{U^2}{R} =\frac{(\qty{100}{\volt})^2}{\qty{50}{\ohm}} = \qty{200}{\watt}$

%%%%%

[question:EB508]

The power can also be calculated when the current is known, with the familiar formula $P = I^2 \cdot R$. Substituting:
  
$P = (\qty{2}{\ampere})^2 \cdot \qty{50}{\ohm} = \qty{200}{\watt}$

%%%%%

[question:EB509]

To calculate the power converted in a $\qty{100}{\ohm}$ resistor across which a voltage of $\qty{10}{\volt}$ is dropped, we again use:

$P = \frac{U^2}{R} = \frac{(\qty{10}{\volt})^2}{\qty{100}{\ohm}} = \qty{1}{\watt} $

%%%%%

[question:EB510]

Answering this question takes a little thought. Both a maximum voltage rating ($\qty{700}{\volt}$) and a maximum power ($\qty{1}{\watt}$) are given. The only question is which limit is reached first as we increase the voltage.

First, let us calculate the voltage that must be applied across the resistor ($\qty{10}{\kilo\ohm}$) for the permitted power to be just reached. For this we calculate (derivation above):

$U = \sqrt{P \cdot R} = \sqrt{\qty{1}{\watt} \cdot \qty{10000}{\ohm}} = \qty{100}{\volt}$

And that is already the maximum DC voltage we are looking for!

%%%%%

[question:EB511]

Here the calculation is the same as in the previous question; only the numerical values are different:

$U = \sqrt{P \cdot R} = \sqrt{\qty{6}{\watt} \cdot \qty{10^5}{\ohm}} \approx \qty{774.6}{\volt} \approx \qty{775}{\volt}$

%%%%%

[question:EB512]

When the resistance value and the maximum power rating are given and the maximum current is asked for, we use the relationship:

$I = \sqrt{\frac{P}{R}} =  \sqrt{\frac{\qty{23}{\watt}}{\qty{120}{\ohm}}} \approx \qty{0.4378}{\ampere} \approx \qty{438}{\milli\ampere}$

[question:EB513]

In this question an oscilloscope is used to measure the peak-to-peak voltage across the load. This voltage is $U_\text{SS} = \qty{25}{\volt}$. This means that the peak voltage is $\hat{U} = \qty{12.5}{\volt}$. We first calculate the RMS value of the voltage:

$U_\text{eff} = \frac{\hat{U}}{\sqrt{2}} = \frac{\qty{12.5}{\volt}}{\sqrt{2}} \approx \qty{8.84}{\volt}$

The RMS current is then (Ohm's law):

$I_\text{eff} = \frac{U_\text{eff}}{R} = \frac{\qty{8.84}{\volt}}{\qty{1000}{\ohm}} \approx \qty{8.8}{\milli\ampere}$

From this the RMS power could also be calculated, but the question does not go that far here.

---

[question:EB514]

Finally, the answer to this question is very easy to work out in your head. Here 11 identical resistors are connected in parallel, as shown in Figure [ref:e_dummyload_11]. This means that the current through each individual resistor is $1/11$ of the total current. So the power in each resistor is also only $1/11$ of the total power.

So the permitted total power is $11 \cdot \qty{5}{\watt} =\qty{55}{\watt}$.

<margin>
[picture:1014:e_dummyload_11:Dummy load made of 11 identical resistors]
</margin>