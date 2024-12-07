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

![Screenshot 2024-12-06 112604](https://github.com/user-attachments/assets/8c6478e5-3805-4f5a-a3be-b382bfe04ad3)


HALF SUBTRACTOR

![Screenshot 2024-12-06 112610](https://github.com/user-attachments/assets/82f3e0e2-1825-4e6e-b017-7a5d6ead3338)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
i)HALF ADDER

module ha(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule
```


```
ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule

```

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber: 24007235*/

**RTL Schematic**


RTL SCHEMATIC FOR HALF ADDER

![Screenshot 2024-11-12 105735](https://github.com/user-attachments/assets/e574f78f-907a-4c9c-b871-eb93e8afe530)


**Output/TIMING Waveform**

TIMING FOR HALF ADDER

![Screenshot 2024-12-06 113809](https://github.com/user-attachments/assets/ad7bbd83-1947-4def-88e2-5ecf9df33db8)


**RTL Schematic**

RTL SCHEMATIC FOR HALF SUBTRACTOR


![Screenshot 2024-11-12 112423](https://github.com/user-attachments/assets/a81ce73e-e88a-4314-bd79-144e02c56828)




**Output/TIMING Waveform**


![Screenshot 2024-12-06 115217](https://github.com/user-attachments/assets/5394bdb2-46d0-44eb-ba91-40f3fa9fb1c9)






**Result:**

Thus the truth table of logic gates in Quartus || using Verilog programming are studied, verified and executed successfully.
