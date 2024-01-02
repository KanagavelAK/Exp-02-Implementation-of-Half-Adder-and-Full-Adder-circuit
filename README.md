### NAME: Kanagavel A K
###   Register No: 212223230096
# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
### Developed by: Kanagavel A K
### RegisterNumber: 212223230096 
# Half Adder:
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
# Full adder:
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
*/
## Truthtable
### Half Adder:
![image](https://github.com/KanagavelAK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151514454/b74d1022-b67e-44ae-8385-b2edbc025d74)

### Full Adder:
![image](https://github.com/KanagavelAK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151514454/d9b4af75-4562-4300-88ed-51a451db467a)

## RTL realization
### Half Adder:
![image](https://github.com/KanagavelAK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151514454/b462d716-1004-403c-8fb8-d883a01f4c17)

### Full Adder:
![image](https://github.com/KanagavelAK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151514454/55b823b2-08ad-4c39-8237-93720150f8e0)

### Waveform:
### Half Adder:
![image](https://github.com/KanagavelAK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151514454/c9c86bf5-f97c-4cc5-aadd-c662d0ac008e)

### Full Adder:
![image](https://github.com/KanagavelAK/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151514454/02aea9c1-5cdb-4e3c-996b-f021f349a783)


### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming

