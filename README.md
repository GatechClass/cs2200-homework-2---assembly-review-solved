# cs2200-homework-2---assembly-review-solved
**TO GET THIS SOLUTION VISIT:** [CS2200 Homework 2 – Assembly Review Solved](https://mantutor.com/product/cs2200-computer-systems-and-networks-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112894&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS2200 Homework 2 - Assembly Review Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Homework 2 – Assembly Review

1 Problem 1: Getting Started with the LC-3300

In this homework, you will be using the LC-3300 ISA to complete a Tower of Hanoi move-counting function. Before you begin, you should familiarize yourself with the available instructions, the register conventions and the calling convention of LC-3300. Details can be found in the section, Appendix A: LC-3300 Instruction Set Architecture, at the end of this document.

The assembly folder contains several tools for you to use:

• assembler.py: a basic assembler that can take your assembly code and convert it into binary instructions for the LC-3300.

• lc3300.py: the ISA definition file for the assembler, which tells assembler.py the instructions supported by the LC-3300 and their formats.

• lc3300-sim.py: A simulator of the LC-3300 machine. The simulator reads binary instructions and emulates the LC-3300 machine, letting you single-step through instructions and check their results.

To learn how to run these tools, see the README.md file in the assembly directory.

Before you begin work on the second problem of the homework, try writing a simple program for the LC-3300 architecture. This should help you familiarize yourself with the available instructions.

We have provided a template, mod.s, for you to use for this purpose. Try writing a program that performs the mod operation on the two provided arguments. A correct implementation will result in a value of 2.

You can use the following C code snippet as a guide to implement this function:

int mod(int a, int b) {

int x = a; while (x &gt;= b) {

x = x – b;

}

return x;

}

There is no turn-in for this portion of the assignment, but it is recommended that you attempt it in order to familiarize yourself with the ISA.

2 Problem 2: Tower of Hanoi

For this problem, you will be implementing the missing portions of the program that calculates the minimum number of moves to solve the Tower of Hanoi problem for n disks.

You will be finishing a recursive implementation of the Tower of Hanoi minimal moves calculator program that follows the LC-3300 calling convention. Recursive functions always obtain a return address through the function call and return to the callee using the return address.

Here is the C code for the Tower of Hanoi minimal moves calculator you have been provided:

int minimumHanoi(int n) {

if (n == 1) return 1;

else

return (2 * minimumHanoi(n – 1)) + 1;

}

Note that this C code is just to help your understanding and does not need to be exactly followed. However, your assembly code implementation should meet all of the given conditions in the description.

Open hanoi.s file in the assembly directory. This file contains an implementation of the Tower of Hanoi minimal moves calculator program that is missing significant portions of the calling convention. Near the bottom of the hanoi.s we have provided multiple numbers that you can use to test your homework. They are located at labels testNumDisks1, testNumDisks2, testNumDisks3. Be sure to use these provided integers by loading them from the labels into registers. None of the numbers provided and tested will be lower than

1.

Complete the program by implementing the various missing portions of the LC-3300 calling convention. Each location where you need to implement a portion of the calling convention is marked with a TODO label as well as a short hint describing the portion of the calling convention you should be implementing. Try to use logical left shift somewhere in your assembly.

3 Problem 3: Short Answer

Please answer the following question in the file named answers.txt:

4 Deliverables

• hanoi.s: your assembly code from Section 2

• answers.txt: your answer to the problem from Section 3

5 Appendix A: LC-3300 Instruction Set Architecture

The LC-3300 is a simple, yet capable computer architecture. The LC-3300 combines attributes of both ARM and the LC-2200 ISA defined in the Ramachandran &amp; Leahy textbook for CS 2200.

The LC-3300 is a word-addressable, 32-bit computer. All addresses refer to words, i.e. the first word (four bytes) in memory occupies address 0x0, the second word, 0x1, etc.

All memory addresses are truncated to 16 bits on access, discarding the 16 most significant bits if the address was stored in a 32-bit register. This provides roughly 64 KB of addressable memory.

5.1 Registers

The LC-3300 has 16 general-purpose registers. While there are no hardware-enforced restraints on the uses of these registers, your code is expected to follow the conventions outlined below.

Table 1: Registers and their Uses

Register Number Name Use Callee Save?

0 $zero Always Zero NA

1 $at Assembler/Target Address NA

2 $v0 Return Value No

3 $a0 Argument 1 No

4 $a1 Argument 2 No

5 $a2 Argument 3 No

6 $t0 Temporary Variable No

7 $t1 Temporary Variable No

8 $t2 Temporary Variable No

9 $s0 Saved Register Yes

10 $s1 Saved Register Yes

11 $s2 Saved Register Yes

12 $k0 Reserved for OS and Traps NA

13 $sp Stack Pointer No

14 $fp Frame Pointer Yes

15 $ra Return Address No

1. Register 0 is always read as zero. Any values written to it are discarded. Note: for the purposes of this project, you must implement the zero register. Regardless of what is written to this register, it should always output zero.

3. Register 2 is where you should store any returned value from a subroutine call.

4. Registers 3 – 5 are used to store function/subroutine arguments. Note: registers 2 through 8 should be placed on the stack if the caller wants to retain those values. These registers are fair game for the callee (subroutine) to trash.

5. Registers 6 – 8 are designated for temporary variables. The caller must save these registers if they want these values to be retained.

7. Register 12 is reserved for handling interrupts. While it should be implemented, it otherwise will not have any special use on this assignment.

8. Register 13 is the everchanging top of the stack; it keeps track of the top of the activation record for a subroutine.

9. Register 14 is the anchor point of the activation frame. It is used to point to the first address on the activation record for the currently executing process.

10. Register 15 is used to store the address a subroutine should return to when it is finished executing.

5.2 Instruction Overview

The LC-3300 supports a variety of instruction forms, only a few of which we will use for this project. The instructions we will implement in this project are summarized below.

Table 2: LC-3300 Instruction Set

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0000 DR SR1 unused SR2

0001 DR SR1 unused SR2

0010 DR SR1 immval20

0011 DR BaseR offset20

0100 SR BaseR offset20

0101 SR1 SR2 offset20

0110 AT RA unused

0111 unused

1000 SR1 SR2 offset20

1001 DR unused PCoffset20

1010 DR SR1 unused 00 SR2

1010 DR SR1 unused 01 SR2

1010 DR SR1 unused 10 SR2

1010 DR SR1 unused 11 SR2

1011 SR unused

ADD

NAND

ADDI

LW

SW

BEQ

JALR

HALT

BGT

LEA

SLL

SRL

ROL

ROR

FABS

5.2.1 Conditional Branching

Branching in the LC-3300 ISA is a bit different than usual. We have a set of branching instructions including BEQ, BGT, and FABS which offer the ability to branch upon a certain condition being met. These instructions use comparison operators, comparing the values of two source registers. If the comparisons are true (for example, with the BGT instruction, if SR1 &gt; SR2), then we will branch to the target destination of incrementedPC + offset20. For FABS, if SR &lt; 0 then we will branch to the series of microstates for negation.

5.3 Detailed Instruction Reference

5.3.1 ADD

Assembler Syntax

ADD DR, SR1, SR2

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0000 DR SR1 unused SR2

Operation

DR = SR1 + SR2;

Description

The ADD instruction obtains the first source operand from the SR1 register. The second source operand is obtained from the SR2 register. The second operand is added to the first source operand, and the result is stored in DR.

5.3.2 NAND

Assembler Syntax

NAND DR, SR1, SR2

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0001 DR SR1 unused SR2

Operation

DR = ~(SR1 &amp; SR2);

Description

The NAND instruction performs a logical NAND (AND NOT) on the source operands obtained from SR1 and SR2. The result is stored in DR.

5.3.3 ADDI

Assembler Syntax

ADDI DR, SR1, immval20

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0010 DR SR1 immval20

Operation

DR = SR1 + SEXT(immval20);

Description

The ADDI instruction obtains the first source operand from the SR1 register. The second source operand is obtained by sign-extending the immval20 field to 32 bits. The resulting operand is added to the first source operand, and the result is stored in DR.

5.3.4 LW

Assembler Syntax

LW DR, offset20(BaseR)

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0011 DR BaseR offset20

Operation

DR = MEM[BaseR + SEXT(offset20)];

Description

An address is computed by sign-extending bits [19:0] to 32 bits and then adding this result to the contents of the register specified by bits [23:20]. The 32-bit word at this address is loaded into DR.

5.3.5 SW

SW SR, offset20(BaseR)

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0100 SR BaseR offset20

Operation

MEM[BaseR + SEXT(offset20)] = SR;

Description

An address is computed by sign-extending bits [19:0] to 32 bits and then adding this result to the contents of the register specified by bits [23:20]. The 32-bit word obtained from register SR is then stored at this address.

5.3.6 BEQ

Assembler Syntax

BEQ SR1, SR2, offset20

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0101 SR1 SR2 offset20

Operation

if (SR1 == SR2) {

PC = incrementedPC + offset20

}

Description

A branch is taken if SR1 is equal to SR2. If this is the case, the PC will be set to the sum of the incremented PC (since we have already undergone fetch) and the sign-extended offset[19:0].

5.3.7 JALR

JALR AT, RA

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0110 AT RA unused

Operation

RA = PC;

PC = AT;

Description

First, the incremented PC (address of the instruction + 1) is stored into register RA. Next, the PC is loaded with the value of register AT, and the computer resumes execution at the new PC.

5.3.8 HALT

Assembler Syntax

HALT

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

0111 unused

Description

The machine is brought to a halt and executes no further instructions.

5.3.9 BGT

Assembler Syntax

BGT SR1, SR2, offset20

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1000 SR1 SR2 offset20

Operation

if (SR1 &gt; SR2) {

PC = incrementedPC + offset20

}

Description

A branch is taken if SR1 is greater than SR2. If this is the case, the PC will be set to the sum of the incremented PC (since we have already undergone fetch) and the sign-extended offset[19:0].

5.3.10 LEA

LEA DR, label

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1001 DR unused PCoffset20

Operation

DR = PC + SEXT(PCoffset20);

Description

An address is computed by sign-extending bits [19:0] to 32 bits and adding this result to the incremented PC (address of instruction + 1). It then stores the computed address into register DR.

5.3.11 SLL

Assembler Syntax

SLL DR, SR1, SR2

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1010 DR SR1 unused 00 SR2

Operation

DR = SR1 &lt;&lt; SR2;

Description

The value stored in SR1 is logically left shifted by the value stored in SR2, and the result is stored in DR.

5.3.12 SRL

Assembler Syntax

SRL DR, SR1, SR2

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1010 DR SR1 unused 01 SR2

Operation

DR = SR1 &gt;&gt; SR2;

Description

The value stored in SR1 is logically right shifted by the value stored in SR2, and the result is stored in DR.

5.3.13 ROL

ROL DR, SR1, SR2

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1010 DR SR1 unused 10 SR2

Operation

DR = (SR1 &lt;&lt; SR2) | (SR1 &gt;&gt; (32 – SR2));

Description

Bits in SR1 are ”rotated” left by SR2 number of bits using circular shifting. During a left rotation, the bits that are shifted out from the left are brought back in on the right side.

5.3.14 ROR

Assembler Syntax

ROR DR, SR1, SR2

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1010 DR SR1 unused 11 SR2

Operation

DR = (SR1 &gt;&gt; SR2) | (SR1 &lt;&lt; (32 – SR2));

Description

Bits in SR1 are ”rotated” right by SR2 number of bits using circular shifting. During a right rotation, the bits that are shifted out from the right are brought back in on the left side.

5.3.15 FABS

Assembler Syntax

FABS SR

Encoding

31302928272625242322212019181716151413121110 9 8 7 6 5 4 3 2 1 0

1011 SR unused

Operation

if (SR &lt; 0) {

SR = ~(SR &amp; SR);

SR += 1;

}

Description

If SR is less than zero, then the microcontroller will redirect to the series of negate microstates.
