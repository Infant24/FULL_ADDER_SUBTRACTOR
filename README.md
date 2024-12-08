# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

## AIM:

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

## Full Adder and Full Subtractor

## Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

## Figure -1 FULL ADDER

## Full Subtractor

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

## Truthtable
![Screenshot 2024-12-08 183804](https://github.com/user-attachments/assets/f244a2af-1676-45b2-a306-dc31eb1fa46c)
![Screenshot 2024-12-08 183811](https://github.com/user-attachments/assets/e536e54d-5371-4062-b761-1f876258b9fd)


## Procedure
1. Type the program in Quartus software.
2. Compile and run the program.
3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
5. For different input combinations generate the timing diagram.




## Program:

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

### module fa(a,b,c,sum,carry);
### input a,b,c;
### output sum,carry;
### wire w1,w2,w3;
### assign sum=a^b^c;
### assign w1=a&b;
### assign w2=b&c;
### assign w3=c&a;
### assign carry=w1|w2|w3;
### endmodule

### module fs(df,bo,a,b,bin);
### input a,b,bin;
### output df,bo;
### wire w1,w2,w3;
### assign w1=a^b;
### assign w2=(~a&b);
### assign w3=(~w1&bin);
### assign df=w1^bin;
### assign bo=w2|w3;
### endmodule

### Developed by: Infant Maria Stefanie .F
### RegisterNumber: 24001512


## RTL Schematic
![Screenshot 2024-12-08 183821](https://github.com/user-attachments/assets/bc93d950-7e8d-4aeb-ba17-d1a6096e5b08)
![Screenshot 2024-12-08 183826](https://github.com/user-attachments/assets/e353babf-7420-4a63-8c23-76fb457f71c9)


## Output Timing Waveform
![Screenshot 2024-12-08 183834](https://github.com/user-attachments/assets/07da04e9-1968-45cc-be1e-0b9c15fa0c4b)
![Screenshot 2024-12-08 183840](https://github.com/user-attachments/assets/9af70d62-fe88-408f-ae45-66238c33f50d)


## Result:

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



