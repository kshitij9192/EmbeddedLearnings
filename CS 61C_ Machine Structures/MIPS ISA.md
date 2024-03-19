ISA -> Instruction Set Architecture

Each CPU designer provides its ISA which is basically the programming interface for that particular piece of hardware.

## ISA 
RISC -> Reduced Instruction Set Computer
RISC was designed on the philosophy of keeping the instruction set small and simple, which makes it easier to build hardware quickly. Let software do the hardwork by utilizing these simple instruction sets.

MIPS architecture follows RISC.
MIPS supports 32 registers in CPU core. The access to the data on these registers is quite fast.
Why not have many more registers on CPU ? {GoldiLock's problem}
If we have too many registers in CPU, they will loose the quick access feature { Too many register will increase memory space and hence access time will be affected.}

These registers store the operands for any instruction during execution.
The registers are named R0, R1, R2, ..., R31
Registers don't have a type, as variables have in C. The operation determines how the contents of registers will be treated.
Few examples of translation among C and Assembly:
![9692fb8a01f30f7afca04de121274ba5.png](../_resources/9692fb8a01f30f7afca04de121274ba5.png)



## Data transfer: From memory to Registers
Load Instruction -> Loads data from memory (RAM) to the CPU register
Store Instruction -> Stores data from CPU Register to RAM
![39ee814c73ad434501c407b87c657a31.png](../_resources/39ee814c73ad434501c407b87c657a31.png)

Some CPUs provide instruction cache and data cache separately.
The code memory segment is cached into the Instruction cache.
The data memory segment is cached into the data cache.

Another one:
![728c417116a8c9a3986462b267ce6e73.png](../_resources/728c417116a8c9a3986462b267ce6e73.png)
In above case, $s3 stores the base address of array.
Then we offset $s3 by 12 to reach A[3].

Another one:
![4f5a58d5bde267bc7d422e0d8bc15b24.png](../_resources/4f5a58d5bde267bc7d422e0d8bc15b24.png)