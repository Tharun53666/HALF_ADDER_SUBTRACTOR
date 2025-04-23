# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![ha](https://github.com/user-attachments/assets/5fe3af86-3872-4b51-bfed-8e2f3ae7dfe5)


Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![hs](https://github.com/user-attachments/assets/842f3f5c-60d8-48f2-92b7-690e84ea2bef)


Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

i)HALF ADDER
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
ii)HALF SUBTRACTOR
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule


Developed by: RegisterNumber:212224240170

**RTL Schematic**
![3(1)](https://github.com/user-attachments/assets/f47b72a6-e5a4-474a-8edc-fe26a6e0716d)


![exp3(2](https://github.com/user-attachments/assets/318a26fd-29fd-4747-9c17-57faf8d65dd7)


**Output/TIMING Waveform**
![3(1](https://github.com/user-attachments/assets/518644f0-6ca1-42af-bf47-27a16299ba92)

![exp 3(2)](https://github.com/user-attachments/assets/21f59269-7a31-4484-ba21-19ec07e68eb7)


**Result:**
Designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming hence the above the output was verified
