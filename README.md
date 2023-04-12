# ALU-Project
This github repository describes about the 1 -Bit, 4-Bit Logic Unit (ALU) using Circuit Verse.

### Introduction to the ALU:-  
  *	ALU stands for Arithmetic Logic Unit. <br />
  *	It is a combinational digital circuit that performs arithmetic and bitwise operations.<br />
  * The flow of bits and the operations performed on them in the subunits of the ALU are controlled by gated circuits.
  *	It’s an important component of computer’s Central Processing Unit (CPU).<br />
  *	In this Project, it performs Addition, Subtraction, NAND and NOR operations.<br />

![image](https://user-images.githubusercontent.com/102464427/231547016-a3ff2f8f-b0c8-47b5-81bc-fa3591a7c141.png)

### Function:-  
*	It can perform any simple arithmetic operations (add, sub etc..) and logical operation such (And, OR) etc.  
*	Depending on the ‘OP’  selected, the result to be shown at the ‘OUT’.  
*	It stands as an Integrated Circuit (IC) (74181). It also can be synthesized using VHDL.  

A Basic ALU supports these common logic operations.
 Arithmatic Operation:-
* ALU accepts the inputs in binary format and performs the Add (with carry), Sub (with Borrow), Two's complement etc.
* The inputs are summed, subtracted or performed the required operations and show up the output in the "OUT."
* in the two's complement, an input is subtracted from the zero and the output appears in "OUT."

 ### Bitwise Logical Operation:-
*  AND- the bitwise operation of AND appears in the "OUT."
*  And so on. it can show up to any logic function such as, OR, XOR, XNOR, NAND, NOR etc.

### Advantage:-
* It supports parallel architecture and applications with high performance.
* It has the capability of performing instructions on a very large set and has a high range of accuracy.

# A Detailed Explanation:-
In the above attached image the ALU is 1 Bit and only can perform Full Addition, Full Subtraction, NAND and NOR operation.

 ### Full Adder:
* A full Adder is a Combinational Circuit which can take 3 inputs at a time and show the addition result.
* The addition results are labelled as SUM and CARRY.
* A full adder is a cascade connection of 2 half adders.
* An extra input is then provided to the half adder-2 and both the carry from the half-adders are performed OR operation to get the CARRY for the Full-Adder.
* Here the full-adder is created using the _sub-circuit_ of the half adder.
* _sub-circuit_ are the self contained circuits that appears as black boxes.

![fa](https://user-images.githubusercontent.com/102464427/231560776-4d453780-b34a-47c4-861a-e1c2d6b4f517.png)


#### Half Adder:
*  A half adder can take only 2 inputs and perform the operation.
*  While the sum is taken out by the XOR operation of the both the inputs, the CARRY is taken out by the AND operation of the both inputs.
*  The expression for the SUM is SUM = (A ^ B). CARRY= (A & B).

![image](https://user-images.githubusercontent.com/102464427/231559859-6df5b162-3397-4f90-9d00-7555c4cd8303.png)

#### Half Subtractor:
* The half subtractor has the same structure as the half adder has.
* Only change is that, it has a NOT gate placed at the any one input at the carry section.
* But, in subtractor, we call the sum as the "Difference" or "D" and the carry is known as "Borrow" or "B."
* The expression for the DIFFEENCE is DIFFERENCE = (A ^ B). BORROW= (A' & B).

![image](https://user-images.githubusercontent.com/102464427/231561717-2db1abf0-f6f2-4ead-832d-05ee3e053a32.png)

### Full-Subtractor:
* The connection of the full subtractor is as same as full-adder, i.e, placing two half-subtractors in cascade.

![image](https://user-images.githubusercontent.com/102464427/231562467-6c9f90e4-cb0b-4595-8f00-e82e197e6656.png)

### NAND:
* NAND gate is also known as **Universal Gate**, as we can implement any circuit using this gate itself.
* This is just a combination of AND and followed by a NOT gate.
* In the ALU, the Sub-Circuit of the NAND gate is being used.
* The expression for the NAND gate is X= ~(A & B).

![image](https://user-images.githubusercontent.com/102464427/231564061-9a38486b-f116-458b-91a2-ee99d725e05b.png)

### NOR:
* Like NAND, NOR is also known as an **Universal gate**.
* This is just a combination of OR and followed by a NOT gate.
* In the ALU, the Sub-Circuit of the NOR gate is being used.
* The expression for the NOR gate is X= ~(A | B).

![image](https://user-images.githubusercontent.com/102464427/231564711-ff4864a6-80c0-4a30-9a6c-5c4fba0f02e5.png)



 






