Let us now look at the process of sampling in a little more detail and recall the example given earlier of the camera that takes pictures of a scene at particular intervals. Let us assume, for example, that our camera takes 24 pictures per second of a particular scene. If we now imagine, for example, that we are filming a runner running, we will find that between the individual pictures there is always a jerky movement of our runner's legs and body compared with the previous picture. If we run the pictures quickly one after another, the result is a movement that looks continuous. The information that we capture at 24 pictures per second is, however, limited in time (remember: discrete-time). What if a fly were suddenly to fly quickly past the lens of our camera between 2 successive pictures? Would we still be able to see it? That depends on whether the fly chooses the right moment between two pictures for its flight. If it came into the camera's field of view only after a picture had been taken and had already left it again before the next picture was taken, we would not be able to find this event in the pictures we had taken. Information would remain hidden from us.

<webonly>
<margin>
[include:applet_nyquist]
</margin>
</webonly>

It is just the same with sampling analogue signals. If these are captured (sampled) at a particular sampling rate $f_\text{s}$, we may no longer be able to capture fast changes in the signal between 2 samples. Sampling therefore always means a loss of information in time as well. Now we can consider what time resolution is needed to sample an analogue signal of a particular frequency (changes in the signal amplitude per second) without loss of information (all changes are to be captured). We can reason as follows. To be able to capture at least every change in the signal correctly, we must (as in our earlier example with the camera) be able to make sure that a sample is taken at least before and after every change in the signal. In the case of our fly flying through the picture, the condition would be that the fly may fly through the picture only so fast that it can be seen in at least 2 pictures. Otherwise we could not tell from where it flew through the picture and in which direction. If this condition is not met, this information escapes us. In this case we also say that error-free reconstruction is not possible.

It can be shown mathematically that, to capture a signal whose highest frequency is $f_{\mathrm{max}}$, the sampling rate $f_\text{s}$ must be more than twice that, i.e. a little more: $f_\text{s} > 2 \cdot f_{\mathrm{max}}$, so that we can reconstruct our signal correctly again. In digital signal processing this finding is called the sampling theorem and, after its discoverers Nyquist and Shannon, it is also known as the Nyquist–Shannon sampling theorem or the Nyquist condition. The sampling theorem therefore determines the minimum sampling rate $f_\text{s}$ theoretically required to reconstruct a signal without errors.

[question:AF618]

[question:AF616]

---

If the theorem is not satisfied, what are known as aliasing effects occur. 

[question:AF617]

<webonly>
The applet alongside lets you experiment with the sampling rate. If the sampling rate falls below $\qty{2}{\kilo\hertz}$, the Nyquist condition is no longer satisfied and the signal can no longer be reconstructed unambiguously.
It is also interesting that even at a sampling frequency of exactly $\qty{2}{\kilo\hertz}$ the reconstruction does not work reliably. For this reason a sampling rate a little above the Nyquist condition is usually chosen, to ensure that the signal can be reconstructed reliably.
</webonly>

<indepth>
Let us take a practical example, such as a CD player working at a sampling rate of, say, $\qty{44.1}{\kilo\sps}$. Taking the sampling theorem described above as a basis, this means that with a sampling rate of $\qty{44.1}{\kilo\sps}$ only frequencies below $\qty{22.05}{\kilo\hertz}$ can be represented. Frequencies up to about $\qty{22}{\kilo\hertz}$ can thus still be represented correctly. This corresponds to the hi-fi frequency range of good stereo systems. 
</indepth>

You can test your knowledge of the sampling theorem with the following exercise.

[question:AF619]
