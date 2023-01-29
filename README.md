# DE-Skill-Assessment-1

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

![sa1 rtl](https://user-images.githubusercontent.com/118707090/215322019-79cb3f57-9825-42e5-bcd9-33b808f600b6.png)

TIMING DIAGRAM:

![sa1 timing diagram](https://user-images.githubusercontent.com/118707090/215322041-7afa22cc-2990-4126-81cf-d10d99f25d19.png)

RESULT:

Thus the design and simulation of octal to binary encoder using verilog is verified successfully.
