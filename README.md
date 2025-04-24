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
module exp2(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=(~B)&(~D)|(A)&(B)&(~C)|(~A)&(B)&(D);
assign F2=(~X)&(Z)|(X)&(Y)|(W)&(Y);
endmodule

Developed by:riyaz M 
RegisterNumber:212224040279


**RTL realization**

**Output:**

**RTL**
![WhatsApp Image 2025-04-24 at 11 29 03_2c70632e](https://github.com/user-attachments/assets/b0feb97a-cf06-4e71-8a7b-71ae512d6910)

**Timing Diagram**
![WhatsApp Image 2025-04-24 at 11 29 02_d57e2374](https://github.com/user-attachments/assets/e6c66ff3-9e83-4650-b86a-dd450879e139)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

