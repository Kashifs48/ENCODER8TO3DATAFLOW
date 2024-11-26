Name: SYED KASHIF S

Register Number: 24006084

EXP5: ENCODER 8-3 DATA FLOW MODELLING
AIM:

To implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

SOFTWARE REQUIRED: Quartus prime

THEORY

Encoder 8 To 3

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/user-attachments/assets/77b06cd4-783b-40d8-9be7-fc7538d116d5)


Figure 01 Block Diagram of Encoder 8 * 3

Truth Table

![image](https://github.com/user-attachments/assets/5d2e6f9c-0ea5-49ff-b7f6-b9e496a769c5)


The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/user-attachments/assets/0262616d-f4c8-412e-abfc-a729d78954bb)


Figure 02 Encoder 8 * 3

Procedure

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

PROGRAM

Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming.

module encoder(din,a,b,c);
input[0:7]din;
output a;
output b;
output c;
assign a=din[4] | din[5] | din[6] | din[7];
assign b=din[2] | din[3] | din[6] | din[7];
assign c=din[2] | din[4] | din[6] | din[7];
endmodule 
RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling

![image](https://github.com/user-attachments/assets/cc478d14-c1d0-4cfb-96cc-e9455f71156a)


Output Timing Waveform
![image](https://github.com/user-attachments/assets/5dc1645f-678a-47f1-9e77-a607ddbd68d3)



RESULTS

Thus to implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables is done successfully.
