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

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

HALF ADDER

![Screenshot 2024-11-25 202405](https://github.com/user-attachments/assets/b8915e2b-b090-4f13-9696-20af6e21fe89)

HALF SUBTRACTOR

![Screenshot 2024-11-25 202713](https://github.com/user-attachments/assets/46e5272a-b548-429c-a799-be47c7a8a865)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
HALF ADDER

module ha (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

HALF SUBTRACTOR

module halfsub(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

Developed by:S KANUSHA SREE
RegisterNumber:24001268
```
**RTL Schematic**

HALF ADDER
![ha logicgate](https://github.com/user-attachments/assets/b50f5480-c955-4d3b-95bb-a3ec8e0290b7)
HALF SUBTRACTOR
![halfsub logicgate](https://github.com/user-attachments/assets/6100edff-7872-4e40-8b8d-765751a02e2c)
**Output/TIMING Waveform**

HALF ADDER
![ha waveform](https://github.com/user-attachments/assets/c4797977-8242-4e0a-a613-11469f0dc21f)
HALF SUBTRACTOR
![halfsub waveform](https://github.com/user-attachments/assets/6ae1a278-fd3a-426a-b09b-1f07b5d49a32)
**Result:**
Designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.

