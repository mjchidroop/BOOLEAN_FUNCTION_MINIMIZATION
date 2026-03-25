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

<img width="427" height="774" alt="image" src="https://github.com/user-attachments/assets/32ca0415-c8bb-4734-ad3c-708464143df7" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Chidroop M J  
RegisterNumber: 212225240029 
```verilog
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

<img width="785" height="433" alt="image" src="https://github.com/user-attachments/assets/1e6fb2e1-ae83-4af6-b005-fbe001f44f83" />

**Output:** 

<img width="1305" height="679" alt="image" src="https://github.com/user-attachments/assets/c6f40ed8-2219-481a-9b89-8ca8fb434cc8" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

