<left>
[photo:299:StepUpDownWandler: Buck-boost (step-down/step-up) converter]
</left>
<right>
* Converts DC voltages $\rightarrow$ DC–DC converter
* e.g. from $\qty{13.8}{\volt}$ to $\qty{5}{\volt}\rightarrow$ step-down (buck converter)
* e.g. from $\qty{12}{\volt}$ to $\qty{19}{\volt}\rightarrow$ step-up (boost converter)
</right>
<note>
The buck-boost converter in the picture can be set to an output of 0.5 V to 25 V. The maximum power is 25 W.
</note>
---
### Efficiency

* The components in the circuit cause losses
* Efficiency $\eta$, usually given in $\%$

<fragment>
$\eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}}$
</fragment>

---
[question:AB213]
---
#### Solution
* given: $U_{\textrm{in}} = \qty{12}{\volt}$
* given: $U_{\textrm{out}} = \qty{5}{\volt}$
* given: $I_{\textrm{in}} = \qty{2}{\ampere}$
* given: $I_{\textrm{out}} = \qty{3}{\ampere}$
* required: $\eta$

<fragment>
$\begin{split} \eta &= \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}} = \frac{U_{\mathrm{out}} \cdot I_{\mathrm{out}}}{U_{\mathrm{in}} \cdot I_{\mathrm{in}}}\\ &= \frac{\qty{5}{\volt} \cdot \qty{3}{\ampere}}{\qty{12}{\volt} \cdot \qty{2}{\ampere}} = \frac{\qty{15}{\watt}}{\qty{24}{\watt}} = \num{0.625} = \qty{62.5}{\percent} \end{split}$
</fragment>
---
[question:AB214]
---
* given: $U_{\mathrm{in}} = \qty{5}{\volt}$
* given: $U_{\mathrm{out}} = \qty{12}{\volt}$
* given: $I_{\mathrm{in}} = \qty{3}{\ampere}$
* given: $I_{\mathrm{out}} = \qty{1}{\ampere}$
* required: $\eta$

<fragment>
$\begin{split} \eta &= \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}} = \frac{U_{\mathrm{out}} \cdot I_{\mathrm{out}}}{U_{\mathrm{in}} \cdot I_{\mathrm{in}}}\\ &= \frac{\qty{12}{\volt} \cdot \qty{1}{\ampere}}{\qty{5}{\volt} \cdot \qty{3}{\ampere}} = \frac{\qty{12}{\watt}}{\qty{15}{\watt}} = \num{0.8} = \qty{80}{\percent} \end{split}$
</fragment>
