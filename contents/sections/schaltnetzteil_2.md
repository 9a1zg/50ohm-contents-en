The switch-mode power supply has already been introduced in Classes N and E. Now we look at the simplified block diagram in more detail.

<margin>
[picture:35:a_schaltnetzteil:Basic circuit diagram of a switch-mode power supply]
</margin>

The important electronic switch in block E also serves to regulate the output to a constant voltage.
Since there are no states between a conducting and a cut-off transistor, there has to be another way of regulating. The transfer of energy from the input side to the load side can be varied by means of the switching time. If the switch stays closed for longer, more energy is transferred to the load side and the output voltage rises. To detect this, the output voltage has to be fed back to the control block of the electronic switch. This feedback is missing from the simplified diagram shown. The output voltage is regulated by what is called the pulse-width modulator. This means that the time for which the switch conducts is varied, while the switching frequency stays constant. 

---

[question:AD311]

Galvanic isolation of the input side from the output side is also important, to keep mains potentials away from the output. This mains isolation is provided by the ferrite-cored transformer. 
See Figure [ref:a_innenansicht_eines_schaltnetzteils]. 

<margin>
[photo:264:a_innenansicht_eines_schaltnetzteils:Inside a switch-mode power supply]
</margin>

---

Varying the switching time produces additional interference signals, which must on no account be allowed to reach the mains side, so that they do not spread through the mains and interfere with other electronic equipment. The mains also acts like an antenna and can therefore radiate interference signals as an electromagnetic wave. If the electronic switch is operated at a switching frequency of $\qty{30}{\kilo\hertz}$, the result is an interference spectrum in which an interference signal appears every $\qty{30}{\kilo\hertz}$. Figure [ref:a_störspektrum] shows the interference spectrum of a switch-mode power supply. The interference spectrum was received directly above the case of the switch-mode power supply. At a distance of $\qty{1}{\meter}$ the interference spectrum can hardly be measured.

[question:AD312]

With switch-mode power supplies that are not adequately suppressed, the interference spectrum impairs radio reception.

[question:AD313]

<margin>
[photo:277:a_störspektrum:Interference spectrum of a switch-mode power supply]
</margin>

---

To prevent interference from getting into the mains, a high-quality low-pass filter must be fitted in the switch-mode power supply on the side connected to the $\qty{230}{\volt}$ AC mains. The typical construction of the filter can be seen in Figure [ref:a-schaltnetzteilfilter].

<margin>
[picture:367:a-schaltnetzteilfilter:Filter at the $\qty{230}{\volt}$ input of a switch-mode power supply]
</margin>

See also the filters in Figures [ref:a_EMV_Filter1] and [ref:a_EMV_Filter2]
*Remember:* the PE conductor must not be connected to the L1 conductor or the N conductor.
The choke T must not act as a transformer for the AC mains voltage.

[question:AD314]


<margin>
EMC filter = radio interference suppression filter against conducted interference
[photo:242:a_EMV_Filter1: Radio interference suppression filter for a switch-mode power supply]
[photo:243:a_EMV_Filter2: Filter directly at the $\qty{230}{\volt}$ AC voltage input]
</margin>