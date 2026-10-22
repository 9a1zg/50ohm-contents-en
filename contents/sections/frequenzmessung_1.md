Radios sometimes have to be realigned, for example after repairs or when components have changed through ageing. For receivers, alignment includes checking the oscillator frequencies. A frequency counter is normally used for this.

[question:EI501]

Figure [ref:e_frequenzzaehler1] shows the display of a frequency counter. The separate three on the far right stands, as on some pocket calculators, for $\num{10^3}$. So the counter is measuring the frequency $\qty{455}\cdot \qty{10^3}{\hertz}$, or $\qty{455}{\kilo\hertz}$. Newer instruments display the unit prefix directly instead of the power of ten.

<margin>
[photo:187:e_frequenzzaehler1:Display of a frequency counter showing $\qty{455}\cdot \qty{10^3}{\hertz}$]
</margin>

% Ich hab das mal aus Platzgründen entfernt
%<margin> 
%[photo:189:e_frequenzzaehler2:Multimeter, das im Frequenzmessbereich $\qty{455}{\kilo\hertz}$ anzeigt. Darüber erscheinen ein Symbol für niedrige %Batteriespannung, die Luftfeuchtigkeit und die Temperatur. Diese Werte haben nichts mit der Frequenzmessung zu tun.]
%</margin>

<indepth>
The frequency $\qty{455}{\kilo\hertz}$ is common as the intermediate frequency of superhet receivers and can be measured when the receiver is tuned to a strong signal.
</indepth>

---

Alignment instructions often require a frequency to be set to within a certain tolerance, for example $\pm\qty{10}{\hertz}$. In such cases it helps to keep the place value of the individual digits in mind. The power of ten displayed by the instrument, i.e. for $\qty{455}{\kilo\hertz}$ the value $\num{10^3}$ or $\num{1000}$, always applies to the digit directly before the decimal point. The digit to the left of it then stands for $\qty{10}{\kilo\hertz}$ or $\qty{10^4}{\hertz}$, and the digit one further to the left, the four in the example, for $\qty{100}{\kilo\hertz}$ or $\qty{10^5}{\hertz}$. To the right it goes the other way.

 Figure [ref:e_frequenzzaehler_stellen] shows an example with a higher frequency.
  
<margin>
[picture:793:e_frequenzzaehler_stellen:This display shows a frequency in $\unit{\mega\hertz}$. That is also the place value of the digit before the decimal point.]
</margin>

<attention>
Frequency counter inputs can have a high internal resistance. We know this from voltmeters and oscilloscopes. But there are also inputs with $\qty{50}{\ohm}$. These are usually particularly sensitive, and the maximum voltage or power given in the counter's operating manual must never be exceeded.
</attention>

[question:EI502]
[question:EI503]

Frequency counters are built for a particular range of values, for example $\qty{100}{\kilo\hertz}$ to $\qty{2}{\giga\hertz}$. Outside this range they measure inaccurately or not at all. For measuring higher frequencies there are frequency dividers. They divide the frequency of a signal applied to their input by a fixed value and deliver the result as an electrical oscillation at their output. They are also called prescalers, because they are connected between the device under test and the counter.

%TODO Bild Frequenzteiler

Prescalers often divide the frequency by ten. If $\qty{2.4}{\giga\hertz}$ is applied to the input of such a 10:1 divider, the frequency counter after it displays $\qty{240}{\mega\hertz}$.

[question:EI504]