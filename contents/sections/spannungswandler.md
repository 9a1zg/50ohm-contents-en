A voltage converter is needed whenever one electric voltage is to be converted into another. In amateur radio this might be, for example, producing $\qty{5}{\volt}$ for a microcontroller from a $\qty{13.8}{\volt}$ supply, or supplying a laptop with $\qty{19}{\volt}$ from a $\qty{12}{\volt}$ battery. Such circuits are called DC–DC converters. If the voltage is raised, this is a step-up converter (boost converter); if it is lowered, a step-down converter (buck converter).

Every voltage conversion involves losses. The power delivered is therefore always less than the power supplied. The ratio of output power to input power is called the efficiency $\eta$:

$ \eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}} $

For the following questions the power formula $P = U \cdot I$ has to be applied to calculate the input and output power. The efficiency can then be worked out.

[question:AB213]
[question:AB214]

<indepth>
[photo:300:StepUpWandler: Buck-boost (step-down/step-up) converter, here set up as a step-up converter from $\qty{7.2}{\volt}$ to $\qty{24}{\volt}$]
This buck-boost converter can be set to an output of $\qty{0.5}{\volt}$ to $\qty{25}{\volt}$. The maximum power is $\qty{25}{\watt}$. Since the efficiency is very high, the switching transistors need no heatsink.  The step-down mode (buck mode) or the step-up mode (boost mode) can be selected with the small switch on the right.
</indepth>