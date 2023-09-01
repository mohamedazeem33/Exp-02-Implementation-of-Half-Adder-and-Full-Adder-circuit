# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: MOHAMED AZEEM N
RegisterNumber:  212222110026

HALF ADDER PROGRAM:
__________________
module HALFADDER(a,b,c,s);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule

FULL ADDER PROGRAM:
___________________
module fulladd(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=((a&b)|(b&c)|(c&a));
endmodule

```
Logic symbol & Truthtable
RTL realization

### Output:
### HalfAdder output diagram:
![Screenshot (110)](https://github.com/mohamedazeem33/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121040764/ebeaae1d-8b99-49b2-a64e-0d5adde440de)
### FullAdder diagram output:
![Screenshot (113)](https://github.com/mohamedazeem33/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121040764/16a7496f-db3a-4857-9186-6dcfc87d385e)


### TIMING DIAGRAM
### half adder:
![Screenshot (109)](https://github.com/mohamedazeem33/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121040764/49509c8f-0a68-428f-913e-864f7eeb07d0)
### full adder:
![Screenshot (112)](https://github.com/mohamedazeem33/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121040764/0c31ea94-58b6-4eb5-b987-5a86de94a54a)



### TRUTH TABLE:
![DE exp 3 truth table](https://github.com/mohamedazeem33/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121040764/4f95e53c-d92c-43bd-aad6-314a5e1734f5)


![DE exp 3 truth table 2](https://github.com/mohamedazeem33/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121040764/a54676c0-c3a0-413b-bf88-5d42fc75917e)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
