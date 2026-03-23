---
created: 2026-03-05 at 00:04
tags:
  - permanent
  - computerarchitecture
publish: "true"
---
See Also:

- [[Pipelining]]
- [[Branch Prediction]]
- [[Superscalar Execution]]
- [[Data Flow Analysis]]
- [[Speculative Execution]]

---

You could have designed the the fastest processor when it comes to responding to the task that is placed directly in front of it. However, designers have realized that to ensure optimal performance, we need to ensure that the processor is not sitting idle waiting for instructions at any given network.

It is the job of the *chipmaker* to make chips of greater and greater density but it is the job of the processor designer to figure out interesting ways to keep the machine doing useful tasks. There are a number of techniques that processor designers use to be able to do this.

![[Pasted image 20260305122059.png|center]]

The techniques use a combination of minimizing delay between tasks using a predicitve framework and by taking advanatage of quick access buffers. What is important to understand is that the techniques take advantage of processor power available to us by avoiding delays, it helps us make the best use of the available power.