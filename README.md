### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., y0, y1, y2, y3, y4, y5, y6, and y7 and three outputs, i.e., a, b, and c. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![Screenshot 2024-12-09 204521](https://github.com/user-attachments/assets/f8b697dd-f764-4506-ae07-828e87ce54c1)


Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![Screenshot 2024-12-09 205928](https://github.com/user-attachments/assets/96c51f9f-fffb-4a2b-827b-be071f59463c)


The logical expression of the term A0, A1, and A2 are as follows:

y0 = y1 + y3 + y5 + y7

y1 = y2 + y3 + y6 + y7

y2 = y4 + y5 + y6 + y7

Logical circuit of the above expressions is given below:

![Screenshot 2024-12-09 094928](https://github.com/user-attachments/assets/4fb4a0f7-075c-4e1d-af3c-09e8827c6873)


Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by:Sarankumar.V RegisterNumber:24010668

```
module encoder(a,b,c,y0,y1,y2,y3,y4,y5,y6,y7);
input y0,y1,y2,y3,y4,y5,y6,y7;
output a,b,c;
assign a= ( y4 | y5 | y6 | y7);
assign b= ( y2 | y3 | y6 | y7);
assign c= ( y1 | y3 | y5 | y7);
endmodule
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![Screenshot 2024-12-09 095221](https://github.com/user-attachments/assets/6dd7d51d-010b-499e-abd7-e2ec7b5bf81b)

**RESULTS**
Thus the truth table of a logic for Encoder 8 to 3 in dataflow modelling in Quartus|| using verilog programming are studied,verified and executed successfully.



