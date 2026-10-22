The third passive component in radio engineering – after the resistor and the capacitor – is the *inductor*. Various types of inductor and their circuit symbols are shown in Figures [ref:e_spulen] and [ref:e_schaltsymbole_spulen]. As we have already learnt in the chapter on the magnetic field, a magnetic field is produced in a coil as soon as an electric current flows through it. The simplest type of inductor is the so-called straight *solenoid*, or cylindrical coil, as shown in Figure [ref:e_spule_Aufbau].

<margin>
[photo:207:e_spulen:Various types of inductor]
[picture:942:e_schaltsymbole_spulen:Circuit symbols for different types of inductor]
[picture:948:e_spule_Aufbau:Construction of an inductor]
</margin>

---

A solenoid has a so-called inductance $L$, which is calculated with the following formula:

$L = \frac{\mu_0 \cdot \mu_r \cdot N^2 \cdot A_S}{l}$

Looking at how an inductor is built, we therefore find the following quantities:
1. $\mu_0$ is the magnetic constant, a constant of nature with the value $\qty{1.2566e-6}{\henry\per\meter}$. The value can always be looked up on the formula sheet.
2. $\mu_r$ is a material constant, because the core of the inductor can be made of a special material that can strengthen magnetic fields.
3. The number $N$ of turns of enamelled copper wire or silver-plated copper wire.
4. $A_S$ is the cross-sectional area of the core.
5. The length $l$ of the coil

[question:EA102]

<indepth>
The symbol $L$ was chosen in honour of Professor Emil Lenz (1804–1864) of St Petersburg, who formulated the law named after him, Lenz's law.
</indepth>

<unit>
An inductor has the inductance $L$ with the unit $\qty{1}{\volt\second\per\ampere}$, which is usually given in *henries* ($\unit{\henry}$). The unit is named after the American physicist *Joseph Henry* (1797–1878). An inductance of $\qty{1}{\henry}$ is present when a change in current of $\qty{1}{\ampere}$ within one second produces a self-induced voltage of $\qty{1}{\volt}$. In practice, inductances are usually much smaller and are typically given in $\unit{\milli\henry}$, $\unit{\micro\henry}$ or $\unit{\nano\henry}$.
</unit>

---

With the help of the formula and the following qualitative relationships, a number of examination questions can already be solved:

1. The inductance rises with the square of the number of turns. If the number of turns is doubled, the inductance rises to four times its value.
2. If the coil is compressed, the inductance $L$ rises.
3. If the cross-sectional area is increased, the inductance $L$ rises.
4. If the magnetic field in the coil is strengthened by a suitable material that conducts magnetic flux well (e.g. iron), the inductance $L$ rises.

[question:EC305]

If the coil is compressed, $l$ becomes smaller. As a result, the inductance $L$ rises.

[question:EC306]

If the length $l$ of the coil is doubled, the inductance $L$ must halve.

[question:EC307]

If the number of turns $N$ is doubled, the inductance $L$ increases fourfold.

If the number of turns is reduced, the inductance falls, but even with half a turn or a quarter turn, and even with a straight piece of wire, a small parasitic inductance is still present.

[question:EC304]

---

We call a particular class of materials *ferromagnetic*: at the atomic level they contain tiny elementary magnets which line up under the influence of an external magnetic field and so greatly increase the *magnetic flux density* (which we will not deal with at this point, however). Among the pure chemical elements, only iron, cobalt and nickel are ferromagnetic.

<indepth>
$\mu_r$, also called the relative permeability, is very large for ferromagnetic materials (for iron, for example, in the range $300\dots\num{10000}$).
</indepth>


[question:EB204]

If a ferromagnetic material such as iron is inserted into the coil, the magnetic field is strengthened and the inductance rises. 

If, on the other hand, we insert a core of a highly conductive (non-ferromagnetic) metal such as aluminium or copper into a solenoid, the inductance of the coil falls. This is because the radio-frequency magnetic field of the coil produces ("induces") currents in the core, so-called eddy currents. These secondary currents in turn produce magnetic fields that oppose the magnetic field of the coil. That is why the inductance falls. The magnetic field inside the core is reduced in the process. 

The answer regarded as correct in the following question is that the magnetic field cannot penetrate the core and therefore the cross-sectional area of the field is reduced. That is not quite what happens physically, however. Simply remember the "correct" answer. 

[question:EB205]

---

As with the capacitor, let us first look at how the inductor behaves with direct current: the inductor is connected to a DC voltage source through a series resistor, as shown in Figure [ref:e_spule_einschalten]. At the moment of switching on, the rise in current is at first delayed, so that the current does not jump but rises only gradually to its maximum value.

The reason for this is Lenz's law: as the current rises, the inductor produces a self-induced voltage that opposes the change in current – and so opposes its cause. This limits the rise in current. Since no current is flowing at the start, almost the whole applied voltage is at first dropped across the inductor. As the current increases, this induced voltage decreases while the current continues to rise.

Once the steady state is reached, the inductor behaves with direct current approximately like a piece of wire. The voltage dropped across it is then practically zero. How the voltage across the inductor varies with time is shown in Figure [ref:e_spule_einschalten_spannung].

<margin>
[picture:1016:e_spule_einschalten:Circuit for examining an inductor]
</margin>
<margin>
[picture:186:e_spule_einschalten_spannung:Voltage curve on switching on]
</margin>

[question:EC301]

---

At the moment of switching off, the self-induced voltage tries to keep the current flowing. The inductor then acts as a generator whose induced voltage has the opposite polarity to before. In this the inductor behaves exactly the opposite way to the capacitor. These processes can be observed well with an oscilloscope, as in Figure [ref:e_Spulenstrom].

<margin>
[photo:257:e_Spulenstrom:Inductor voltage and inductor current on switching on and off]
</margin>

Inductors can therefore also be used to create a delay. In the following question, the current through lamp 2 rises more slowly than through lamp 1, because it has a coil in series whose self-induced voltage lets the switch-on current rise only slowly.

[question:EC302]

As with the capacitor, an inductor behaves differently when it is connected to a DC voltage or to an AC voltage. In radio engineering it is above all the behaviour with AC voltage that matters. So let us now look at how it behaves with alternating current. 

Like a capacitor, the inductor has an AC resistance $X_{\textrm{L}}$: although the wire of the coil has only a very small ohmic resistance (conductor resistance), the current that flows becomes smaller as the frequency of the AC voltage rises:

$X_{L} = \omega \cdot L = 2\cdot\pi\cdot f \cdot L$

The formula shows that the AC resistance rises as the frequency increases and falls as the frequency decreases.

[question:EC303]
