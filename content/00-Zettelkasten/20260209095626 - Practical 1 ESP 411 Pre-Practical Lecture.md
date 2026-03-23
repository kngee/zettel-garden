---
created: 2026-02-09 at 09:56
tags:
  - fleeting
  - signalprocessing
publish: "false"
---
[[ESP 411_Prac1_guidelines_2026.pdf]]
[[Preprac1_v1_2026(1).pdf]]

---

- Look into Bit Reveral when implementing the FFT
- Recursive vs Iterative FFT, depending on what we choose, it will determine if we need bit reversal
- Understand the Butterfly Diagram
- Max out prac 1 to simplify pracs 2 and 3.
- Reuse the twiddle factors to optimize the implementation. take advantage of polarity to only half of the wheel.
- Serial vs FPGA implementation.
- Always assume FFT size is a power of 2 to simplify the mathematics.
- You can start your development in python to check your approach before converting to C and testing on the STM. We can mention this in the report.
- Screen Size is 320x240