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

Developed by: DHARANYA.N
RegisterNumber:212223230044*/
```
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
```


**RTL realization**
![Screenshot 2024-03-20 174840](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742468/e9eafb9b-fb7c-4e47-acf1-c113d4ee6efa)

**LOGICGATE**
![Screenshot 2024-03-20 183735](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742468/373379fe-5d1d-4ef0-8177-df4103a50d5a)


**Timing Diagram**
![Screenshot 2024-03-20 175714](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742468/77122968-71b3-484b-ab94-1d145064c6d9)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

