## Fundamental and harmonics

* An ideal sinusoidal signal consists only of its fundamental (1st harmonic)
* Departures from the sine shape produce integer multiples of the fundamental frequency
* These multiples are called harmonics

--- style="font-size: smaller;"
### Representation in the frequency spectrum

<left>
[picture:869:zusammenhang_oberwellen_harmonische:Relationship between overtones and harmonics]
</left>
<right>
* 1st harmonic = fundamental frequency
* 2nd harmonic = twice the fundamental frequency
* 3rd harmonic = three times the fundamental frequency
* All harmonics are numbered with an ordinal number (n)
</right>
<note>
Depending on the signal distortion, more even or more odd harmonics are produced.
Square-wave signals (e.g. from overdriving an amplifier) contain mainly odd harmonics.
Sawtooth signals contain mainly even harmonics.
</note>

--- style="font-size: smaller;"
### Overtones – multiples of the fundamental frequency

<left>
[picture:595:a_oberwellen:Signal made up of the fundamental and harmonics]
</left>
<right>
* A signal that is not ideally sinusoidal also contains overtones
* Overtones are integer multiples of the fundamental frequency
* 1st overtone = 2nd harmonic = twice the fundamental frequency
* 2nd overtone = 3rd harmonic = three times the fundamental frequency
</right>

---
[question:AB403]

---
[question:AB401]

---
[question:AB402]

---
## Harmonic analysis with the spectrum analyser

* Even an apparently sinusoidal signal can contain significant harmonics
* Harmonic content is measured with a spectrum analyser
* Display in the frequency domain
* Amplitudes of the harmonics are displayed logarithmically

---
[question:AI615]

---
[question:AI614]

---
## Calculating harmonics and overtones

* Harmonic frequencies = fundamental frequency × ordinal number (n)
* Overtone frequencies = fundamental frequency × (n + 1)

---
[question:AJ201]

---
#### Solution
* given: $f = \qty{3.730}{\mega\hertz}$
* required: $f$ of the 2nd harmonic

<fragment>
$2 \cdot f = 2 \cdot \qty{3.730}{\mega\hertz} = \qty{7.460}{\mega\hertz}$
</fragment>

---
[question:AJ205]

---
#### Solution
* given: $f = \qty{144.690}{\mega\hertz}$
* required: $f$ of the 2nd odd harmonic

<fragment>
2nd odd harmonic = 3rd harmonic
  
$3 \cdot f = 3 \cdot \qty{144.690}{\mega\hertz} = \qty{434.070}{\mega\hertz}$
</fragment>
---
[question:AJ202]

---
#### Solution
* given: $f = \qty{7.050}{\mega\hertz}$
* required: $f$ of the 3rd harmonic

<fragment>
$3 \cdot f = 3 \cdot \qty{7.050}{\mega\hertz} = \qty{21.150}{\mega\hertz}$
</fragment>

---
[question:AJ206]

---
#### Solution
* given: $f = \qty{144.300}{\mega\hertz}$
* required: several harmonics

<fragment>
$\begin{split}2 \cdot \qty{144.300}{\mega\hertz} &= \qty{288.600}{\mega\hertz}\\ 3 \cdot \qty{144.300}{\mega\hertz} &= \bold{\qty{432.900}{\mega\hertz}}\\ &\vdots\\ 9 \cdot \qty{144.300}{\mega\hertz} &= \bold{\qty{1298.700}{\mega\hertz}}\end{split}$
</fragment>
