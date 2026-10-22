A *notch filter* is a very narrowband filter intended to suppress one particular frequency in the AF spectrum of the received signal. This serves, for example, to blank out an interfering carrier in a transmission selectively while leaving the rest of the transmission almost unaffected. Notch filters can be implemented either in the AF section or in the IF section. Filters in the IF section have the advantage that they can suppress stronger interfering signals in particular more effectively and reduce their influence on the AGC.

[question:EF215]

<margin>
[picture:242:frequenzverlauf_notchfilter:Filter response of a notch filter]
</margin>

---

The filter response of a notch filter is designed so that only a small part of the frequency range of the AF signal is suppressed very strongly. This produces a notch in the spectrum – hence the name notch filter.

[question:EF216]

<tip>
Many modern radios implement notch filters using digital filter technology. The bandwidth, the filter response and the frequency can often be set precisely. A further advantage in this context is the so-called automatic notch filter, which can detect steady carrier components in the AF signal and blank them out automatically.
</tip>