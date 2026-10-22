The frequency of an oscillator always depends on the ambient temperature, because the properties of the components used change with temperature. In transistors and diodes this affects, for example, the gain, the threshold voltage and the capacitances. Passive components such as capacitors, resistors and in particular crystals also have temperature-dependent electrical properties.

To keep the frequency of an oscillator as stable as possible, it should be thermally insulated as well as possible from other sources of heat and cold in the equipment. This can be done, for example, by keeping it as far as possible from internal and external sources of heat and cold and from air currents. In addition, a crystal oscillator is preferable to an RC oscillator, LC oscillator or VCO, as it has a much higher frequency stability thanks to the high Q of the crystal.

[question:AF215]

There are different types of crystal oscillator, which differ in their frequency stability:

* The simplest crystal oscillator (see Figure [ref:a_xo]) is called an *XO*, short for crystal oscillator.
* A *TCXO* (temperature-compensated crystal oscillator) compensates for the effects of temperature with additional components in the oscillator circuit, so that their temperature-dependent effects largely cancel each other out within the usual operating temperature range.
* An *OCXO* (oven-controlled crystal oscillator) stabilises the temperature of the crystal oscillator with a controlled heater. For this, the oscillator sits in a thermally insulated case that largely protects it from outside heat and cold. Of the oscillator types mentioned, the OCXO offers the highest frequency stability. 

<margin>
[photo:333:a_xo:XO crystal oscillator at $\qty{433.75}{\mega\hertz}$]
[photo:337:a_ocxo:OCXO crystal oscillator at $\qty{10}{\mega\hertz}$]
</margin>

[question:AD602]
[question:AD603]
[question:AD605]

Especially when operating at high frequencies, the frequency stability of the reference oscillator of transceivers, transverters and converters is very important when using transmission modes that are sensitive to frequency errors. To reach the high output or receive frequencies, the frequency of the reference oscillator is multiplied inside the equipment. As a result, frequency errors of the reference oscillator are multiplied in the transmit or receive frequencies, which can lead to large frequency errors and frequency instability (e.g. drift of the transmitted or received signal). For this reason at least a TCXO should be used, for example, on the $\qty{3}{\centi\meter}$ band, i.e. the $\qty{10}{\giga\hertz}$ band.

[question:AD604]