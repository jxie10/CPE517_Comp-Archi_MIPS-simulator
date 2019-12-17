This is a Lab of Stevens Institute of Technology CPE517_Comp Archi<br>
The goal of this assignment is to understand how pipelined MIPS datapath is performed. This pipelined simulator will not only model the functional behavior of each instruction, but also enable pipelined instruction processing.<br>
---
# Use Makefile to create an interactive shell<br>
The provided shell.c implements several command lines to control the execution of the simulator. You can think it as a command line version of the MARS simulator like loading and running program, examining register and memory values, etc. The shell accepts one program file as a command line argument and loads it into the program memory. The shell supports the following commands: <br>

•	g | G | go: simulate the program until it indicates that the simulator should halt.<br>
•	r | R | run <n>: simulate the execution of the machine for n instructions.<br>
•	mdump <low> <high>: dump the contents of memory, from location low to location high to the screen <low> and <high> address should be provided as hexadecimal numbers.<br>
•	rdump: dump the current instruction count, the contents of $0- $31, FLAG N, Z, C, V, and the PC to the screen.<br>
•	i | I | input reg_num reg_val: set register (denoted reg_num) to value (reg_val).<br>
•	? | help: print out a list of all shell commands.<br>
•	q | Q| quit: quit the shell.<br>
#Instructions can run:<br>
Use MARS to generate opcode and write them into a .txt, need to note *stall*.<br>
Instruction supply: add, addu, sub , subu, lui, ori, addi, addiu, lw, sw, bgyz, j. Also supply forwarding between ALU calculation operations. But there is some problems in lw forwarding.
