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
```
module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule
```

**RTL realization**
<img width="1920" height="1080" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/6ea81209-f324-46f2-83ea-295b836bed3f" />

<img width="1920" height="1080" alt="Screenshot (89)" src="https://github.com/user-attachments/assets/0d44c96f-3494-4f1a-a34e-07ec4e6f9faa" />


**RTL**
<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/e97560fa-b2e0-4b18-9621-4b40e453f5ca" />


<img width="1920" height="1080" alt="Screenshot (90)" src="https://github.com/user-attachments/assets/2dd8d231-47f2-4d31-acdf-54c694fd407e" />

**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/3ea1f79c-daf2-42da-84d2-284aa3db40ab" />
<img width="1920" height="1080" alt="Screenshot (90)" src="https://github.com/user-attachments/assets/68bb8b34-c29b-4f61-a846-0c9b5cdddbfb" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

