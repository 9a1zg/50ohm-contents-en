Why do we have a $\qty{230}{\volt}$ AC mains supply? AC voltage has one decisive advantage over DC voltage: it can be converted to other voltages easily and with low losses by means of transformers. This allows the voltage to be adapted efficiently for transmission and use.

Because of self-induction in coils, energy can be transferred with AC voltage between two coils, as shown in Figure [ref:e_netztrafo]. This gives a new component, the *transformer* (in German *Übertrager* or *Transformator*, *Trafo* for short). It consists of two coils that are magnetically coupled through an iron or ferrite core. To tell the two sides apart, we speak of the primary side, with the number of turns $N_P$, and the secondary side, with the number of turns $N_S$.

<margin>
[picture:1017:e_netztrafo:Circuit diagram of a transformer]
</margin>

<margin>
[photo:239:e_Trafo mit getrennten Wicklungen:Transformer with visibly separate windings]
</margin>

A transformer is used to convert a high AC voltage, e.g. $\qty{230}{\volt}$, into a 
lower AC voltage, e.g. $\qty{13.8}{\volt}$. A transformer can only transfer AC voltages. If a DC voltage is wrongly applied to a transformer, it acts like a short circuit because of the low ohmic resistance of the primary winding. The transformer can then overheat badly and, in the worst case, burn out.

---

The transformation ratio of a transformer can be stated as follows:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S}$

The ratio of the numbers of turns is therefore equal to the ratio of the voltages. By rearranging this basic equation, both the voltages $U$ and the numbers of turns $N$ on the primary or secondary side can be calculated.

<indepth>
These relationships apply to the ideal case of an unloaded transformer, the so-called open-circuit case. Open circuit means that no load is connected to the secondary side.
</indepth>

[question:EC401]

We calculate: 

$\begin{align*}ü = \frac{15}{1} = 15 &= \frac{\qty{230}{\volt}}{U_S} &\quad\quad\quad &|~\cdot~U_S\\[1.5ex]15 \cdot U_S &= \qty{230}{\volt} &\quad\quad\quad &|~:~15\\[1.5ex]U_S &= \frac{\qty{230}{\volt}}{15} = \qty{15.33}{\volt}\end{align*}$

[question:EC402]

First we note that $N_P = 5\cdot N_S$ and that $U_P = \qty{230}{\volt}$ is given. Once again the voltage $U_S$ is required.

$ü = \frac{5\cdot N_S}{N_S} = \frac{\qty{230}{\volt}}{U_S}$ 

The $N_S$ cancel out, so all that is left is:

$ü = 5 = \frac{\qty{230}{\volt}}{U_S}$ 

We multiply both sides by $U_S$ and divide both sides by 5.

$U_S = \frac{\qty{230}{\volt}}{5}$ 

In the following question, the number of secondary turns is required. 

[question:EC403]

We are given $N_P=600$, $U_P=\qty{230}{\volt}$ and $U_S=\qty{11.5}{\volt}$. The number of secondary turns $N_S$ is required.

$\frac{600}{N_S} = \frac{\qty{230}{\volt}}{\qty{11.5}{\volt}}$ 

This simplifies to:

$\frac{600}{N_S} = 20$ 

We multiply both sides by $N_S$ and divide both sides by $20$.

$N_S = \frac{600}{20} = 30$

The following transformer steps the output voltage $U_S$ up, so the number of secondary turns must be greater than the number of primary turns.

[question:EC404]

We are given $N_P= 150$, $U_P=\qty{45}{\volt}$ and  $U_S=\qty{180}{\volt}$. $N_S$ is required.

We substitute:

$ \frac{150}{N_S} = \frac{\qty{45}{\volt}}{\qty{180}{\volt}}$

This simplifies to 

$ \frac{150}{N_S} =0.25 $

Again we multiply both sides by $N_S$ and divide both sides by $0.25$.

$ N_S= \frac{150}{0.25} = 600$