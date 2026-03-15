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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule



/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Suvetha R 
RegisterNumber:212225220113 */


**RTL realization**
C:\Users\acer\Pictures\Screenshots\Screenshot 2026-03-14 105929.png
**Output:**

**RTL**
C:\Users\acer\Pictures\Screenshots\Screenshot 2026-03-15 154241.png
**Timing Diagram**
C:\Users\acer\Pictures\Screenshots\Screenshot 2026-03-14 111439.png
**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

