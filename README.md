![Screenshot 2023-11-24 154729](https://github.com/Hafeezuldeen/Experiment--02-Implementation-of-combinational-logic-/assets/144979314/cfec3cc3-ec00-4f36-8da7-03ef09e812ca)# Experiment--02-Implementation-of-combinational-logic
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
module exp2de(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization
![Screenshot 2023-11-24 154729](https://github.com/Hafeezuldeen/Experiment--02-Implementation-of-combinational-logic-/assets/144979314/4c4b6291-ccf6-46a0-8f9d-9582772cec14)
TRUTH TABLE:![WhatsApp Image 2023-11-24 at 21 14 33_c5959897](https://github.com/Hafeezuldeen/Experiment--02-Implementation-of-combinational-logic-/assets/144979314/82d469bc-98e8-45f5-a969-42fa063b435c)



## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
