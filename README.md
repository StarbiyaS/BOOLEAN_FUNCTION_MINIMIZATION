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

Developed by: STARBIYA S RegisterNumber:212223040208
```
module program2(A,B,C,D,F1);
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
````

**RTL realization**

**Output:**

![image](https://github.com/StarbiyaS/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870533/ec22c86a-cbf9-4ec3-8b9b-7bc9f22e23ad)



**Timing Diagram**
![image](https://github.com/StarbiyaS/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870533/9e10fdd0-db88-480f-bf3e-df851f50f2be)

![image](https://github.com/StarbiyaS/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870533/875e77fe-84f1-49bb-b38c-9129b2a90a89)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

