### TITTLE:
Design a 4 bit binary to BCD converter using verilog.

### THEORY:
BCD code plays an important role in digital circuits. The BCD stands for Binary Coded Decimal Number. In BCD code, each digit of the decimal number is represented as its equivalent binary number. So, the LSB and MSB of the decimal numbers are represented as its binary numbers.ln the 4 bit binary to BCD code converter, the input is 4- bit binary so there is 16 possible combinations. From 10 to 15 decimal numbers, since we cannot represent these numbers by 4 bit BCD code, so we need 8 bit to represent such 2 digit decimal number.But the first 3 bits are zero. Therefore, we can ignore the first 3 bit and we are going to use remaining 5 bits to represent such number in BCD code.

### PROGRAM:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus

using Verilog programming.

Developed by: vasanth s

egisterNumher: 212222110052

module bcd(input [3:0] bin_in, output reg [3:0] bcd_out);

always @* begin

case (bin_in) 4'be000: bcd_out = 4'b0000;

4'b0001: bcd_out = 4'b0001;

4'be010: bcd_out = 4'b9910;

4'b0011: bcd_out = 4'b0011;

4'b0100: bcd_out = 4'b0100;

4'b0101: bcd_out = 4'b0101;

4'b0110bcd_out = 4'b0110;

4'b0111: bcd_out = 4'b0111;

4'b1000: bcd_out = 4'b1000;

4'b1001: bcd_out = 4'b1001;

default: bcd_out = 4'bxxxx;
endcase

end

endmodule
```
### LOGIC DIAGRAM:
![1](https://github.com/vasanth0908/Simulation-project--Digital-Electronics/assets/122000018/b2f88ad7-73cd-456f-94c7-5888a5d96c40)


### TRUTH TABLE:
![2](https://github.com/vasanth0908/Simulation-project--Digital-Electronics/assets/122000018/109b8424-0f80-4d64-8c5b-c31048bb58d1)

### TIMING DIAGRAM:

### Result:
4 bit binary to BCD converter using verilog has been Designed by using verilog



image

RESULT:
Thus,to design a 4 bit binary to BCD converter is implemented successfully in Quartus using Verilog programming.
