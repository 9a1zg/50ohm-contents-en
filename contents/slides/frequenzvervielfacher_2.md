<left>
[picture:489:a_frequenzvervielfacher_schaltung:Example of a frequency multiplier circuit with a class C amplifier without base bias]
</left>
<right>
* The input signal is fed to a non-linear distorting stage
* E.g. a class C amplifier, by operating it without base bias
* The signal is heavily distorted
* A filter selects the desired harmonic
</right>
<note>
Amplifier circuits come later in the chapter.
</note>
---
<left>
[picture:489:a_frequenzvervielfacher_schaltung:Example of a frequency multiplier circuit with a class C amplifier without base bias]
</left>
<right>
* Only integer multiples are possible
* As a rule, the 2nd or 3rd harmonic is used
* Higher multiplication with stages connected one after the other
</right>
<note>
</note>
---
[question:AF312]
---
[question:AF311]
---
### Screening

* Frequencies are produced at the intermediate stages
* These often lead to interference
* All stages must be well screened

---
[question:AF313]
---
### Several multiplier stages

* The individual frequencies between the multiplier stages can lead to interference
* Trace the path through the individual stages and calculate the individual frequencies
* The order of the stages is important for determining the interference frequencies

---
[question:AF314]
---
#### Solution
* given: $f_\text{Sender} = \qty{432}{\mega\hertz}$
* given: $f_\text{Grund} = \qty{12}{\mega\hertz}$
* given: $f_\text{QRM} = \qty{144}{\mega\hertz}$
* required: sequence of multipliers

<fragment>
$n = \frac{f_\text{Sender}}{f_\text{QRM}} = \frac{\qty{432}{\mega\hertz}}{\qty{144}{\mega\hertz}} = 3$
</fragment>
<fragment>
Only the combination $\textrm{Fundamental frequency}\,\cdot 2\cdot 2\cdot 3\cdot 3$ is possible, since it is the one that triples the frequency in its last step.
</fragment>
---
Check:
$\begin{split}f_\text{Sender} &= f_\text{Grund}\cdot 2\cdot 2\cdot 3\cdot 3\\ &= \qty{12}{\mega\hertz}\cdot 2\cdot 2\cdot 3\cdot 3\\ &= \qty{24}{\mega\hertz}\cdot 2\cdot 3\cdot 3\\ &= \qty{48}{\mega\hertz}\cdot 3\cdot 3\\ &= \bold{\qty{144}{\mega\hertz}}\cdot 3\\ &= \qty{432}{\mega\hertz}\end{split}$
