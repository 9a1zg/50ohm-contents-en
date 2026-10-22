Oscillators are among the most important circuit elements in amateur radio. They are, so to speak, the heart of every radio. Oscillators are used to generate RF oscillations in transmitters and receivers. There are various ways of implementing oscillators technically.

---

<margin>
[include:applet_schwingkreis]
</margin>

The simplest form of oscillator is the so-called *LC oscillator*, whose frequency-determining elements form a tuned circuit (consisting of an inductor and a capacitor), as met in the previous chapter.

[question:ED501]

LC oscillators have the disadvantage that their frequency-determining components (L and C) can change considerably with temperature, which can lead to large frequency errors.

According to the formula sheet, the formula for the frequency of oscillation (Thomson's formula) is:

$ f_0 = \frac{1}{2\pi \sqrt{L\cdot C}} $

The frequency of an LC oscillator changes when the value of the capacitor or the inductor changes, e.g. because of the effect of temperature. How this affects the frequency can be seen from the formula:
If the capacitance of the capacitor or the inductance of the inductor *rises*, the frequency of the tuned circuit *falls*. Conversely, the frequency of the tuned circuit *rises* if the capacitance or inductance *falls*.

[question:ED503]
[question:ED505]
[question:ED502]
[question:ED504]

How quickly the temperature changes also determines how quickly the frequency of an oscillator changes. The frequency does not change abruptly, however, since thermal effects always have a certain inertia. The frequency of an oscillator that is subject to fluctuating temperatures therefore usually changes slowly in one direction or the other.

[question:EF304]

A type of oscillator with much better frequency stability is the *crystal oscillator*. Here the frequency-determining component is a crystal, whose resonant frequency depends only very slightly on its temperature (compared with LC oscillators).

[question:ED506]
[question:ED507]

To avoid unwanted radiation, oscillators and buffer stages should always be screened as well as possible. This can be done, for example, by fitting the oscillator in an earthed metal case.

[question:EF207]