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

Developed by: 212223230140
RegisterNumber:Naveen kumar V
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule
```



**RTL realization**

**Output:**



**RTL**
![booleanfunction1](https://github.com/Naveenkumarvedarajan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147140428/da91af6d-229b-4612-98d1-b286d9696bbe)


**Timing Diagram**
![booleanfunction](https://github.com/Naveenkumarvedarajan/BOOLEAN_FUNCTION_MINIMIZATION/assets/147140428/3be49505-776f-494e-8b29-368139a991da)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

