---
created: "2026-03-10 at 10:32"
tags:
  - fleeting
publish: "false"
---
> Pre prac 2 lecture.
---
- Task C is new this year, the figures that he cites shows the two ways to accomplish. They just want us to show the layout of the 3 registers and the control signals between them. It will depict what will happen on a per clock cycle basis.

> Discussion Tutorial 4 Now

- SRAMS are faster than DRAMS but the DRAMS are less expensive and smaller
- Drams are just caps, so analog. SRAMS, uses standard flip flops and digital gates.
- EPROM - read and written electronically. All storage cells erases to same inital state before a write through UV exposure. There is a phsyically window that the UV light can be shined through. Classical ROM required that the data could only be written once at manufacture which is terrible, EPROM helped solve this issue.
- EEPROM can be written into anytime without erasing contents.
- Flash ememory balances cost and functonality. This accesses blocks of memory and not individual bytes like EEPROM. It allows for higher density than the similar to EPROM.
- Traditional DRAM is async, SDRAM is synchronized with the external clock sisgnal and runs at the full speed of the processor which allows it to achieve higher data rates.
- DDR Ram - achieves higher data rate 3 ways.
	- synchronized to the rising and failling edge of the cock rather than just the rising
	- Uses higher clock rate on the bus to increase the transfer rate
	- Uses buffering scheme
- **DRAMS are typically expressed as bits and not bytes**, make sure to standardize the unit when you are making the comparison
- Question 6.9 using billion hours of operations, look to the theory as to why
- Try to express the number of the final answer as months
- ECC memory using the hamming algorithm! 
- All the check bits will be at the positions of $2^n$. Converting to binary will allow you to see which sums the check bits will be used for.
- The result of the checksum tells you where the error is.
- 