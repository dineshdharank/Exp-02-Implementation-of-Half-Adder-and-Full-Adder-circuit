## Name: Dineshdharan.K
## Reg: 23014095

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

### Program:

## HALF ADDER:

~~~ module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule ~~~

## FULL ADDER:

~~~ module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule ~~~
 
## Truth Table:
Half Adder:

![Screenshot 2023-12-15 180904](https://github.com/dineshdharank/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145980096/ba53bca7-795b-4b01-bab0-b9b3de8653d2)

Full Adder:

![Screenshot 2023-12-15 180953](https://github.com/dineshdharank/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145980096/7b8d88cf-a45c-44fb-8cd4-e717a825b5b7)

## RTL:
Half Adder:

![Screenshot 2023-12-15 181120](https://github.com/dineshdharank/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145980096/08dd95d7-41ea-4984-abcb-75a6ae57fbc3)

Full Adder:

![Screenshot 2023-12-15 181202](https://github.com/dineshdharank/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145980096/e4aaf544-8634-40db-8ee9-ea577af3ee5a)


## Timing Diagram:
Half Adder:

![Screenshot 2023-12-15 181531](https://github.com/dineshdharank/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145980096/d03c68f1-27c8-49ca-80f4-b57102cd96b1)

Full Adder:

![Screenshot 2023-12-15 181618](https://github.com/dineshdharank/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145980096/a80c9b56-ec97-4996-bd8e-8ff3d0239b3a)


### Result:
