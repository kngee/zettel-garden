---
created: 2026-03-05 at 13:25
tags:
  - permanent
  - computerarchitecture
publish: "true"
---
See Also:

- [[Instruction execution Rate comparisons between different machines]]  

---
The main characteristic of a processor that we want to use is the fixed frequency of a processor that has a frequency of $f$, From this we can determine $\tau$ that we define as the cycle time. We are interesting in derving some basic measures of computer performance.

What we understand about a processor's instruction set is that not all instructions take the same amount of time to execute, so we define a parameter called Average Cycles Per Instruction that is specfic to a particular instruction. $CPI_I$, we then combine this paramater with the number of instructions in a particular program which we call the instruction count $I_c$. 
E
![[Pasted image 20260305211811.png|center]]

We are interesting being able to express the overall average cycles per instruction for a particular program. $$CPI=\frac{\sum_{i=1}^{n}CPI_i\times I_i}{I_c}$$
where $I_i$ is the number of instructions in a program of type $i$ ie. fetch or decode.

We can use this metric to retrieve the total processing time with the formula $$T=CPI\times I_c \times \tau$$
The first improvement that we can introduce to the program is understand that when an instruction is processed, a portion of that time is actual processing while the rest is memory transferring. 

The updated equation understands that the memory interactions are dependent on the memory cycle time. It is possible that the memory cycle time is greater than the processor cycle time.

The new equation is described with a few new parameters that are the sum fo the processor cycles and the memory references that need to be made.  $$T=I_c\times[p+(m\times k)]\times\tau$$
Processor design really becomes intricate at this point because there are 4 system attributes that can affect these parameters. Such as how you design the instruction set architecture, the technology for the compiler and the processor implementation and finally the cache and memory hierarchy.

Finally, some more measures that designed that describe the instructions executed per seconds in terms of Millions of instructions. This is simply derived using the parameters outlined above $$MIPS=\frac{I_c}{T\times10^6}=\frac{f}{CPI\times10^6}$$
The final measure that was introduced in this section that finds basic performance measures for CPUs is a measure interested in the number of floating point operations per second which we describe with $$MFLOPS = \frac{\text{Number of executed floating} - \text{point operations in a program}}{\text{Execution Time}\times 10^6}$$