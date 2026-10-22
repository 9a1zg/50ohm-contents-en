In the lessons for Classes N and E we have already met typical ways in which electronic equipment and installations are affected – for example by direct pick-up into the case or by coupling into leads – together with suitable countermeasures and ways of dealing with them. In Class A these aspects are explored a little further. 

[question:AJ105]

If home-built digital receivers suffer interference to reception, one possible cause may be poor screening of the receiver. Here it makes sense to fit the receiver's printed circuit board into an earthed metal case. Particularly with SDR receivers or home-built designs using SDR technology, good screening is essential to avoid radiated pick-up. Conversely, this also reduces unwanted radiation from these devices.

[question:AJ103]

---

In Class E we have already dealt with coupling into mains leads. There is, however, a further countermeasure that we want to look at more closely below. If interference is conducted in via the mains lead, it makes sense to fit a mains filter in the form of a low-pass filter (see Figure [ref:a_netzfilter] and Figure [ref:a_netzfilter_draw]). These filters are available as ready-made units that comply with the VDE regulations. 

[question:AJ116]
[question:AJ117]
[question:AJ118]

<margin>
[photo:244:a_netzfilter:Mains filter]
[picture:367:a_netzfilter_draw:Circuit of a mains filter]
</margin>

Different transmission methods have different effects on equipment and cables because of their modulation characteristics. The types of modulation CW and SSB in particular (in which the amplitude changes rapidly) often lead to effects in loudspeaker leads, followed by rectification of the RF at the base-emitter paths in the AF section of amplifiers. The base-emitter junction behaves like a diode and rectifies the RF. The AF demodulated in this way becomes audible in the loudspeakers.

[question:AJ107]
[question:AJ106]

To protect DVB-T receivers from strong signals from a VHF/UHF amateur transmitter in the immediate vicinity, a high-pass filter should be fitted in the antenna feed cable of the DVB-T receiver. This is only effective with passive receiving antennas, however. Unselective TV antenna preamplifiers in particular are quickly overloaded by nearby transmitted signals, since they amplify a wide frequency range.
With active receiving antennas, a high-pass filter must be fitted ahead of the antenna's preamplifier.
When fitting filters, the insertion loss of the filters in the passband must also be taken into account. It should be as low as possible, and no more than $\qtyrange{2}{3}{\dB}$, so that the wanted received signal passes as unhindered as possible.

[question:AJ113]
[question:AJ114]
[question:AJ108]

In principle it makes sense to install a low-pass filter with a cut-off frequency of $\qtyrange{30}{40}{\mega\hertz}$ after a high-power HF transmitter. A low-pass effect that effectively suppresses harmonic emissions can also be obtained by using an antenna tuner in a low-pass configuration (pi or LC filter).

[question:AJ112]
[question:AJ104]

Strong transmitted signals from an amateur station can cause interference to reception, noise or dropouts/artefacts/muting (particularly in digital receivers such as DAB/DVB-T) in DAB, TV and VHF FM receivers. This interference is often caused by overloading of the receiver input by high signal strengths at the receiving location, and leads to a reduction in the receiver's sensitivity or to overloading of the receiver's input stage.

[question:AJ110]
[question:AJ111]
[question:AJ109]

To avoid the problems mentioned above, the radio amateur should therefore always work only with the minimum transmit power necessary for satisfactory communication.

[question:AJ101]

Decoupling capacitors are often used to block RF interference in circuits and equipment. They must be able to divert the RF to chassis as efficiently as possible. Ceramic capacitors are particularly well suited to this. Electrolytic and plastic film capacitors are unsuitable, since their wound construction gives them a high self-inductance. With tantalum capacitors, a ceramic capacitor is often connected in parallel because of its better RF bypassing properties, since tantalum capacitors on their own are suitable only for medium radio frequencies up to approx. $\qty{30}{\mega\hertz}$, whereas ceramic capacitors can block far higher frequencies.
To divert RF interference effectively, there must be an effective earth with a low impedance.

[question:AJ119]
[question:AJ102]

RF chokes are often used in the supply lines of RF stages. They present a series impedance to RF and effectively block both RF entering the stages and RF flowing back into the stages' power supply.
Because of their wound construction, these chokes also have self-capacitance, so that together with their inductance they form unwanted resonances (tuned circuits). This can give rise to unwanted *spurious resonances* in the RF stages, caused by the *self-resonances* of the RF chokes. Spurious resonances can adversely affect the characteristics of RF stages. This can lead to unwanted feedback effects, particularly in amplifiers, and to dips in the power response of RF stages.

[question:AJ214]