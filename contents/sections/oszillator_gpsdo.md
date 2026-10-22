In the previous chapter we saw that there are various types of oscillator with differing frequency stability and accuracy. Crystal oscillators in the form of a TCXO, and above all an OCXO, achieve particularly high stability. Modern radios with a TCXO, for example, achieve a frequency accuracy of $\pm\qty{0.5}{\ppm}$. For a wanted frequency of $\qty{10}{\mega\hertz}$, the actual frequency therefore lies in the range $\qtyrange{9.999995}{10.000005}{\mega\hertz}$, i.e. at most $\pm\qty{5}{\hertz}$ away from the nominal frequency. This error is small and as a rule more than adequate for operation on HF.

If, however, we are working not at $\qty{10}{\mega\hertz}$ but at $\qty{10}{\giga\hertz}$, the possible error increases to $\pm\qty{5000}{\hertz}$. It can then already be larger than the bandwidth of a typical SSB filter. In a contact on a pre-arranged frequency, the signal may therefore lie outside the receive passband. For such applications, e.g. with the geostationary satellite QO-100, which transmits at $\qty{10}{\giga\hertz}$, even more accurate frequency references are therefore needed. 

<margin>
[picture:1081:a_gpsdo:GPS-disciplined oscillator (GPSDO) in a QO-100 station]
</margin>

You could go to great lengths to stabilise an OCXO further, or use other types of oscillator such as rubidium frequency standards, which achieve higher stability than crystal oscillators, especially over longer periods. Such frequency standards, however, often have drawbacks such as higher power consumption, larger dimensions and a higher price, since they are developed mainly for professional applications.

Fortunately there is another possibility: global navigation satellite systems (GNSS) such as GPS or Galileo need very accurate time references. The position of the receiver is determined from the propagation times of signals transmitted to the receiver from several satellites. Since every precise clock needs a stable oscillator as its timebase, we can use the time reference obtained from the satellite signals to stabilise our own TCXO or OCXO. Such an oscillator is called a GPS-disciplined oscillator (GPSDO). How this control works technically is something we will look at in a later chapter on phase-locked loops (PLLs). Figure [ref:a_gpsdo] shows a GPSDO in a QO-100 station, supplying the software-defined radio (SDR) with a stable reference frequency. A home-built module can be seen in Figure [ref:a_gpsdo_homebrew].

---

You might now ask why we do not use the time reference provided by GPS directly as the oscillator signal. From the weak, modulated satellite signals, the GPS receiver usually derives a precise time signal, for example one pulse per second. In the short term, however, the exact timing of this pulse can fluctuate because of noise, multipath propagation, atmospheric effects and delays in the receiver. Viewed over longer periods, on the other hand, the frequency derived from it is very accurate.

A TCXO or OCXO, in turn, has good or very good short-term stability, but in the long term it can slowly drift away from the nominal frequency because of remaining temperature effects and the ageing of its components. A GPSDO therefore combines both properties: the local TCXO or OCXO supplies an output signal that is stable in the short term and low in noise, while a slow control loop corrects its long-term error using the GPS time reference. In this way a GPSDO achieves both very good short-term stability and high long-term stability and frequency accuracy.

[question:AD606]

<margin>
[photo:335:a_gpsdo_homebrew:Home-built GPSDO with a TCXO]
</margin>