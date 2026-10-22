<margin>
[picture:542:n_digital_voice_repeaternetwork:Repeater network for digital voice: repeater DB0FZ with internet connection, hotspot DN9YI and repeater DB0HOB with a radio link to DB0FZ]
</margin>

Speech can also be transmitted digitally, e.g. with the transmission methods DMR, D-Star, C4FM and M17. Depending on the method, this can be done with a computer or with a radio suitable for it. This makes it possible to communicate with radio amateurs all over the world via networked VHF or UHF repeaters. When two or more repeaters are networked, transmissions received by one of the stations can be forwarded over a network, e.g. HAMNET or the internet, and radiated again by other connected stations. To get access to such a repeater network, you can also run what is known as a hotspot at home. Unless there is an appropriate authorisation for a remotely controlled station, a hotspot may only be operated as an attended station, i.e. the transmitter must be switched off when it is not being supervised on site. On HF, digital voice contacts are mainly made direct, for example with FreeDV.

<webmargin>
| l: Abbreviation | X: Transmission method |
| D-STAR | Digital Smart Technologies for Amateur Radio |
| C4FM | Continuous 4-level frequency modulation |
| DMR | Digital Mobile Radio |
| M17 | Open-source transmission method |
[table:n_dv_uebertragungsverfahren:Commonly used transmission methods for digital voice]
</webmargin>

[question:NE404]

---

With digital voice transmission, the speech signals are converted into a data stream before transmission. Several such data streams can also be transmitted in a rapidly alternating, periodic sequence. This is called TDMA (time-division multiple access). In this way two or more voice contacts use the same frequency practically simultaneously. For a radio, this means that while the PTT button is pressed it has to keep switching rapidly between transmit and receive, so that it does not lose the timing. 

<margin>
[picture:474:n_digital_voice_tdma:TDMA with three contacts on one frequency]
</margin>

<tip>
Most external power amplifiers cannot switch between transmit and receive as quickly as TDMA would require. For DMR and other methods that use time slots, therefore, only power amplifiers suitable for this may be used. Otherwise the frequency is occupied not only during your own time slot. This can interfere with the transmissions of other stations on the same frequency.
</tip>

[question:NE403]

---

Unlike analogue transmissions, where usually only the frequency and the mode have to be known in order to make contact with another station, digital voice often involves more settings, for example the talkgroup, the room or reflector for linking repeaters, or the TDMA time slot to be used.

<indepth>
Depending on the method, there can also be many other settings, for example with DMR the colour code, which allows several user groups to share one frequency without hearing each other. Such parameters must be set correctly on the radio before a contact begins, so that the contact can be made.
</indepth>

[question:NE402]

On VHF/UHF handheld transceivers and via repeaters, the digital methods DMR, D-Star or C4FM are often used as well as FM voice.

[question:NE307]

% TODO: Auf die Tabelle wird nicht eingegangen und sie ist nicht komplett ... 
%<webmargin>
%| l: Verfahren | l: Eigene Kennung | l: Gruppenruf | l: Direktruf | X: Sonstige |
%| M17 | Rufzeichen | - | Rufzeichen | Channel Access Number (CAN), Übertragungsrate (1600 oder 3200 Bit/s) |
%| FreeDV | - | - | - | Mode (1600, 700C, 700D, 700E, 2020) |
%| DMR | DMR-ID | Talkgroup | DMR-ID | Color-Code (1 bis 4, im Amateurfunk meist 1), Zeitschlitz (TS 1 oder TS 2) |
%| C4FM | Rufzeichen | Reflektor | - | |
%| D-Star | Rufzeichen | ? | ? | |
%[table:n_digital_voice_verfahren:Verfahren für Digital Voice und mögliche Einstellungen]
%</webmargin>

<latexonly>
\newpage
</latexonly>