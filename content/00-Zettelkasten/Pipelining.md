---
created: 2026-03-05 at 12:27
tags:
  - permanent
  - computerarchitecture
publish: "true"
---
See Also:

- [[Techniques to speed up microprocessor speed]]

---

Pipelining is a processor design technique that we use to speed up a processor's execution of tasks by minimizing delay. 

![[Pasted image 20260305122855.png|center]]

We take advantage of multiple different execution processes that take place when we are to perform an instruction. There is a fetch, decode and execute involved that can all be run in parallel as opposed to one at a time. Therefore, pipelining performs different functions at the same time on different instructions. 

While it executes one, it fetches another, decodes another etc. but this is all happens at the same time as opposed to serial.