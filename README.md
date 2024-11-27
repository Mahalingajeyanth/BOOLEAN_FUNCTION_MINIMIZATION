# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**


**Logic Diagram**
![IMG-20241029-WA0004 1](https://github.com/user-attachments/assets/54db04b9-202e-455d-bb82-a3207ce5bb26)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~c)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```

Developed by: RegisterNumber:24900649


**RTL realization output**
![Screenshot (2)](https://github.com/user-attachments/assets/1d553408-1b94-4cbe-b62c-4914a80bf226)


**Timing Diagram**
![wave form](https://github.com/user-attachments/assets/6aa65c40-2361-4cba-92e0-58feb36e62e9)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

