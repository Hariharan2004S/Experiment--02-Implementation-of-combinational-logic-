# Experiment--04-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:Program For F1
```
module combilogic(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire G1,G2,G3,G4,G5;
assign G1=((~A)&(~B)&(~C)&(~D));
assign G2=((A)&(~C)&(~D));
assign G3=((~B)&(C)&(~D));
assign G4=((~A)&(B)&(C)&(D));
assign G5=((B)&(~C)&(D));
assign F1=G1|G2|G3|G4|G5;
endmodule
Program For F2

module combilogic(W,X,Y,Z,F);
input W,X,Y,Z;
output F;
wire G6,G7,G8,G9,G10;
assign G6=((X)&(~Y)&(Z));
assign G7=((~X)&(~Y)&(Z));
assign G8=((~W)&(X)&(Y));
assign G9=((W)&(~X)&(Y)); 
assign G10=((W)&(X)&(Y));
assign F=G6|G7|G8|G9|G10;
endmodule
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```
Developed by: Hariharan.S
RegisterNumber: 212222050016
``` 
*/
## RTL realization


## Output:
First Question
## RTL
![rtl1](https://github.com/Hariharan2004S/Experiment--02-Implementation-of-combinational-logic-/assets/123146156/29c7ea20-de06-4463-8dda-e6359dfa4b6f)

## Timing Diagram
![td1](https://github.com/Hariharan2004S/Experiment--02-Implementation-of-combinational-logic-/assets/123146156/12def9d3-6077-487b-8fd1-950ae5db5612)
Second Question
## RTL
![rtl2](https://github.com/Hariharan2004S/Experiment--02-Implementation-of-combinational-logic-/assets/123146156/1e288ed9-be83-42fc-a60e-60160bb76d64)

## Timing Diagram
![td2](https://github.com/Hariharan2004S/Experiment--02-Implementation-of-combinational-logic-/assets/123146156/216b7873-ad83-4637-9fc0-46580b4d141d)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
