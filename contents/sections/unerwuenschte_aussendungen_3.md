In Class E we have already met unwanted emissions in the form of *harmonics* and *spurious emissions*. Overtones, or harmonics, of a signal always arise when there are departures from the ideal sine curve, and they are always integer multiples of the fundamental frequency, as shown in Figure [ref:a_harmonische].

The following examination question gives an example: if an amplifier is overdriven, the peaks of the amplitude of the sine signal are limited – and this produces harmonics.

[question:AJ207]

<margin>
[picture:868:a_harmonische: Overtones (OW), harmonics (Harm.) and spurious emissions (NA)]
</margin>

---

When looking at multiples of the fundamental frequency of a signal, we distinguish between the *harmonics and overtones* of the signal. The two terms differ only in their definition and in the way they are counted. The 1st harmonic of a signal is its fundamental frequency itself. The 2nd harmonic corresponds to the 1st overtone of a signal, the 3rd harmonic to the 2nd overtone of a signal, and so on. Table [ref:a_harmonische] alongside shows the relationship. 

<margin>
| l: Multiple of the fundamental frequency | l: Harmonic | l: Overtone |
| $f_0$ | 1 | ~ |
| $2 \cdot f_0$ | 2 | 1 |
| $3 \cdot f_0$ | 3 | 2 |
| $4 \cdot f_0$ | 4 | 3 |
[table:a_harmonische:Harmonics and overtones]
</margin>

---
  
[question:AJ203]
[question:AJ204]

<tip>
VHF FM broadcasting is the "classic" radio broadcasting on very high frequencies (VHF). Radio programmes are broadcast in the frequency range from $\qtyrange{87.6}{107.9}{\mega\hertz}$.
</tip>

If particular overtones or harmonics of a signal are to be suppressed individually, this can be done not only with the classic harmonic filter (low-pass) but also with what are called *rejector circuits*. A rejector circuit suppresses exactly one frequency as strongly as possible and lets all other frequencies pass almost unhindered.

[question:AJ210]

---

Under the Amateur Radio Ordinance (Amateurfunkverordnung, AFuV), unwanted emissions must be kept to the lowest possible level. For home-built amateur radio equipment, and for equipment originally sold commercially that has been modified by a radio amateur, [Order 33/2007](https://50ohm.de/vfg33) of the Federal Network Agency (Bundesnetzagentur, BNetzA) sets specific limits. Figure [ref:a_vfg33] shows an extract from this order with the permitted limits for unwanted emissions. 

The limits are usually given in $\unit{\dBc}$ and state by how many decibels an unwanted emission must be attenuated relative to the carrier signal or to the maximum transmitted signal level of the transmitter (PEP). As an alternative to the relative figure in $\unit{\dBc}$, an absolute power limit, for example in $\unit{\dBm}$ or $\unit{\micro\watt}$, may also apply to unwanted emissions. In each case, the higher of the two permitted power values that result from the two limits is the one that counts.

Limits for unwanted emissions also apply to amateur radio equipment sold commercially in the European Union. They are regulated uniformly throughout the EU. Unlike the limits of Order 33/2007, the permitted values here depend in part on the transmit power of the equipment. Figure [ref:a_etsi_vfg] compares the limits for commercially sold equipment with the requirements of Order 33/2007.

An example makes the difference clear: for a commercially sold handheld with a transmit power of $\qty{5}{\watt}$, a limit of $\qty{-50}{\dBc}$ applies in the frequency range shown. If, on the other hand, a corresponding $\qty{5}{\watt}$ set for the 2 m or 70 cm band is home-built, a limit of $\qty{-60}{\dBc}$ must be met under Order 33/2007.

At a transmit power of $\qty{750}{\watt}$, this limit remains at $\qty{-60}{\dBc}$ for the home-built set. For a commercially sold set of the same power, on the other hand, a stricter limit of $\qty{-70}{\dBc}$ applies.

The following examination questions refer to home-built or modified amateur radio equipment, and thus to the limits for unwanted emissions as laid down in Order 33/2007 of the BNetzA.

<margin>
[photo:319:a_vfg33:Extract from Order 33 of 2007.]
[picture:1139:a_etsi_vfg:Comparison of the ETSI standard EN 301783 with Order 33 of 2007. The amateur bands are shaded grey in the background.]
</margin>

---

For the VHF/UHF/SHF range from $\qtyrange{50}{1000}{\mega\hertz}$, spurious emissions and harmonics must be attenuated by at least $\qty{60}{\dB}$ relative to the maximum peak level of the transmitter's transmitted signal (PEP), as long as the power of these signals is above a level of $\qty{0.25}{\micro\watt}$ (see Figure [ref:a_uagw]). 

<margin>
[picture:918:a_uagw:Harmonic attenuation, VHF/UHF/SHF range]
</margin>

[question:AJ225]

---

For the HF range from $\qtyrange{1.7}{35}{\mega\hertz}$, spurious emissions and harmonics must be attenuated by at least $\qty{40}{\dB}$ relative to the maximum peak level of the transmitter's transmitted signal (PEP), as long as the power of these signals is above a level of $\qty{0.25}{\micro\watt}$ (see Figure [ref:a_uagw2]).

<margin>
[picture:1140:a_uagw2:Harmonic attenuation, HF range]
</margin>

[question:AJ224]

%TODO BILD VON DL1COM EINBAUEN
A spectrum analyser in *Spurious Emissions* mode can be used to measure the harmonics, as shown in Figure [ref:a_uagw]. The spectrum analyser automatically records the level of the carrier and the suppression of the harmonics, and also shows these on the screen. If you build equipment yourself, it is essential to make sure by measurement that the prescribed limits are met. A commercial manufacturer of radios does confirm compliance with these limits with the CE declaration, but it still happens that individual sets do not meet the requirements – in such cases the BNetzA can prohibit their operation and sale.

Unwanted emissions arise not only from harmonics; they can also occur in the frequency generation of transmitters – for example from unwanted mixing products, from fluctuations in the supply voltage or from overdriving of the AF signal. We will look at this a little more closely below. 

To suppress unwanted mixing products – but also harmonics – a band-pass filter is often used after mixers. Particularly in single-band transmitters and in equipment for the VHF, UHF and SHF ranges, band-pass filters are used instead of classic low-pass harmonic filters. In these radios, signal components often have to be suppressed that already arise within the processing of the transmitted signal and may even lie below the actual transmit frequency.

[question:AJ211]
[question:AJ209]
[question:AJ208]

Unwanted emissions can also be present in the immediate vicinity of the transmitted signal. They are difficult or impossible to suppress with filters and should therefore be suppressed effectively by appropriate measures right at the start of the signal processing. Such *spurious emissions*, also called *spurious products* (and informally also known as "splatter"), which unintentionally widen the transmitted signal, often arise from setting the microphone amplifier of a transmitter too high. This distorts the AF signal, which results in unwanted spurious emissions. Figure [ref:a_harmonische] shows the spurious emissions. 

[question:AJ219]

Unwanted emissions can also arise from an inadequately stabilised supply voltage to transmitter output stages. For example, a poorly filtered or poorly stabilised power supply (with a ripple voltage on its output) can, on the supply-voltage side, lead to AM emissions from the output stage. AF signals coupled in on the mains supply side of a transmitter can also lead to corresponding AM emissions. With CW emissions this can often be noticed as a "buzzing" carrier or tone, especially with older transmitters.

[question:AJ222]
[question:AJ223]