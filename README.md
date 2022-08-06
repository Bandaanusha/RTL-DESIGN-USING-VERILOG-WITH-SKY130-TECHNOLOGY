# RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY
## Table of Contents
```
 1. Day1 - Introduction to Verilog RTL design and synthesis
  1.1. SKY130RTL D1SK1 - Introduction to open-source simulator iverilog
   1.1.1 SKY130RTL D1SK1 L1 Introduction iverilog design and test bench
  1.2  SKY130RTL D1SK2- Labs using iverilog and gtkwave
    1.2.1 SKY130RTL D1SK2 L1 Lab1 introduction to lab
    1.2.2 SKY130RTL D1SK2 L2 Lab2 introduction to iverilog gtkwave part1
    1.2.3 SKY130RTL D1SK2 L3 Lab2 introduction to iverilog gtkwave part2
  1.3 SKY130RTL D1SK3 Introduction to Yosys and Logic synthesis
    1.3.1 SKY130RTL D1SK3 L1 Introduction to yosys
    1.3.2 SKY130RTL D1SK3 L2 Introduction to logic synthesis part1
    1.3.3 SKY130RTL D1SK3 L3 Introduction to logic synthesis part2
 1.4 SKY130RTL D1SK4 Labs using Yosys and SKY130PDK's
    1.4.1 SKY130RTL D1SK4 L1 Lab3 yosys 1 good mux Part1
    1.4.1 SKY130RTL D1SK4 L2 Lab3 yosys 1 good mux Part2
    1.4.1 SKY130RTL D1SK4 L3 Lab3 yosys 1 good mux Part3
```
## 1. Day1 - Introduction to Verilog RTL design and synthesis
### 1.1. SKY130RTL D1SK1 - Introduction to open-source simulator iverilog
Simulator is tool used for simulating the design. iverilog is a open source simulator. Simulating Register transfer level (RTL) design checks adherence of RTL design to specifications. 
#### 1.1.1. SKY130RTL D1SK1 L1 Introduction iverilog design and test bench
Design is a verilog code intended for particular functionality to meet with the required specifications.TestBench is the setup to apply stimulus to the design to check its functionality. Fig 1 shows working of testbench.
![1](https://user-images.githubusercontent.com/62790565/183249511-3da7501f-e4a4-4fa0-90a3-cf6888604666.jpeg)
Fig 1
Simulator looks for the changes on the input signals, upon changes to the input the output is evaluated. Fig 2 shows iverilog based simulation flow, Applying Design and testbench to iverilog simulator generates value Change Dump (vcd) file indicates that any changes in the input are dumped to output. gtkwave tool is used to view the input and output waveforms.
![2](https://user-images.githubusercontent.com/62790565/183249896-56e0d3bc-885d-40b6-8c9a-a75ccb72ca6a.jpeg)
Fig 2
###  1.2  SKY130RTL D1SK2- Labs using iverilog and gtkwave
Fig 3 shows terminal window creating a directory VLSI and git clone sky130RTLDesignAndSynthesisWorkshop directory from https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git and walking through files in sky130RTLDesignAndSynthesisWorkshop directory. lib folder consists of all sky130 library cells and verilog_model consits of verilog code for all the standard cells.``
Fig 3
In this session, I've performed simulation of multiplexer. I've added both RTL design code and test bench code in iverilog to generate vcd file with







