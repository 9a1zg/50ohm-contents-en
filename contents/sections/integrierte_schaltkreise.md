Integrated circuits are complex circuits implemented on a semiconductor substrate. This makes them a great help in building electronic circuits.

[question:AC601]

<margin>
[photo:334:a_ic:TinyWhisper HF transmitter from JKU Linz and JMU Würzburg, implemented as an integrated circuit in 130 nm CMOS technology]
</margin>

A special class of integrated circuits are monolithic microwave integrated circuits (MMICs). They combine both active and passive components on the same substrate. They are typically designed for an input and output impedance of $\qty{50}{\ohm}$. With them, high gain over a wide bandwidth is possible with few components.

[question:AC602]
[question:AC603]
[question:AC604]

---

To work out the examination questions, it helps first to look more closely at the circuit in Figure [ref:a_mmic].

The capacitors $C_1$ and $C_3$ serve as coupling capacitors. They let RF signals pass but block DC voltage. This prevents DC voltages from being passed between the individual stages of the circuit and affecting the operating point.

The choke in the supply line $U_\mathrm{CC}$ prevents RF signals from escaping through the power supply. At radio frequencies the choke has a high impedance and therefore acts as a block. The capacitor $C_2$ serves to decouple the supply voltage for RF. It shunts any remaining RF components to chassis and ensures that the supply voltage stays stable as far as RF is concerned. Together with the choke, it provides RF decoupling of the supply voltage. We will meet this circuit again later as the "bias tee".

A special feature of many MMICs is that the supply voltage is fed in through the output. The resistor $R_\text{BIAS}$ sets the operating point of the MMIC.

<margin>
[picture:773:a_mmic:MMIC circuit]
</margin>

Depending on the question, the voltage drop across the resistor $R_\text{BIAS}$ can first be determined from the voltage drop across the MMIC. With the known resistance, the current through the circuit can then be calculated. The same current also flows through the MMIC, so that, for example, its thermal power dissipation can be determined from it.

The following questions can therefore be solved in much the same way as the circuits with bipolar transistors that we already know.

[question:AF425]
[question:AF426]
[question:AF427]

% Eine wesentliche Erleichterung bei dem Aufbau von elektronischen Schaltung 
% ist die Verwendung von integrierten Schaltungen.
% Eine integrierte Schaltung enthält in einem Gehäuse eine komplexe elektronische Schaltung, 
% die auf einem Chip hergestellt wurde.

% "Zusatzinfo" Praktische Anwendungen:
% Operationsverstärker: siehe Abschnitt ...
% Niederfrequenzverstärker: siehe Abschnitt ...
% Mikrowellenverstärker MMIC: siehe Abschnitt ...
% Kombinierte Mischer- und Oszillatorschaltung: siehe Abschnitt ...
% Komplette Empfänger: siehe Abschnitt ...
% Digitale Schaltkreise: siehe Abschnitt ...
% PLL-Schaltungen: siehe Abschnitt ...

% Durch wenige externe Bauteile kann z.B. ein Audioverstärker, ein Oszillator mit Mischer oder sogar ein kompletter % Kurzwellenempfänger realisiert werden.
% Bild eines IC mit Typenbezeichnung und Blockschaltbild z.B. LM386
% Für Frequenzen ab ca. 100 MHz werden sogenannte Monolithic Microwave Integrated Circuit (MMIC) eingesetzt.
% Bild MMIC MSA 0686 oder ERA 3
% Hierbei handelt es sich um einen Verstärker. der breitbandig den Frequenzbereich von 100 MHz bis 2 GHz um  20dB verstärken kann
% und eingangs- und ausgangsseitug für 50 Ohm Last angepasst ist.
% Es muss lediglich der Strom für den Arbeitspunkt laut Datenblatt eingestellt werden, damit der MMIC auch nicht % thermisch überlastet wird. 
% Dazu ist bei vorgegebener Betriebsspannung ein Widerstand und dessen elektrische Belastung zu berechnen.

% Da der MMIC ein Gehäuse für SMD-Technik besitzt, ist es notwendig, auch die äußere Beschaltung in SMD- Technik auszuführen.
% Der Gesamtaufbau des Verstärkers wird so deutlich kleiner sein als früher in diskreter Schaltungstechnik.
% Bild Vergleich diskrete Schaltung und MMIC



