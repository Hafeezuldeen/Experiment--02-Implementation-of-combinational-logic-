NAME:HAFEEZUL DEEN .S
REFERENCE NUMBER:23008281
 
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
## Program:
```
module exp2de(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization
![WhatsApp Image 2023-11-24 at 21 14 32_d62e6b6a](https://github.com/Hafeezuldeen/Experiment--02-Implementation-of-combinational-logic-/assets/144979314/117e5d3b-33bb-4f4b-b712-1f1b7d0e0a64)
TRUTH TABLE:![WhatsApp Image 2023-11-24 at 21 14 33_c5959897](https://github.com/Hafeezuldeen/Experiment--02-Implementation-of-combinational-logic-/assets/144979314/82d469bc-98e8-45f5-a969-42fa063b435c)



## Timing Diagram
![image](https://github.com/Hafeezuldeen/Experiment--02-Implementation-of-combinational-logic-/assets/144979314/b3cee5d5-b46a-4324-aa30-46766f306eb1)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
