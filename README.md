# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**
<img width="320" height="193" alt="11" src="https://github.com/user-attachments/assets/f3223c21-69e9-4b45-9a46-ca08f8197808" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:MOHAMED ASARUDEEN A
RegisterNumber: 25005844 */
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```


**RTL realization**
<img width="1920" height="1080" alt="22" src="https://github.com/user-attachments/assets/5b868bb2-b14b-442c-b443-7d6f70ae0816" />


**Output:**

**RTL**
<img width="1920" height="1080" alt="33" src="https://github.com/user-attachments/assets/622a051c-4274-46e4-aeb8-08d348d4d41f" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

