---
created: 2026-03-05 at 12:37
tags:
  - permanent
  - computerarchitecture
publish: "true"
---
See Also:

- [[Pipelining]]
- [[Techniques to speed up microprocessor speed]]

---

Branch prediction is a technique to speed up a processor's execution of instruction by taking advantage of periods where there is a delay by pre-empting which branch of instructions are likely to be executed next. If this can be predicted with a reasonably good accuracy then these branches can be loaded into a buffer and be made ready for quick access to the processor.

![[Pasted image 20260305124557.png|center]]

*I like this image because of the premeditation. Branch prediction effectively does the same, in that it makes the prediction and prepares for execution. There is enough time to withdraw if it so happens that the wrong prediction was made*.