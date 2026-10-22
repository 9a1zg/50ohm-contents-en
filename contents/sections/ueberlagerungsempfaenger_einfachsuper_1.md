We met the crystal set as the simplest receiver in the previous chapter. The crystal set is a so-called tuned radio frequency (TRF) receiver, which we also met in Class N. In a TRF receiver, as shown in Figure [ref:e_geradeausempfänger], after reception and, where necessary, amplification, the signal is simply demodulated. This receiver concept, however, has the disadvantage of poor selectivity. To improve it, the input filter block (2) could be made up of several filters to increase the selectivity. But then all these filters would have to be adjusted whenever the receive frequency is changed, and that is very complicated. For this reason the *superheterodyne receiver* (see Figure [ref:ueberlagerungsempfaenger_einfachsuper]) was developed, which in technical language is also called the *superheterodyne* or, for short, the *superhet*.

<margin>
[picture:736:e_geradeausempfänger:Tuned radio frequency (TRF) receiver]
</margin>

<margin>
[picture:803:ueberlagerungsempfaenger_einfachsuper:Superhet with amplifiers]
</margin>

---

The idea of the superhet is as simple as it is ingenious. Instead of tunable filters, a variable-frequency oscillator (VFO) is used, with whose help the received signal is first converted to a fixed frequency, the so-called intermediate frequency $f_\mathrm{z}$ (often also called the IF). Very selective, high-quality filters can be made for this fixed intermediate frequency. Figure [ref:ueberlagerungsempfaenger_einfachsuper_filter] illustrates this principle.

<margin>
[picture:913:ueberlagerungsempfaenger_einfachsuper_filter:Superhet with filters]
</margin>

The input filter first lets through only the wanted frequency range, for example the HF range. A mixer then converts the input signal, together with the frequency of the VFO, to the constant intermediate frequency, for example $\qty{455}{\kilo\hertz}$. In this specific example, the VFO can be set between $\qty{3.455}{\mega\hertz}$ and $\qty{30.455}{\mega\hertz}$, so that the entire HF range can be mixed down. The decisive advantage of the superhet over the TRF receiver lies precisely in this constant intermediate frequency: the filtering of the signal can be optimised for one fixed frequency, which achieves a very high selectivity.

---

Since the filters do not have to be tunable, their bandwidth and skirt steepness can be optimised specifically, for instance by using crystal, ceramic or digital filters. For example, filters with a bandwidth of about $\qty{2.4}{\kilo\hertz}$ can be used for voice transmission (SSB), and narrow filters of about $\qty{300}{\hertz}$ for telegraphy (CW). Suitably adapted filters can also be used for other modes such as AM, FM or digital modes.

With this concept the superhet achieves considerably better selectivity than the TRF receiver. A further advantage is that all the following modules always work at the same intermediate frequency and therefore do not have to be tunable either, which simplifies the construction and improves the reception quality.

[question:EF102]

Superhets can work with one or more intermediate frequencies. In the simplest case it is a direct-conversion receiver, in which the intermediate frequency is the wanted audio frequency. For this, the oscillator frequency must be very close to the receive frequency.

[question:EF208]

A superhet does, however, also have some disadvantages, in particular the occurrence of so-called image frequencies. We will deal with this problem, and with more advanced receiver concepts such as the multiple-conversion superhet with several intermediate frequencies, in more detail only in Class A.

<indepth>
The inventor of the superhet cannot be named unambiguously. One reason for this is that it was developed during the First World War, when all the warring parties were working intensively on improving radio and wireless technology. Around the year 1918, several researchers were working on this principle independently of one another, among them Edwin Armstrong in the USA, Lucien Lévy in France and Walter Schottky in Germany.
  
The term heterodyne, or superheterodyne, is a coinage. It is made up of the Latin super ("above") and the Greek words hetero ("different") and dynamis ("power" or "effect"). The name describes the basic operating principle of the superhet: mixing two signals of different frequencies to produce a new frequency.
</indepth>