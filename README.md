# BOOLEAN_FUNCTION_MINIMIZATION #

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software: – Quartus prime**


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

**BOOLEAN MINIMIZATION**


![WhatsApp Image 2024-12-21 at 8 56 17 AM](https://github.com/user-attachments/assets/9f69bad2-a30c-48de-bf3d-d452d2116997)


![WhatsApp Image 2024-12-21 at 8 56 30 AM](https://github.com/user-attachments/assets/38792f90-773a-4165-91c1-b4cf03b8b23f)


**TRUTH TABLE**

![image](https://github.com/user-attachments/assets/6542c99b-7818-4a63-aec5-a7195065e637)

![image](https://github.com/user-attachments/assets/21fe727f-048e-4c62-8d3a-3aa7e11d6c57)


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Trisha Priyadarshni Parida

RegisterNumber: 212224230293

*/

```i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```



**RTL:**

<img width="614" alt="EXP 2 DE RTL" src="https://github.com/user-attachments/assets/8956e3c0-ca9e-4ed7-aa0c-98a994885539" />

<img width="638" alt="EXP 2 DE FUNCT 2 RTL" src="https://github.com/user-attachments/assets/8da81774-f3c5-4706-bffc-0cb178f46beb" />


**Timing Diagram:**

<img width="960" alt="EXP 2 DE WAVEFORM" src="https://github.com/user-attachments/assets/6f542db4-eeea-4149-8ec6-93212f1713e1" />

<img width="958" alt="EXP 2 DE FUNCT 2 WF" src="https://github.com/user-attachments/assets/949f12b4-9fcf-4a71-9826-1fe7a0b7a7ad" />


**Result:**

Thus the given logic functions are implemented & their operations are verified using Verilog programming.

