# TITTLE
simulate octal to binary converter.

# THEORY
An octal number system uses a base of 8, meaning it has 8 possible digits: 0, 1, 2, 3, 4, 5, 6, and 7. On the other hand, the binary number system uses a base of 2, with only two possible digits: 0 and 1.

To convert an octal number to binary, we need to convert each digit of the octal number into its equivalent binary representation.

Here's a table showing the conversion of each octal digit to binary:

![image](https://github.com/SandhiyaR1/Simulation-project--Digital-Electronics/assets/113497571/7b65ac65-5682-4df8-8192-c6e290a5be49)
To perform the conversion, we can use a combinational logic circuit, such as a case statement, as shown in the Verilog code example. The input to the converter is the octal number, represented as a binary-coded decimal (BCD) format. For example, if the octal number is 5, its BCD representation is 3'b101.

Inside the case statement, we map each possible octal digit to its corresponding binary value using the table above. The resulting binary value is then assigned to the binary output. If an invalid octal digit is provided, such as 8 or 9, the default case can be used to handle the error condition.

By implementing this logic in Verilog, we can simulate the octal to binary conversion and obtain the binary representation of an octal number.

# LOGIC DIAGRAM
![image](https://github.com/SandhiyaR1/Simulation-project--Digital-Electronics/assets/113497571/52efa983-a2a7-44bf-a97d-a040f39ae877)


# NETLIST DIAGRAM

![deass2](https://github.com/SandhiyaR1/Simulation-project--Digital-Electronics/assets/113497571/faccdfc2-427b-417e-8e19-0a65c4ef71aa)


# TIMING DIAGRAM
![image](https://github.com/SandhiyaR1/Simulation-project--Digital-Electronics/assets/113497571/3fbaea12-9e08-41f9-b5a7-9f4be7602419)

# PROGRAM
```
module ass(y0,y1,y2,y3,y4,y5,y6,y7,a,b,c);
input y0,y1,y2,y3,y4,y5,y6,y7;
output a,b,c;
or(a,y4,y5,y6,y7);
or(b,y2,y3,y6,y7);
or(c,y1,y3,y5,y7);
endmodule
```


# REFERENCE
Thus the simulation of octal to binary coverter is obtained.

