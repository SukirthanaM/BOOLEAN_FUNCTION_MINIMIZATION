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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Sukirthana.M
RegisterNumber: 212224220112
```
module EXP2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
output F1,F2;
wire X1,X2,X3,X4,X5,X6;
assign X1=(~B)&(~D);
assign X2=(A)&(B)&(~C);
assign X3=(~A)&(B)&(D);
assign X4=(~Y)&(Z);
assign X5=(X)&(Y);
assign X6=(W)&(Y);
assign F1=X1|X2|X3;
assign F2=X4|X5|X6;
endmodule
```
*/


**RTL realization**
![image](https://github.com/user-attachments/assets/179bc725-8ffb-4742-906a-4868889eefa0)

**Output:**
![image](https://github.com/user-attachments/assets/69f664c7-d58e-4053-92b9-1fb3503cd8ae)

**Timing Diagram**
![Screenshot (73)](https://github.com/user-attachments/assets/52c84db0-d95d-4d82-b697-165d3439e60c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

