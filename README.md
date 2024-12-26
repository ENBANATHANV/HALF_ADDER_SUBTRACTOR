
#### NAME : ENBANATHAN V
#### REG NO : 24001750
# EXPERIMENT-3 : HALF ADDER AND SUBTRACTOR



## AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

# Half Adder:

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

# Half Subtractor:

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

 # Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

# Program:
```
module HALF_ADDER_AND_HALF_SUBTRACTOR (A,B,sum,carry,difference,borrow);
input A,B;
output sum,carry,difference,borrow;
assign sum=A^B;
assign carry=A&B;
assign difference=A^B;
assign borrow=(~A)&B;
endmodule
```

# Truthtable:

![download](https://github.com/user-attachments/assets/07c839e0-4d6b-41a6-b978-05b5bfd1d5cc)


![Half-Adder-Truth-Table-](https://github.com/user-attachments/assets/7e06b4a3-cdef-42af-8ada-ed3fc5c1f171)

# RTL OUTPUT:
![Screenshot (32)](https://github.com/user-attachments/assets/aee2e69f-bf5a-4cb9-bb63-8683a3d25c2e)


# OUTPUT WAVEFORM:
![Screenshot (37)](https://github.com/user-attachments/assets/ba072065-1f2b-4df5-9496-b23a298d0b5d)


# Result:
Designed a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming.

