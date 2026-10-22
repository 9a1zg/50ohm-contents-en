Besides the well-known lead-acid (Pb) and nickel-metal hydride (NiMH) rechargeable batteries, in radio engineering, e.g. for portable operation, we are increasingly relying on lithium iron phosphate (LiFePO4) batteries. Let us first look at such a battery and its markings in Figure [ref:a_akku_lifepo4].

<margin>
[photo:175:a_akku_lifepo4:LiFePO4]
</margin>

<indepth>
* Capacity: $\qty{4200}{\milli\ampere\hour}$
* Voltage: 4S1P / $\qty{13.2}{\volt}$
% * Entladung: 30C Constant / 40C Burst
% * Balance Stecker: JST-XH
% * Entlastung Stecker: $\qty{5.5}{\milli\meter}$ Kugel-Stecker

The most important ratings for us are the nominal voltage of $\qty{13.2}{\volt}$ and the configuration 4S1P. This means that the nominal voltage of $\qty{13.2}{\volt}$ comes from 4 cells in series and 1 in parallel, i.e. all 4 are connected in series. LiFePO4 cells usually have a nominal cell voltage of $\qty{3.2}{\volt}$ to $\qty{3.3}{\volt}$. This gives $\qty{3.3}{\volt} \cdot 4 = \qty{13.2 }{\volt} \cdot 1 = \qty{13.2}{\volt}$.

A 4S2P battery contains 8 cells in all: 4 in series, with 2 of these strings in parallel. This would then give a voltage of $\qty{13.2}{\volt}$ but a capacity of $\qty{8400}{\milli\ampere\hour}$.

</indepth>

For the example battery, $\qty{4200}{\milli\ampere\hour}$ is given as the rated capacity. The rated capacity $Q$ of a battery is also referred to as its charge and is given in $\unit{\ampere\hour}$ or $\unit{\milli\ampere\hour}$.

For our example battery this corresponds to $\qty{4.2}{\ampere\hour}$. In theory this would mean that we can load our battery with $\qty{4.2}{\ampere}$ for $\qty{1}{\hour}$, or with $\qty{2.1}{\ampere}$ for $\qty{2}{\hour}$, and so on. This is described by the formula:

$t=\frac{Q}{I}$

$t=\frac{\qty{4.2}{\ampere\hour}}{\qty{4.2}{\ampere}} = \qty{1}{\hour}$

[question:AB210]

Now we also want to know how much electrical energy is stored in the battery. The energy ($\unit{\watt\hour}$) is the charge $Q$ ($\unit{\ampere\hour}$) of the battery multiplied by the total voltage $U$ in volts.

$\qty{1}{\watt\hour} = \qty{1}{\ampere\hour} \cdot \qty{1}{\volt}$

For our example we calculate $\qty{4.2}{\ampere\hour} \cdot \qty{13.2}{\volt} = \qty{55.44}{\watt\hour}$ as the stored energy.

[question:AB501]

%Die Entladung dieses Akkus kann mit einem konstanten Entladestrom von "30 C" erfolgen. Das bedeutet, dass der Akku mit 30 $\cdot$ Kapazität $Q$ entladen werden kann.
%
%Endladestrom: $I = 30 \cdot \qty{4200}{\milli\ampere} = \qty{126}{\ampere}$
%
%Das ist allerdings nur ein theoretisch möglicher Wert, da unser Akku somit innerhalb von $\qty{108}{\second}$ entladen wäre. Auch der Kabelquerschnitt ist dabei zu berücksichtigen.
%

When batteries are connected in series, as in Figure [ref:a_akku_4S1P], the voltages add and the capacity stays the same. 
When they are connected in parallel, as in Figure [ref:a_akku_4S2P], the voltage stays the same and the capacities add. 

<margin>
% TODO Bild Reihenschaltung liegt bei DG1HXJ als .tex
[photo:176:a_akku_4S1P:Series connection]
</margin>

<margin>
% TODO Bild Parallelschaltung liegt bei DG1HXJ als .tex
[photo:177:a_akku_4S2P:Parallel connection]
</margin>

<attention>
When using a LiFePO4 battery connected as 4S1P, bear in mind that voltages between $\qty{10}{\volt}$ and $\qty{14.4}{\volt}$ can be present. Not every radio can work with these voltages. It is also important that we only connect together cells/batteries with the same ratings, as the cells affect one another and can otherwise be damaged. With today's lithium batteries in particular, it makes sense to fit a monitoring device (balancer, battery monitor). Among other things, it provides the necessary equalisation of the cell voltages and optimum charging.
</attention>

---


% In der Abb. [ref:a_akku_lifepo4_anschluss]
% TODO Bild Infobox Anschluss Akku liegt bei DG1HXJ als .tex
%<margin>
%[photo:178:a_akku_lifepo4_anschluss:LiFePO4 Anschlüsse]
%</margin>

To answer the following question, you need to know that the total voltage is the sum of the cell voltages. The total charge, on the other hand, is the charge of one cell.

[question:AB209]

For the next question, the usable quantity of charge of $\qty{90}{\percent}$ must first be worked out.
The discharge time $t$ is given by: $t=\frac{Q}{I}$

[question:AB211]
