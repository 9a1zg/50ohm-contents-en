### Why I/Q?

* Symbols can differ in amplitude, frequency or phase.
* For amplitude and phase, a clear representation is needed.
* This representation is called the *I/Q representation*.
* It shows the signal state of a symbol as a point in a plane.

--- style="font-size: 0.7em;"

<left>
[include:applet_iq_zeiger]
</left>
<right>
### Symbol as a phasor

* Length of the phasor: amplitude $A$
* Angle of the phasor: phase $\varphi$

* The phasor can be split into two components:

$I=A\cdot\cos(\varphi)$

$Q=A\cdot\cos(\varphi-\qty{90}{\degree})=A\cdot\sin(\varphi)$

* The constellation diagram shows the initial state of the phasor for each symbol.
</right>


---

[question:AF633]

---

### Constellation diagram

[picture:1060:a_konstellationsdiagramm:Constellation diagram]

---

### Constellation diagram

* To represent the symbols, we do not look at the continuous rotation of the carrier.
* Instead, we look at the signal state that belongs to a symbol.
* Each possible symbol state is shown as a point in the I/Q plane.
* Distance from the origin: amplitude
* Angle to the I axis: phase

---

### Why do we need this?

* Constellation diagrams show at a glance the possible symbols of a digital transmission method.
* You can see whether the symbols differ in amplitude, in phase or in both.
* In the next sections we use this representation for mapping, PSK and QAM.