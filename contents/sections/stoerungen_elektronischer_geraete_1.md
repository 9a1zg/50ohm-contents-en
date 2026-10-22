When transmitters are operated – especially high-power transmitters – electronic equipment and installations can be affected in various ways. We have already met such *breakthrough*, and some basic advice on what to do about it, in Class N. The aim is to avoid these effects as far as possible, or to eliminate their causes by suitable countermeasures. In this lesson we want to look more closely at causes and countermeasures. In principle, electronic equipment can be affected in two ways:

- *Radiated pick-up* occurs when RF gets directly into the electronics of a device via the receiving antenna (Figure [ref:e_antenne_einstrahlung]) or because of an inadequately screened case (Figure [ref:e_direkteinstrahlung]) and affects it there.
- *Conducted pick-up* occurs when RF gets into a device via leads or cables, e.g. via the mains lead, antenna feeder, loudspeaker cables etc. (Figure [ref:e_einstroemung])

<margin>
[picture:744:e_antenne_einstrahlung:Radiated pick-up via the receiving antenna]
[picture:746:e_direkteinstrahlung:Direct pick-up into a device]
[picture:747:e_einstroemung:Conducted pick-up via connecting leads]
</margin>

[question:EJ102]
[question:EJ101]

Even when a transmitter is operated in accordance with the law, receivers in the immediate neighbourhood may be affected when receiving other frequencies. High transmit powers of amateur stations and the use of high-gain antennas can produce very high field strengths locally and within the radiation area of the antennas. These can overload receivers and their receiver stages, which can lead to a reduction in receiver sensitivity, up to complete blocking of reception. This can mean, for example, that garage door controls no longer work as usual. LED lights controlled by capacitive sensors are also often affected by transmissions. This is called *overloading* of equipment, or *breakthrough*. 

[question:EJ106]
[question:EJ107]
[question:EJ103]
[question:EJ112]

Breakthrough in the neighbourhood is often associated with the operation of an amateur station. To establish whether there may be a connection with the amateur station's transmissions, evaluating – and, where necessary, keeping – a log of the transmissions made and contacts held is very helpful. This can also, where appropriate, rule out that suspected effects in the neighbourhood are due to the amateur station.

[question:EJ122]

The radio amateur should help the neighbours in a cooperative, solution-oriented way and also make suggestions for a remedy. Problems can often be solved more easily by talking directly than by involving the authorities. Only when all efforts have failed can the competent regional office of the Federal Network Agency (Bundesnetzagentur, BNetzA) be asked to examine the situation. This should, however, really be the last resort for solving the problem.

[question:EJ124]

These efforts include various measures, for example:

%- Reduzierung der Sendeleistung der Amateurfunkanlage % Das sollte das letzte Mittel sein!
- Screening sensitive equipment or leads
- Fitting filters and common-mode chokes on the neighbour's receiving side
- Setting up an effective RF earth
- Using outdoor antennas for reception

We want to look at these measures more closely below.

To avoid breakthrough into equipment, a radio amateur should always use only the *transmit power necessary for satisfactory communication* for transmissions.

[question:EJ104]
[question:EJ105]

If several strong signals are present at the same time in a receiving installation (e.g. from receiving a local TV transmitter and a strong amateur station in the neighbourhood), unwanted harmonics and their mixing products can arise in the receiver through overloading of its receiver stages. This is called *intermodulation*. Intermodulation produces *phantom signals*, which arise only when the signals involved are present.

[question:EJ120]

Even in a switched-off stereo system, strong RF signals can lead to audible noises in the loudspeakers through rectification at non-linear components such as transistors in the AF output stage. Corroded contacts between metals (metal oxides) also have the property that they can form rectifying effects through non-linearities. As a result, when the amateur station transmits, unwanted mixing products can arise on the transmitting or the receiving side, which can lead to breakthrough into television and broadcast reception.

[question:EJ113]
[question:EJ121]


Not all breakthrough can be remedied by measures on the transmitting side. Often the affected equipment itself is not suitable for the place where it is used, does not meet the applicable legal requirements, or its leads and screening are not designed adequately against radiated or conducted RF pick-up. In such cases it makes sense to suggest measures to those affected so that the problems can be remedied.

One possible measure is to screen RF modules with a metal case that is as fully enclosed as possible.

[question:EJ108]

If an HF transmitting antenna is close to and parallel to a $\qty{230}{\volt}$ AC mains cable, RF currents can be coupled into the mains. To keep effects in your own home as small as possible, it is advisable to use a separate RF earth lead for transmitting antennas.

[question:EJ109]
[question:EJ111]

Another possibility is *fitting filters in the leads of equipment* and fitting *common-mode chokes (choking)* to leads.

Filters in particular can be fitted in the receive path on the side of the affected equipment (TV, DVB-T2 receiver, DAB receiver etc.). For example, the field strength of an amateur HF transmitter (e.g. in the range $\qtyrange{3}{30}{\mega\hertz}$) can affect TV reception (e.g. $\qtyrange{470}{690}{\mega\hertz}$). Fitting a high-pass filter can considerably reduce the influence of the amateur radio signal: frequency components outside the TV reception range – in this example, the HF range – are suppressed, so that the receiver stages of the equipment can no longer be overloaded.

[question:EJ116]
[question:EJ117]

The transmitted signal of an amateur station is often coupled into nearby receivers or other equipment suffering interference via the braid of coaxial cables or via leads. If this leads to breakthrough, what is called a *common-mode choke* should be installed on the leads to the affected equipment. A common-mode choke blocks *common-mode currents* on the braid and the inner conductor to the affected equipment. Ferrite toroidal cores or clip-on ferrite cores are typically used as common-mode chokes. Another way of avoiding effects on the control lines of electrical installations and equipment is to use screened control cables (e.g. for door intercoms, telephone lines etc.)

[question:EJ118]
[question:EJ119]
[question:EJ115]
[question:EJ114]

Poor reception conditions at the affected equipment (e.g. an indoor TV antenna for reception) can also make breakthrough into reception more likely. One possible countermeasure would be to use an outdoor antenna, with suitable pre-filters if necessary.

[question:EJ123]