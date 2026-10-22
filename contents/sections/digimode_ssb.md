Unlike voice transmission, many digital transmission methods (data modes) need only a very small bandwidth. While speech signals in SSB typically occupy a bandwidth of about $\qty{2.4}{\kilo\hertz}$, data modes manage with much narrower frequency ranges. BPSK31, for example, needs a bandwidth of only about $\qty{31.25}{\hertz}$, while FT8 manages with around $\qty{50}{\hertz}$. On HF, the signals produced by data modes are usually also modulated in SSB. The RF bandwidth of the transmitted signal then corresponds exactly to the AF bandwidth of the data mode.

[question:EE402]
[question:EE403]

Within the usual SSB receive bandwidth of about $\qty{2.4}{\kilo\hertz}$, several such narrowband data mode signals can be received at the same time.

<margin>
[picture:718:e_digimode_ssb_empfang_mehrerer_digimodes:Waterfall display of the reception of several data mode signals within the SSB bandwidth of 2.4 kHz. Each column is the transmission of a different signal]
</margin>

[question:EE404]

Purely by calculation, up to 48 FT8 signals ($\frac{\qty{2400}{\hertz}}{\qty{50}{\hertz}}$) or even up to 76 BPSK31 signals ($\frac{\qty{2400}{\hertz}}{\qty{31.25}{\hertz}}$) fit into an SSB bandwidth of $\qty{2.4}{\kilo\hertz}$. On the computer, either a single data mode signal can then be selected specifically or – depending on the software – a large number of these signals can be decoded at the same time. It is precisely this high spectral efficiency that makes narrowband data modes particularly attractive for amateur radio operation.

---

Slow-scan television (SSTV) refers to the transmission of still pictures using digitised picture data. The pictures are transmitted line by line, which allows a comparatively low transmission speed. There are various SSTV methods, which differ in resolution, colour depth and transmission time, among other things. A major advantage of SSTV is the small bandwidth it needs: it is typically below $\qty{3}{\kilo\hertz}$ and so roughly corresponds to the bandwidth of an SSB voice signal. As a result, SSTV can also be used on the HF bands and is particularly suitable for worldwide picture transmission in amateur radio. Figure [ref:e_digimode_ssb_sstv] shows a typical SSTV picture.

In contrast to this is amateur television (ATV), in which moving pictures – that is, real television – are transmitted. Because of the much greater amount of information, ATV needs a much larger bandwidth, typically several megahertz, often $\qty{6}{\mega\hertz}$ or more. For this reason ATV is not feasible on the HF bands and is used only in higher frequency ranges, mostly from the $\qty{70}{\centi\meter}$ band upwards or, for example, in the $\unit{\giga\hertz}$ range via QO-100. Frequency ranges wide enough to provide the bandwidth needed for transmitting moving pictures are available there.

[question:EE415]

<margin>
[photo:84:e_digimode_ssb_sstv:Confirmation of an SSTV contact, sent to F1BIB by ON1GA, with RST 575 and the picture as originally received]
</margin>
