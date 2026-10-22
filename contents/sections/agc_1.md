*Automatic gain control* *(AGC)* in receivers ensures that the AF output signal (received volume) stays almost constant even when the RF input signal at the receiver fluctuates (e.g. because of fading), and that volume fluctuations are reduced. To do this, the received level is measured at the output of the receive path and the RF gain is controlled accordingly, so that the received volume after demodulation can be influenced in this way. AGC is not to be confused with ALC (automatic level control), which is located in the transmit path.

<margin>
[picture:1055:e_agc:AGC in a superhet]
</margin>

---

Depending on the receiver's features, the AGC can be adjusted with regard to its response (attack time, decay time). Usual names for this are AGC Slow, AGC Normal and AGC Fast, which outline how quickly it responds. The AGC Slow or Normal setting is normally sensible for SSB operation. For telegraphy (CW), the AGC Fast or Normal setting is normally sensible, so that strong signals cannot mask weak signals and the control follows quickly. For digital modes it may be sensible to deactivate the AGC.

[question:EF211]
[question:EF212]

<tip>
On some receivers the AGC can also be deactivated completely. The RF gain can then be controlled, for example manually, by adjusting the RF gain control. However, this is only sensible for special applications (e.g. overloading of the RF input section by strong signals), and possibly for digital modes.
</tip>