# BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy
## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

## Software :
Quartus prime

## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:
```
Developed by: NAVEEN KUMAR S
RegisterNumber: 212223040129
```
### F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 
```
module ex022(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1 =((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule
```
### F2=xy’z+x’y’z+w’xy+wx’y+wxy
```
module ex021(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
## Truth Table :
![image](https://github.com/user-attachments/assets/6870b772-1964-4a81-8652-e8a48f3de10d)
![image](https://github.com/user-attachments/assets/66f3bff8-1d7d-41df-84e1-2449b4c84db2)

## RTL realization:

![ex022](https://github.com/user-attachments/assets/05ef7302-2145-4d1f-adbc-10eabf79885a)
![ex021](https://github.com/user-attachments/assets/8156561c-c611-4f12-8c09-1741f0d94565)

## Timing Waveform:

![Screenshot 2024-09-20 133724](https://github.com/user-attachments/assets/64cd3547-b321-4547-97e1-ccdf4b922489)
![Screenshot 2024-09-27 140252](https://github.com/user-attachments/assets/3f598a70-6732-4d5a-9052-89ec8a3b54ac)

## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
