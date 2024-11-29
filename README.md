# BOOLEAN_FUNCTION_MINIMIZATION

Developed by: JAYAGANAPATHI S

RegisterNumber: 24900059

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

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
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
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

**LOGIC SYMBOL AND TRUTH TABLE:**

![Screenshot 2024-11-29 113030](https://github.com/user-attachments/assets/1f9a6a0a-a839-4536-bb0d-4840713e7468)


![Screenshot 2024-11-29 113044](https://github.com/user-attachments/assets/25ae6ed7-939d-497c-b456-a707e5e76a37)

**RTL realization**

![Screenshot ](https://github.com/user-attachments/assets/1a0a101f-c06f-42dc-aa2b-452c24df59b1)

**Output:**

![Screenshot 2024-11-29 112556](https://github.com/user-attachments/assets/5ddcbb11-5ada-460a-bff1-338bdc53859e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

