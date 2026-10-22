[picture:810:doppelsuper_blockschaltbild:Block diagram of a double-conversion superhet]

1. RF section with preselection
2. First mixer with VFO
3. First IF amplifier with roofing filter
4. Second mixer with CO

--- data-transition="none"
[picture:810:doppelsuper_blockschaltbild:Block diagram of a double-conversion superhet]

5. Second IF amplifier with filter
6. Third mixer as product detector or demodulator, with BFO where necessary
7. AF amplifier

--- data-transition="none"
[picture:810:doppelsuper_blockschaltbild:Block diagram of a double-conversion superhet]

* Use of two intermediate frequencies
* High 1st IF $\rightarrow$ good image rejection
* Low 2nd IF $\rightarrow$ high selectivity

---
* After the 1st IF there is an input filter ahead of the 2nd mixer
* The image frequency is easy to suppress because of the large spacing
* After the 2nd IF, a filter with a high Q
* Easy to make for low frequencies
* Place the IF and the wanted receive frequency far apart $\rightarrow$ avoids direct reception of the IF
* The 1st IF should be twice the maximum receive frequency

---
[question:AF112]
---
[question:AF113]
---
[question:AF114]
---
### Roofing filter

* After the 1st mixer, a narrow filter (*roofing filter*)
* Tuned to the 1st IF
* Bandwidth at least as large as the largest receive bandwidth required

---
[question:AF116]
---
[question:AF209]
---
[question:AF117]
---
### Oscillator frequencies
* The oscillator frequencies each lie above or below the wanted input frequency
* There are two possible solutions for each mixer

<fragment>
1. $f_\text{OSZ} = f_\text{ZF}\,+\,f_\text{E}$
2. $f_\text{OSZ} = f_\text{ZF}\,-\,f_\text{E}$
</fragment>

---
[question:AF210]
--- style="font-size: smaller;"
#### Solution
* given: $f_\text{E} = 3\dots\qty{30}{\mega\hertz}$
* given: $f_\text{ZF1} = \qty{50}{\mega\hertz}$
* required: $f_\text{OSZ}$

<fragment>
$f_\text{ZF} = |f_\text{E} − f_\text{OSZ}| \Rightarrow f_\text{OSZ} = f_\text{ZF} \pm f_\text{E}$
</fragment>
<fragment>
<left>
Solution 1:
$\begin{split}f_\text{OSZ} &= f_\text{ZF} \, + \, f_\text{E}\\ &= \qty{50}{\mega\hertz} \, + \, 3\dots\qty{30}{\mega\hertz}\\ &= 53\dots\qty{80}{\mega\hertz}\end{split}$
</left>
</fragment>
<fragment>
<right>
Solution 2:
$\begin{split}f_\text{OSZ} &= f_\text{ZF} \, - \, f_\text{E}\\ &= \qty{50}{\mega\hertz} \, - \, 3\dots\qty{30}{\mega\hertz}\\ &= 47\dots\qty{20}{\mega\hertz}\end{split}$
</right>
</fragment>
---
[question:AF120]
--- style="font-size: smaller;"
### Solution
<left>
* given: $f_\text{E} = \qty{3.65}{\mega\hertz}$
* given: $f_\text{ZF1} = \qty{50}{\mega\hertz}$
</left>
<right>
* given: $f_\text{ZF2} = \qty{9}{\mega\hertz}$
* given: $f_\text{NF} = \qty{455}{\kilo\hertz}$
</right>
* required: $f_\text{OSZ}$ for $f_\text{VFO}$, $f_\text{CO1}$, $f_\text{CO2}$

