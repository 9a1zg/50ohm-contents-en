In Class E we have already met AGC (automatic gain control). With strong input signals, the AGC reduces the gain of amplifier stages in the receive path, and with weak input signals it increases it accordingly. This keeps the amplitude of the demodulated signal, and thus the volume of the AF signal, constant.

Without AGC, strong signals would overdrive the AF stages and weak signals would be only very faintly audible in the AF. The AF volume would constantly have to be readjusted by hand. The AGC thus evens out the dynamic range of the received signal and dynamically adapts the sensitivity of the receive path to the RF input signals.

[question:AF224]

<margin>
[picture:1055:e_agc:AGC in a superhet]
</margin>

---

For the AGC to be able to adapt the gain automatically to the strength of the received signal, it needs information about the signal's amplitude. For this, part of the IF signal can be rectified and then smoothed, as shown in Figure [ref:e_agc_regelspannung].

The diode rectifies the high-frequency IF signal. A following RC network suppresses the fast AC components, so that a DC voltage is produced whose level depends on the amplitude of the IF signal. The stronger the received signal, the greater the magnitude of this voltage. 

This *AGC voltage* is fed back to the controllable RF or IF amplifier stages, where it is used to control their gain. In this way a closed control loop is formed: a stronger received signal leads to a stronger control action and thus to lower gain.

<margin>
[picture:142:e_agc_regelspannung:AGC voltage]
</margin>

[question:AD503]
