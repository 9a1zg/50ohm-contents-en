<left>
[picture:807:spiegelfrequenzen_mischen1:Mixing with receive frequency $f_\text{e}$, oscillator frequency $f_\text{o}$ and the intermediate frequency $f_\text{ZF}$]

$f_\text{ZF} = \left|f_\text{e} \pm f_\text{o}\right|$
</left>
<right>  
The mixing process to $f_\text{ZF}$ inherently always selects two receive frequencies
</right>

---
<left>
[picture:806:spiegelfrequenzen_fe1_fe2:Receive frequencies that both lead to the same $f_\text{ZF}$]
</left>
<right>
* Wanted receive frequency $f_\text{e1}\rightarrow$ image frequency $f_\text{e2}$
* Spacing between wanted receive frequency and image frequency $\rightarrow2 \cdot f_\text{ZF}$
</right>
---
<left>
Oscillator oscillates above the receive frequency

$\downarrow$

Image frequency at ${2 \cdot f_\text{ZF}}$ above the receive frequency
</left>
<right>
Oscillator oscillates below the receive frequency

$\downarrow$

Image frequency at ${2 \cdot f_\text{ZF}}$ below the receive frequency
</right>

---

$f_\text{S} = 2 \cdot f_\text{OSZ}\,-\,f_\text{E} =$
$ \begin{cases}f_\text{OSZ}\,+\,f_\text{ZF} = f_\text{E}\,+\,2 \cdot f_\text{ZF} &\text{if } f_\text{E} \lt f_\text{OSZ} \\ f_\text{OSZ}\,-\,f_\text{ZF} = f_\text{E}\,-\,2 \cdot f_\text{ZF} &\text{if } f_\text{E} \gt f_\text{OSZ} \end{cases}$

---
## Image rejection

<left>
[picture:808:spiegelfrequenzen_mischen2:Additional band-pass filter for image rejection]
</left>
<right>
* Without suppression, the image frequency can cause interference to reception
* Prevention: the wanted frequency is selected by a band-pass filter
* The image frequency is suppressed as much as possible
</right>
---
Measure for the highest possible rejection:
* Choose a high IF, so that the spacing between the wanted receive frequency and the image frequency is as large as possible
* With a large spacing, a high-quality band-pass filter is easier to realise

---
[question:AF201]
---
[question:AF202]
---
#### Solution
* given: $f_\text{OSZ} = \qty{134.9}{\mega\hertz}$
* given: $f_\text{E} = \qty{145.6}{\mega\hertz}$
* required: $f_\text{S}$

<fragment>
$\begin{split}f_\text{S} &= 2 \cdot f_\text{OSZ} - f_\text{E}\\ &= 2 \cdot \qty{134.9}{\mega\hertz} - \qty{145.6}{\mega\hertz}\\ &= \qty{124.2}{\mega\hertz}\end{split}$
</fragment>
---
[question:AF203]
---
#### Solution
* given: $f_\text{OSZ} = \qty{39}{\mega\hertz}$
* given: $f_\text{E} = \qty{28.3}{\mega\hertz}$
* required: $f_\text{S}$

<fragment>
$\begin{split}f_\text{S} &= 2 \cdot f_\text{OSZ} - f_\text{E}\\ &= 2 \cdot \qty{39}{\mega\hertz} - \qty{28.3}{\mega\hertz}\\ &= \qty{49.7}{\mega\hertz}\end{split}$
</fragment>
---
[question:AF204]
---
[question:AF106]
---
[question:AF107]
---
#### Solution
* given: $f_\text{OSZ} = \qty{24.94}{\mega\hertz}$
* given: $f_\text{E} = \qty{14.24}{\mega\hertz}$
* required: $f_\text{S}$

<fragment>
$\begin{split}f_\text{S} &= 2 \cdot f_\text{OSZ} - f_\text{E}\\ &= 2 \cdot \qty{24.94}{\mega\hertz} - \qty{14.24}{\mega\hertz}\\ &= \qty{35.64}{\mega\hertz}\end{split}$
</fragment>
---
[question:AF108]
---
#### Solution
* given: $f_\text{ZF} = \qty{10.7}{\mega\hertz}$
* given: $f_\text{E} = \qty{28.5}{\mega\hertz}$
* required: $f_\text{S}$

<fragment>
For $f_\text{E} < f_\text{OSZ}$:
$\begin{split}f_\text{S} &= f_\text{E} + 2 \cdot f_\text{ZF}\\ &= \qty{28.5}{\mega\hertz} + 2 \cdot \qty{10.7}{\mega\hertz}\\ &= \qty{49.9}{\mega\hertz}\end{split}$
</fragment>
---
[question:AF109]
---
[question:AF110]
---
[question:AF111]
