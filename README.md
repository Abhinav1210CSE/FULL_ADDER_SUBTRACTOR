# FULL_ADDER_SUBTRACTOR
# DATE:17/10/2024


Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**

/* Developed by: Abhinav.C.S RegisterNumber :24001247

FULL ADDER
module exp4fulladder(a,b,cin,sum,carry);
 input a,b,cin;
 output sum,carry;
 assign sum=( (a ^ b)^cin);
 assign carry= ( (a & b)| ( cin &(a ^ b )));
 endmodule

 FULL SUBTRACTOR
 module exp4fullsubtractor(a,b,bin,difference,borrow);
 input a,b,bin;
 output difference,borrow;
 assign difference= ( (a ^ b)^bin);
 assign borrow= ( ( a & b)| ( bin & ((a ^ b ))));
 endmodule

**RTL Schematic**

FULL ADDER

![WhatsApp Image 2024-12-01 at 10 19 57 PM](https://github.com/user-attachments/assets/f58f8597-b2c6-4299-86e9-be119a3dd370)

FULL SUBTRACTOR

![WhatsApp Image 2024-12-01 at 10 19 57 PM (1)](https://github.com/user-attachments/assets/a6baf4ea-6c69-4559-a31e-fbe8682ddcd1)


**Output Timing Waveform**
![WhatsApp Image 2024-12-01 at 10 19 57 PM (2)](https://github.com/user-attachments/assets/2eae3f15-3291-4125-a2b5-4289e98bd6c5)
![WhatsApp Image 2024-12-01 at 10 19 57 PM (3)](https://github.com/user-attachments/assets/e7659b7d-dd33-4a9c-971f-75069818dd59)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



