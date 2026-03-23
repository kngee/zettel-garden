---
created: 2026-02-09 at 20:19
tags:
  - permanent
  - signalprocessing
  - esp411
publish: "true"
---

See Also:

- ...

---

> What are the core subsystems in the required system

- We need to understand our audio source and then build two bits of external circuit which is just an *amplitude offset and scaling circuit* and *anti-aliasing filter*
- We need to be able to implement ADC on the STM board
- We need to implement the FFT algorithm from first principles on the STM board
- We need to be able to display the output on the screen without the use of any external libraries.

> What is the engineering challenge of this practical

- How do we go from the Fourier Transform to the Fast Fourier Transform?
- Motivate the design considerations necessary to explain our implementation decisions.
- **Figure out how the STM32 works and become a guru.**
	- We need to start making code snippets that go through the tutorials.

> Anti Alias Filter

- 20 kHz filter that is **Triple Interleaved**

> FFT Implementation

- Our FFT should be a minimum of 128 points of the sampled signal which would be between $0-1~V$.
- We can compare our FFT function with that from the DSP Library