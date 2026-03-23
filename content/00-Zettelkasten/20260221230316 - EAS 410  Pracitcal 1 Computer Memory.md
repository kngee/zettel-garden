---
created: "2026-02-21 at 23:46"
tags:
  - fleeting
publish: "false"
---
> This note will handle Task B of Practical 1 in EAS that relates to the design of RAM.
---

- The Task is to design an 8-bit, 256 byte RAM. A specfic memory chip design is to be used. The chip is an array of 8 by 8 array bits of information. Both full word and half word nibbles need to be written. 
- Right now I will review chapter 6 of the textbook to be able to do the chip design.
- Right now, I need to go into more detail, I can't just have the high level diagram of the RAM.
- Everythng that requires an explanantion requires an accompanying diagram. Now I need to figure out what those are.
	- We need to have a diagram that shows the logic for each chip, eahc chip has a row decoder, column decoder, the memory cells, logic for the write enable and inputs through the bit in, it needs input through the enable pin and it needs a data out that connects to its corresponding line to a specific index on the data bus.
	- 