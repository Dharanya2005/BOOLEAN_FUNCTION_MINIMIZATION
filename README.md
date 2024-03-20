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

Developed by:DHARANYA.N
RegisterNumber:21222323004
module exp22(A,B,C,D,F1);
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
*/


**RTL realization**
![Screenshot 2024-03-20 174840](https://github.com/Dharanya2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742468/1cc36a40-3c3d-4a20-950f-83965538f416)


**LOGICGATES**
![Screenshot 2024-03-20 183735](https://github.com/Dharanya2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742468/bcaf9f72-9575-4aa6-a02f-4932c2f1aa3a)

**Timing Diagram**
![Screenshot 2024-03-20 175714](https://github.com/Dharanya2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742468/f6035da4-ff25-4e34-94f9-25a72bb0545d)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

