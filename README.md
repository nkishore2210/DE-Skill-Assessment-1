# DE-Skill-Assessment-1

Name:Kishore.N
Ref. No. 22008365

TITLE:

Design and simulate octal to binary encoder using verilog.

AIM:

To Design and simulate octal to binary encoder using verilog.

INTRODUCTION:

The 8 to 3 line Encoder is also known as Octal to Binary Encoder.
In 8 to 3 line encoder, there is a total of eight inputs, i.e., Y0, Y1, Y2, Y3, Y4, Y5, Y6, and Y7 and three outputs, i.e., A0, A1, and A2.
In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side.
Below are the block diagram and the truth table of the 8 to 3 line encoder.

LOGIC DIAGRAM:

![image](https://user-images.githubusercontent.com/118707090/215322107-dfaf0ee3-0a2b-4f5c-b8d5-1ae25c8a3b5a.png)

BLOCK DIAGRAM:

![image](https://user-images.githubusercontent.com/118707090/215322226-dcfacf6e-be93-4de8-9308-8f8c446afb8b.png)

TRUTH TABLE:

![image](https://user-images.githubusercontent.com/118707090/215322159-0ed48f24-81c5-4c98-a8c6-1e78fd1160ff.png)

EXPLANATION:

8 to 3-bit priority encoder is an encoder that consists of 8 input lines and 3 output lines.
It can also be called an Octal to a binary encoder.
Each input line has a base value of 8 (octal) and each output has a base value of 2 (binary).

PROGRAM:

module oc_bi_encoder(a0,a1,a2,a3,a4,a5,a6,a7,y1,y2,y3);
input a0,a1,a2,a3,a4,a5,a6,a7;
output y1,y2,y3;
or(y1,a4,a5,a6,a7);
or(y2,a2,a3,a6,a7);
or(y3,a1,a3,a5,a7);
endmodule

RTL DIAGRAM:

![de sa1 rtl](https://user-images.githubusercontent.com/118707090/215322598-95c41dee-986e-46cf-a3e3-900d8140bd26.png)

TIMING DIAGRAM:

![de sa1 td](https://user-images.githubusercontent.com/118707090/215322569-f4d3a517-6bbc-42bb-af48-1acb03a5e8b1.png)

RESULT:

Thus the design and simulation of octal to binary encoder using verilog is verified successfully.
