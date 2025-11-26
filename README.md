# BOOLEAN-FUNCTION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 ```
 module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(w&y)|(x&y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:M MOHAMED SHAJID  RegisterNumber: 25013425


**RTL realization**

**Output:**
<img width="1321" height="637" alt="Capture boolean" src="https://github.com/user-attachments/assets/4bcda026-1c57-40eb-9d07-74360984ce18" />

**RTL:**
<img width="1343" height="592" alt="Capture b2" src="https://github.com/user-attachments/assets/96124e16-4c65-4d37-afdf-dccff6a94797" />


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
