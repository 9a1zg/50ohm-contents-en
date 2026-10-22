When an analogue signal is digitised, two properties have to be considered: at what moments is the signal measured, and how precisely can the measured values be represented? The two corresponding steps are called *sampling* and *quantisation*.

The terms *continuous-time*, *discrete-time*, *continuous-value* and *discrete-value* describe two properties of a signal that are independent of each other. On the one hand, you can consider whether the signal is defined at every moment in time. On the other hand, you can consider whether it can take any value.

An ideal analogue signal is both *continuous-time* and *continuous-value*. It is defined at every moment in time and can take any intermediate value within its range of values. Figure [ref:a_wertkont_zeitkont] shows such a signal.

---

Analogue signals have no smallest time resolution and run on continuously in time. They are therefore called *continuous-time*. In sampling, by contrast, such a signal is measured, that is, sampled, only at particular moments. The individual sampled values are called *samples*.

Each sample represents only the instantaneous state of the signal at the moment of sampling. Between two sampling instants the analogue signal can go on changing. Since after sampling there are only individual values, separated from one another in time, the sampled signal is called *discrete-time*.

Figure [ref:a_wertkont_zeitdisk] shows such an ideally sampled signal. It is *discrete-time*, since values exist only at particular sampling instants. At first, however, the individual samples can still take any value and are therefore *continuous-value*.

<margin>
[picture:408:a_wertkont_zeitkont:Continuous-value and continuous-time signal]
[picture:409:a_wertkont_zeitdisk:Continuous-value and discrete-time signal]
</margin>

[question:AF601]
[question:AF603]

The process in which a continuous-time signal is sampled at particular moments and so turned into a discrete-time signal is called *sampling*.

[question:AF606]

The speed at which an analogue signal is sampled is called the *sampling rate* or *sample rate*. It states how many samples are taken per unit of time, for example per second.

On digital storage media such as CDs, for example, analogue audio signals are sampled at a sampling rate of $\num{44100}$ samples per second (unit $\unit{\sps}$), or $\qty{44.1}{\kilo\sps}$ for short.

[question:AF615]

---

Besides the time resolution, the resolution of the measured values also plays a part in digitisation. Analogue signals can take any voltage value and vary between these values without fixed intermediate steps. They are therefore called *continuous-value*.

In digitisation, by contrast, only a limited number of possible numerical values is available. A measured voltage value must therefore be assigned to one of these fixed levels. The signal is then *discrete-value*.

If an analogue signal value lies between two possible levels, a decision has to be made as to which level the measured value is assigned to. This process is called *quantisation*. The signal, which was previously continuous-value, is mapped onto a finite number of possible values.

[question:AF605]

To illustrate this, Figure [ref:a_wertdisk_zeitkont] shows a *discrete-value but continuous-time signal*. The signal is still defined at every moment, but can take only certain fixed, predefined values. So the possible values are already quantised, but time has not yet been made discrete.

When sampling and quantisation are combined, the result is a *discrete-value and discrete-time signal*, as shown in Figure [ref:a_wertdisk_zeitdisk]. Samples exist only at particular moments, and their possible values, too, are restricted to fixed levels. This corresponds to the digital representation of a signal that was previously analogue.

<tip>
To illustrate this, you can compare an analogue dimmer with a step switch. With an analogue dimmer the brightness of a lamp can be set as finely as you like. With a step switch with, for example, $\num{5}$ steps, on the other hand, only $\num{5}$ different brightness values are available. Intermediate values are not possible.

If a brightness set with the analogue dimmer is to be reproduced with the step switch, the step that fits best has to be chosen. This is exactly the principle of quantisation: a continuous value is assigned to one of several fixed, predefined values.
</tip>

<margin>
[picture:410:a_wertdisk_zeitkont:Discrete-value and continuous-time signal]
[picture:411:a_wertdisk_zeitdisk:Discrete-value and discrete-time signal]
</margin>

[question:AF602]
[question:AF604]

<indepth>
Here you have the chance to try the whole thing out again. A continuous-time sine signal is digitised by an A/D converter and then turned back by a D/A converter into an analogue signal that is continuous-time but still discrete-value. The sliders let you set the time quantisation and the value quantisation of the A/D and D/A converters.

[include:quantisierung_und_sampling]
</indepth>