<fragment>
$f_\text{ZF1} = \begin{cases}f_\text{E}\,+\,f_\text{OSZ}\\ f_\text{OSZ}\,-\,f_\text{E}\\ f_\text{E}\,-\,f_\text{OSZ}\end{cases} \Rightarrow f_\text{OSZ} = \begin{cases}f_\text{ZF}\,-\,f_\text{E}\\ f_\text{E}\,+\,f_\text{ZF}\\ f_\text{E}\,-\,f_\text{ZF}\end{cases}$
</fragment>
<fragment>
$f_\text{VFO} = \begin{cases}f_\text{ZF1}\,-\,f_\text{E} = \qty{50}{\mega\hertz}\,-\,\qty{3.65}{\mega\hertz} = \qty{46.35}{\mega\hertz}\\ f_\text{E}\,+\,f_\text{ZF1} = \qty{3.65}{\mega\hertz}\,+\,\qty{50}{\mega\hertz} = \qty{53.64}{\mega\hertz}\\ f_\text{E}\,-\,f_\text{ZF1} = \qty{3.65}{\mega\hertz}\,-\,\qty{50}{\mega\hertz} = \cancel{\qty{-46.35}{\mega\hertz}}\end{cases}$
</fragment>
--- style="font-size: smaller;"‚
<fragment>
$f_\text{CO1} = \begin{cases}f_\text{ZF2}\,-\,f_\text{ZF1} = \qty{9}{\mega\hertz}\,-\,\qty{50}{\mega\hertz} = \cancel{\qty{-41}{\mega\hertz}}\\ f_\text{ZF1}\,+\,f_\text{ZF2} = \qty{50}{\mega\hertz}\,+\,\qty{9}{\mega\hertz} = \qty{59}{\mega\hertz}\\ f_\text{ZF1}\,-\,f_\text{ZF2} = \qty{50}{\mega\hertz}\,-\,\qty{9}{\mega\hertz} = \qty{41}{\mega\hertz}\end{cases}$
</fragment>
<fragment>
$f_\text{CO2} = \begin{cases}f_\text{NF}\,-\,f_\text{ZF2} = \qty{455}{\kilo\hertz}\,-\,\qty{9}{\mega\hertz} = \cancel{\qty{-8.545}{\mega\hertz}}\\ f_\text{ZF2}\,+\,f_\text{NF} = \qty{9}{\mega\hertz}\,+\,\qty{455}{\kilo\hertz} = \qty{9.455}{\mega\hertz}\\ f_\text{ZF2}\,-\,f_\text{NF} = \qty{9}{\mega\hertz}\,-\,\qty{455}{\kilo\hertz} = \qty{8.545}{\mega\hertz}\end{cases}$
</fragment>
<fragment>
VFO: $\bold{\qty{46.35}{\mega\hertz}} \And \qty{53.65}{\mega\hertz}$, CO1: $\bold{\qty{41}{\mega\hertz}} \And \qty{59}{\mega\hertz}$, CO2: $\qty{8.545}{\mega\hertz} \And \bold{\qty{9.455}{\mega\hertz}}$
</fragment>
---
[question:AF118]
--- style="font-size: smaller;"‚
#### Solution
<left>
* given: $f_\text{E} = \qty{21.1}{\mega\hertz}$
* given: $f_\text{ZF1} = \qty{9}{\mega\hertz}$
</left>
<right>
* given: $f_\text{ZF2} = \qty{460}{\kilo\hertz}$
</right>
* required: $f_\text{VFO} \gt f_\text{E}$, $f_\text{CO} \lt f_\text{ZF1}$

<fragment>
$f_\text{ZF} = \begin{cases}f_\text{OSZ}\,-\,f_\text{E}\\ f_\text{E}\,-\,f_\text{OSZ}\end{cases} \Rightarrow f_\text{OSZ} = \begin{cases}f_\text{E}\,+\,f_\text{ZF}\\ f_\text{E}\,-\,f_\text{ZF}\end{cases}$
</fragment>
<fragment>
$f_\text{VFO} = f_\text{E}\,+\,f_\text{ZF1} = \qty{21.1}{\mega\hertz}\,+\,\qty{9}{\mega\hertz} = \qty{30.1}{\mega\hertz}$
</fragment>
<fragment>
$f_\text{CO} = f_\text{ZF1}\,-\,f_\text{ZF2} = \qty{9}{\mega\hertz}\,-\,\qty{460}{\kilo\hertz} = \qty{8.54}{\mega\hertz}$
</fragment>

---
[question:AF119]
--- style="font-size: smaller;"‚
#### Solution
<left>
* given: $f_\text{E} = \qty{28}{\mega\hertz}$
* given: $f_\text{ZF1} = \qty{10.7}{\mega\hertz}$
</left>
<right>
* given: $f_\text{ZF2} = \qty{460}{\kilo\hertz}$
</right>
* required: $f_\text{VFO} \gt f_\text{E}$, $f_\text{CO} \gt f_\text{ZF1}$

<fragment>
$f_\text{ZF} = \begin{cases}f_\text{OSZ}\,-\,f_\text{E}\\ f_\text{E}\,-\,f_\text{OSZ}\end{cases} \Rightarrow f_\text{OSZ} = \begin{cases}f_\text{E}\,+\,f_\text{ZF}\\ f_\text{E}\,-\,f_\text{ZF}\end{cases}$
</fragment>
<fragment>
$f_\text{VFO} = f_\text{E}\,+\,f_\text{ZF1} = \qty{28}{\mega\hertz}\,+\,\qty{10.7}{\mega\hertz} = \qty{38.70}{\mega\hertz}$
</fragment>
<fragment>
$f_\text{CO} = f_\text{ZF1}\,+\,f_\text{ZF2} = \qty{10.7}{\mega\hertz}\,+\,\qty{460}{\kilo\hertz} = \qty{11.16}{\mega\hertz}$
</fragment>
