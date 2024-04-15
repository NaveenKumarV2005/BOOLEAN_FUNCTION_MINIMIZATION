# BOOLEAN_FUNCTION_MINIMIZATION
## Developed by:NAVEENKUMAR.V
## RegisterNumber: 212223220068
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

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

//type code for f2 as like f1 endmodule



## truth table:


![316395754-a9ccb75e-db7b-490e-8b69-10f820e6bff4](https://github.com/NaveenKumarV2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/151476286/65556930-73cf-4fe0-99f4-386561139f69)









![316395946-6835b6c0-9fe5-4f55-8288-53b7d0c42104](https://github.com/NaveenKumarV2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/151476286/ea7a10f2-719e-4ca9-8115-410fe9eab135)







**RTL realization**



![316222000-35846536-0657-4c35-9caa-81906cb5b6bd](https://github.com/NaveenKumarV2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/151476286/6432e9e0-24f8-495f-8e3d-4ebcdbbe7002)



**Output:**
**Logic Diagram**


![Screenshot 2024-04-15 221521](https://github.com/NaveenKumarV2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/151476286/2fc79cda-b028-4ff5-96a7-332131d05752)





**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

