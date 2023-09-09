# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
#### Hardware 

PCs, Cyclone II , USB flasher

#### Software 

Quartus prime
### Theory
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

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: SUJITHRA B K N

RegisterNumber:  212222230153

#### HALF ADDER:

```
module ex03(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule
```

#### FULL ADDER:

```
module fulladder(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```

### Output:

### 1. RTL

#### HALF ADDER

![Screenshot 2023-09-02 091540](https://github.com/sujithrabkn/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477857/0ee058e6-1f15-44d6-8542-e9edcc0fc44e)

#### FULL ADDER

![Screenshot 2023-09-02 094443](https://github.com/sujithrabkn/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477857/697df826-b98b-4bac-9a42-491b5cac886c)



### 2. TRUTH TABLE 

#### HALF ADDER

![266654416-76d22e8d-9c16-483f-a86d-97010d36007a](https://github.com/sujithrabkn/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477857/876bdb21-7c9d-4e68-9545-322849786d7b)


#### FULL ADDER

![266654525-a5313912-38be-4892-a629-28e6c35d2b93](https://github.com/sujithrabkn/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477857/de98122f-d9f8-4cc0-9742-f2c2f058a7fb)


### 3. WAVEFORM

#### HALF ADDER

![Screenshot 2023-09-02 093245](https://github.com/sujithrabkn/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477857/d1451e89-67bd-4494-848a-9dee95fb6b2d)

#### FULL ADDER

![265629963-b5c9748a-da88-428a-9fda-90b04a98d9d0](https://github.com/sujithrabkn/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477857/0e1022a4-cd3e-4022-b843-26e60b1751bd)


### Result:

Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
