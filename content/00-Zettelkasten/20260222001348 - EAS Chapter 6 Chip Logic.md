---
created: "2026-02-22 at 00:13"
tags:
  - fleeting
publish: "false"
---
> This note is to review the chip design section in chapter 6 of the textbook as too be able to implement the chip for the compoter memory practical.
---
- Chips are to be designed with trade offs in speed, cost and density in mind.
- A key design issue is the number of bits of data that can be written at a time. 
- **Chips contain an array of memory cells**.
- The horizontal lines connect to the select terminal of each chip 
- The vertical lines conect to the data-in terminal of each chip.
- 

> Module Organisation.

- A RAM chip will need as many memory chips required to the store the bits for a word.
- The example in the textbook is for a module that holds $256 kB$ of memory, in our practical we only need to design RAM for 256 bytes! 
- The bit size of the required address lines is calculated using the number of words that need to be addressed.  $$\text{Num bits in address}=\log_2(\text{Total Words})$$
- Each memory chip in the example handles the input and output of one bit.
- **The organisation works as long as the size of memory in words equals the number of bits per chip**
- We can build larger memory by arranging a number of these memory chips in an array. For example, if we wanted to make $1Mb$ word memory, then we can could array 4 of the $256kB$ word memory chips and then the effect this would have on the addressing is that 2 additional bits would be required on the select lines that serve to select which memory chip in the array we should use.
- The main challenge with the practical though is that i need to find a way to write memory such that i don't overwrite protected memory when I am directly working with *nibbles* and not *words*.
	- 