---
created: 2025-12-18 at 07:20
tags:
  - telecommunications
  - fleeting
---
B. P. Lathi and Z. Ding, _Modern Digital and Analog Communication Systems_, 4th International ed. New York, NY, USA: Oxford University Press, 2010.

---
##### 1.1 Communication Systems
p2.For a signal to be efficiently transmitted, it may require that the band of the signal be modified.
p3.A typical communication systems model performs the same functions fundamentally.
p3.A channel is a physical medium that behaves like a filter because the signal may be attenuated and distorted.
p3.There are physical phenomena that can distort a signal waveform ie. frequency-dependent gains, multipath effects, Doppler Shifts.
p3.Distortion can be classed as either linear or non-linear. Regardless, there are a number of ways that we can correct for this distortion either at the transmitter or the receiver.
p3.Noise is one of the underlying factors that limit the rate of telecommunicaitons.
##### 1.2 Analog and Digital Messages  
p4.Digital communications has the added benefit of immunity to noise and interferences due to its finite alphabet.
p5.Regenerative repeaters allow for digital messages to be transmitted with higher accuracy over longer distances.
p6.Sampling Theorem states that if the highest frequency in the signal spectrum is $B$, the signal can be reconstrcted from its discrete samples taken uniformly at not less than $2B$ samples per second.
p7.Pulse-Coded Modulation is a very simple method for the translation of a quantized digital signal into a signal waveform.
p8.It was the transistor that made PCM practicable.
##### 1.3 Channel Effect, Signal-To-Noise Ratio, and Capacity
p9.The fundamental parameters and physical limitations that control the rate and quality of a digital communication system are its channel bandwidth $B$ and the power of the signal $P_s$.
p9.The bandwidth of a signal refers to the range of frequencies that it can transmit with reasonable fidelity. Signals rich in content will change quickly and therefore have a higher bandwidth than signals that are dull.
p9.A signal can be successfully sent over a channel if the channel bandwidth exceeds the signal bandwidth.
p9.Signal power $P_s$ has 2 roles in information transmission. Increasing the signal power strengthens the pulse of the signal and diminishes the effect of channel noise and interferance. A large signal power is necessary to maintain  a minimum SNR over a longer distance.
p9.The parameters of $B$ and $P_s$ are interchangable if we are interested in maintaining a given rate and accuracy of information transmission.
p10.In a given communication channel, one resource may be more valuable than another.
p10.SNR and bandwidth can both affect the channel *throughput*. The maximum *throughput* that can be achieved through a certain channel is defined ad the channel capacity.
p10.AWGN channel is an ideal model that captures distortionless channels and provides a performance upper bound for more general distortive channels. 
p10.The band-limited AWGN channel capacity was highlighted by Shannon's Equation $$C=Blog_2(1+SNR)~~~bits/s$$
p10.Shannon's equation brings out the limitation on the rate of communication imposed by $B$ and $SNR$
p11.Shannon's equation shows us the unequal trade effect that exists between the $B$ and $SNR$ parameters. 
##### 1.4 Modulation and Detection
p11.Modulation is performed to facilitate transmission. The baseband signal is the analog signal generated through A/D conversion.
p11.Channels cannot be moved to accomodate a signal. and so the message signal needs to be moved to accomodate the channel.
p11.A carrier is a sinusoid of high frequency with a number of parameters that can be varied in proportion to the baseband signal $m(t)$.
p11.For ease of transmission, the modulated signal should be of a wavelength that results in a practical antenna size when implemented.
p12.Modulation allows multiple signals to be transmitted at the same time in the same geographcal area without direct mutual interference.
##### 1.5 Digital Source Coding and Error Correction Coding
p13.Source coding is applied to maximally compress a given message without sacrificing its detection accuracy.
p13.Error correction codes rely on redundancy to combat the impacts of noise and interferance.
p13.Source coding and ECCs can be considered to fight against one another because ECCs introduce the redundancy that the source coding is trying to remove.
p14.A predicitable signal is not random and is fully redundant. A message only contains information if it is unpredictable.
p14.Source coding is trying to remove the most predictable and thus redundant parts of a message to only transmit the most unpredictable parts.
p14.Entropy coding is a technique that relates the information of a message with the probablity $P$.
p15.Joint source-channel coding can maximally remove signal redundancy without losing error correction.
##### 1.6 Historical Review of Modern Telecommunications
p16.Wireless communications is greatly dependent on the discovery of electromagnetics.
p16.Claude Shannon's seminal papers in 1948 changed everything and it just so happened to release alongside the first development of semiconductors.

