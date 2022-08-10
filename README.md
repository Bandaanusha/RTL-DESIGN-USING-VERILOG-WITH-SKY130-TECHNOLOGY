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
 2. Day 2-Timing libs, hierarchial vs flat synthesis and efficient flop coding styles
  2.1 SKY130RTL D2SK1 -Introduction to timing.libs
    2.1.1 SKY130RTL D2SK1 L1 Lab4 Introduction to dot lib part1
    2.1.2 SKY130RTL D2SK1 L2 Lab4 Introduction to dot lib part2
    2.1.3 SKY130RTL D2SK1 L3 Lab4 Introduction to dot lib part3
  2.2 SKY130RTL D2SK2 - Hierarchial vs Flat Synthesis
    2.2.1 SKY130RTL D2SK2 L1 Lab5 hierarchial vs flat synthesis part1
    2.2.2 SKY130RTL D2SK2 L2 Lab5 hierarchial vs flat synthesis part2
  2.3 SKY130RTL D2SK3 - Various Flop Coding Styles and optimization
    2.3.1 SKY130RTL D2SK3 L1 Why Flops and Flop coding styles part1
    2.3.2 SKY130RTL D2SK3 L2 Why Flops and Flop coding styles part2
    2.3.3 SKY130RTL D2SK3 L3 Lab flop synthesis simulations part1
    2.3.4 SKY130RTL D2SK3 L4 Lab flop synthesis simulations part2
    2.3.5 SKY130RTL D2SK3 L5 Intresting optimizations part1
    2.3.6 SKY130RTL D2SK3 L6 Intresting optimizations part2
3. Day 3 - combinational and sequential optimizations
 3.1 Introduction to optimizations
 3.2 Combinational logic optimizations
 3.3 Sequential logic optimizations
 3.4 Sequential optimizations for unused outputs
```
## 1. Day1 - Introduction to Verilog RTL design and synthesis
### 1.1. SKY130RTL D1SK1 - Introduction to open-source simulator iverilog
Simulator is tool used for simulating the design. iverilog is a open source simulator. Simulating Register transfer level (RTL) design checks adherence of RTL design to specifications. 
#### 1.1.1. SKY130RTL D1SK1 L1 Introduction iverilog design and test bench
Design is a verilog code intended for particular functionality to meet with the required specifications.TestBench is the setup to apply stimulus to the design to check its functionality. Fig 1 shows working of testbench.
![1](https://user-images.githubusercontent.com/62790565/183249511-3da7501f-e4a4-4fa0-90a3-cf6888604666.jpeg)
<br>Fig 1
<br>Simulator looks for the changes on the input signals, upon changes to the input the output is evaluated. Fig 2 shows iverilog based simulation flow, Applying Design and testbench to iverilog simulator generates value Change Dump (vcd) file indicates that any changes in the input are dumped to output. gtkwave tool is used to view the input and output waveforms.
![2](https://user-images.githubusercontent.com/62790565/183249896-56e0d3bc-885d-40b6-8c9a-a75ccb72ca6a.jpeg)
Fig 2
###  1.2  SKY130RTL D1SK2- Labs using iverilog and gtkwave
Fig 3 shows terminal window creating a directory VLSI and git clone sky130RTLDesignAndSynthesisWorkshop directory from https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git and walking through files in sky130RTLDesignAndSynthesisWorkshop directory. lib folder consists of all sky130 library cells and verilog_model consits of verilog code for all the standard cells.``
<br> Fig 3
<br> In this session, I've performed simulation of multiplexer. I've added both the RTL design code and test bench code in iverilog to generate vcd file which I used in gtkwave generator to get the output waveformes after simulation. The output was generated by taking the inputs from the testbench code.
Here is design code multiplexer.
```
module good_mux (input i0 , input i1 , input sel , output reg y); 
	always @ (*)
	begin
		if(sel)
		y <= i1;
		else 
		y <= i0;
	end
endmodule**
```
Testbench code of multiplexer
```
`timescale 1ns / 1ps
module tb_good_mux;
// Inputs
reg i0,i1,sel;
// Outputs
wire y;
  		// Instantiate the Unit Under Test (UUT), name based instantiation
	good_mux uut (.sel(sel),.i0(i0),.i1(i1),.y(y));
	//good_mux uut (sel,i0,i1,y);  //order based instantiation
initial begin
	$dumpfile("tb_good_mux.vcd");
	$dumpvars(0,tb_good_mux);
	// Initialize Inputs
	sel = 0;
	i0 = 0;
	i1 = 0;
	#300 $finish;
end
always #75 sel = ~sel;
always #10 i0 = ~i0;
always #55 i1 = ~i1;
endmodule*
```
The following commands on terminal to simulate multiplexer design code
```
$ iverilog good_mux.v tb_good_mux.v
$ ./a.out
$ gtkwave tb_good_mux.vcd
```
Fig 4 is  a view of output of multiplexer on gtkwave
![Screenshot from 2022-08-06 19-19-58](https://user-images.githubusercontent.com/62790565/183253261-e6831deb-7bf6-4d22-a8d1-f420e5ca653c.png)
Fig 4
### 1.3 SKY130RTL D1SK3 Introduction to Yosys and Logic synthesis
#### 1.3.1 SKY130RTL D1SK3 L1 Introduction to yosys
Yosys is a synthesizer, a tool used for converting the RTL to netlist.Fig 5 shows the flow of yosys,applying design and .lib files to yosys we get netlist as output.read_verilog command is used to read the design, read_liberty command to read the .lib file and write_verilog command to write out the netlist file.Netlist is representation of the design in form of cells present in .lib.
![5](https://user-images.githubusercontent.com/62790565/183275983-e5d109b6-a27e-4dc2-ab8b-1d9cacadafb6.jpeg)
<br>Fig 5
<br>Output of simulating by applying netlist and testbench to iverilog and viewing generated vcd file on gtkwave toolshould be same as output of simulating by applying design and testbench to iverilog and viewing generated vcd file on gtkwave provided testbench applied in both the cases should is same, then the sysnthesis is said to be verified.
![6](https://user-images.githubusercontent.com/62790565/183276366-111784a5-b222-4721-90f6-b44a21aa0112.jpeg)
Fig 6
#### 1.3.2 SKY130RTL D1SK3 L2 Introduction to logic synthesis part1
RTL design is a behavioral representation of the required specification .Synthesis is RTL to Gate level translation. the design is converted into gates and the connections are made between the gates. This gives out as a file called netlist.Fig 7 gives the illustration of synthesis
![7](https://user-images.githubusercontent.com/62790565/183277889-190764f8-0f55-462c-8226-6d74e1f8a031.jpeg)

<br>Fig 7
<br>.lib is a collection of logical modules.It includes basic logic gates like And, Or, Not, etc. Same gate has different flavours such has slow, medium, fast.

![8](https://user-images.githubusercontent.com/62790565/183277894-226874e3-d83e-43c2-9e27-39dff657d03b.jpeg)

<br>Fig 8
<br>Consider the above digital circuit, the minimum clock period is given by the equation :
```
Tclk > Tcq-a + Tcombi +Tsetup-b
```
Combinational delay in logic path determines the maximum speed of operation of digital logic circuit.So we need fast cells to make Tcombi small increases the speed of operation.The following equation gives the maximum hold time
```
Thold_b < Tcq_a +Tcombi
```
To ensure that there are n "HOLD" issues at DFF_B shown in Fig 8,  we need cells that work slowly. Hence we need cells that works fast to meet the required performance and we need cells that work slow to meet HOLD. This collection of different flavours of cells forms the .lib . Load in the Digital Logic circuit is capacitance. Faster the charging/ discharging of capacitance lesser the cell delay. To charge or discharge the capacitance fast, we need transistors capable of sourcing more current. Wide transistors offfers low delay but requires mre area and power. Narrow transistors requires less area and power but offers more delay. Hence faster cells comes with a penality of area and power.
### 1.4 SKY130RTL D1SK4 Labs using Yosys and SKY130PDK's
#### 1.4.1 SKY130RTL D1SK4 L1 Lab3 yosys 1 good mux Part1
Moving into VLSI to sky130RTLDesignAndSynthesisWorkshop to verilog_files and then invoking yosys
```
$ cd VLSI
$ cd sky130RTLDesignAndSynthesisWorkshop
$ cd verilog_files
$ yosys
yosys >
```
Reading library files and design of multiplexer and synthesizing it and displaying gates
```
> read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
> read_verilog good_mux.v
> synth -top good_mux
> abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
> show
```

![Screenshot from 2022-08-07 12-13-20](https://user-images.githubusercontent.com/62790565/183279565-365fd63f-2081-43d2-952d-8ef6bf9b1ce3.png)

Generating netlist and displaying it
```
> write_verilog -noattr good_mux_netlist.v
> !gvim good_mux_netlist.v
```
Fig9 shows the netlist
## 2. Day 2-Timing libs, hierarchial vs flat synthesis and efficient flop coding styles
### 2.1 SKY130RTL D2SK1 -Introduction to timing.libs
#### 2.1.1 SKY130RTL D2SK1 L1 Lab4 Introduction to dot lib part1
This lab guides us through the .lib files where we have all the gates coded in. According to the below parameters the libraries will be characterized to model the variations.sky130_fd_sc_hd__tt_025C_1v80 named library is 130 nm library typical process at 25 degree celsius and at 1v.
![10](https://user-images.githubusercontent.com/62790565/183284976-2063f72b-86e6-4560-ae0e-17af548b3fbd.JPG)
<br> Fig 10
<br> With in the lib file, the gates are delared as follows to meet the variations due to process, temperatures and voltages.
With in the lib file, the gates are declared as follows to meet the variations due to process, temperatures and voltages.
![Screenshot from 2022-08-07 15-32-47](https://user-images.githubusercontent.com/62790565/183285736-6d66015a-5f6d-484c-8767-52429e2aacdf.png)
<br> Fig 11
<br> For the above example, for all the 2 combinations i.e 2^2 (2 is no.of  input variables), the delay, power and all the related parameters for each gate are mentioned.
<br> This image displays the power consumtion comparision.
![166107259-6fa398a4-2099-4da3-9b93-818c2c3f2404](https://user-images.githubusercontent.com/62790565/183285918-594e9856-9207-4220-8e1f-6a1e6a933152.JPG)
<br> Fig 12
<br> Below image is the delay order for the different flavor of gates.
![166187423-d21465e1-abc3-4ad0-a534-60f8e706ab6f](https://user-images.githubusercontent.com/62790565/183285933-a9fb50a8-493d-4c6a-b198-3db670c4ff35.JPG)
<br> Fig 13
### 2.2 SKY130RTL D2SK2 - Hierarchial vs Flat Synthesis
#### 2.2.1 SKY130RTL D2SK2 L1 Lab5 hierarchial vs flat synthesis part1
Design having multiple modules in it are analyzed here.Consider the multiple_modules.v design consisting two submodules. code of this design is :
```
module sub_module2 (input a, input b, output y);
	assign y = a | b;
endmodule

module sub_module1 (input a, input b, output y);
	assign y = a&b;
endmodule


module multiple_modules (input a, input b, input c , output y);
	wire net1;
	sub_module1 u1(.a(a),.b(b),.y(net1));  //net1 = a&b
	sub_module2 u2(.a(net1),.b(c),.y(y));  //y = net1|c ,ie y = a&b + c;
endmodule
```
To invoke yosys and synthesize use the following commands:
```
$ yosys
> read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
> read_verilog multiple_modules.v
> synth -top multiple_modules
> abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
```
To display gatelevel design use the following command:
```
> show multiple_modules
```
This displays hierarchial design as shown in Fig 14
![Screenshot from 2022-08-07 15-58-25](https://user-images.githubusercontent.com/62790565/183287346-cce344ba-1fd5-41c7-b54d-5634eac064e6.png)
<br> Fig 14
<br> To generate netlist and display is use the following commands
```
> write_verilog -noattr multiple_modules_hier_netlist.v
> !gvim good_mux_netlist.v
```
<br> The synthesizer considers the module hierarcy and does the mapping accordting to instantiation. Here is the hierarchical netlist code for the multiple_modules:
```
module multiple_modules(a, b, c, y);
	  input a;
	 input b;
	 input c;
	  wire net1;
	 output y;
  sub_module1 u1 (.a(a),.b(b),.y(net1) );
  sub_module2 u2 (.a(net1),.b(c),.y(y));
endmodule

module sub_module1(a, b, y);
 wire _0_;
 wire _1_;
 wire _2_;
 input a;
 input b;
 output y;
 sky130_fd_sc_hd__and2_0 _3_ (.A(_1_),.B(_0_),.X(_2_));
 assign _1_ = b;
 assign _0_ = a;
 assign y = _2_;
endmodule

module sub_module2(a, b, y);
wire _0_;
 wire _1_;
 wire _2_;
input a;
input b;
 output y;
 sky130_fd_sc_hd__lpflow_inputiso1p_1 _3_ (.A(_1_),.SLEEP(_0_),.X(_2_) );
 assign _1_ = b;
 assign _0_ = a;
 assign y = _2_;
endmodule
```
#### 2.2.2 SKY130RTL D2SK2 L2 Lab5 hierarchial vs flat synthesis part2
The following commands are used to flatten the hierarchy and display gate level circuits:
```
> flatten
> show
```
![Screenshot from 2022-08-07 16-12-44](https://user-images.githubusercontent.com/62790565/183287459-a3cd6edd-60cf-4802-ae21-b959de02f371.png)
<br> Fig 15
<br> To generate netlist and display is use the following commands
```
> write_verilog -noattr multiple_modules_flatten_netlist.v
> !gvim good_mux_netlist.v
```
<br> In flattened netlist, the hierarcies are flattend out and there is single module i.e, gates are instantiated directly instead of sub_modules. Here is the flattened netlist code for the multiple_modules:
```
module multiple_modules(a, b, c, y);
	 wire _0_;
	 wire _1_;
	 wire _2_;
	 wire _3_;
	 wire _4_;
	 wire _5_;
	 input a;
	 input b;
	 input c;
	 wire net1;
	 wire \u1.a ;
	 wire \u1.b ;
	 wire \u1.y ;
	 wire \u2.a ;
	 wire \u2.b ;
	 wire \u2.y ;
	output y;
	 sky130_fd_sc_hd__and2_0 _6_ (
	  .A(_1_),
	 .B(_0_),
	 .X(_2_)
	);
	 sky130_fd_sc_hd__lpflow_inputiso1p_1 _7_ (
	  .A(_4_),
	  .SLEEP(_3_),
	  .X(_5_)
	 );
	 assign _4_ = \u2.b ;
	 assign _3_ = \u2.a ;
	 assign \u2.y  = _5_;
	 assign \u2.a  = net1;
	 assign \u2.b  = c;
	 assign y = \u2.y ;
	 assign _1_ = \u1.b ;
	 assign _0_ = \u1.a ;
	 assign \u1.y  = _2_;
	 assign \u1.a  = a;
	 assign \u1.b  = b;
	 assign net1 = \u1.y ;
	endmodule
```
Module level synthesis
The following commands are used to synthesize and to show gatelevel circuit of submodule1 of multiple_modules.v design
```
> read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
> read_verilog multiple_modules.v
> synth -top submodule1
> abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
> show
```
![Screenshot from 2022-08-07 16-52-44](https://user-images.githubusercontent.com/62790565/183288320-e6233a10-c27f-407a-adf9-5e9f635a3542.png)
<br> Fig 16
<br> Module level synthesis is significant when there is multiple instantiation of same module.
### 2.3 SKY130RTL D2SK3 - Various Flop Coding Styles and optimization
#### 2.3.1 SKY130RTL D2SK3 L1 Why Flops and Flop coding styles part1

![17](https://user-images.githubusercontent.com/62790565/183291263-1754b75b-1e00-410f-b12a-11c683db9d6b.jpeg)

consider the digital circuit shown in Fig 17, changes in inputs a,b,c are propagated to the output Y with propagation delay with a glitch. If there are more combinatinal circuits output of which is input to the other, there will more glitches in the output makes it unstable. Hence we need flops to store which restricts glitches in output as output changes with clock. Flops are initialized by set and reset inputs. set=1 sets the output to 1 and reset=1 sets the output to 0.
<br> Four types of flop initialization by set and reset inputs
1.asynchronous reset
2. synchronous reset
3. asynchronous set
4. synchronous set
<br> D flip flop with asynchronous reset
<br> Digital circuit
![1d](https://user-images.githubusercontent.com/62790565/183303297-83df0773-6571-4edf-9e70-4bfad04e556e.jpeg)
<br> Fig 18
<br> Code of design d flip flop with asynchronous reset
```
module dff_asyncres ( input clk ,  input async_reset , input d , output reg q );
always @ (posedge clk , posedge async_reset)
begin
	if(async_reset)
		q <= 1'b0;
	else	
		q <= d;
end
endmodule
```
<br> Simulation result
![ardff](https://user-images.githubusercontent.com/62790565/183292968-ca2b7d3b-5a64-400d-b99e-22680c7746d2.png)
Fig 19

<br> Synthesized circuit
![d1](https://user-images.githubusercontent.com/62790565/183292995-bacbacbd-0b5d-4cb4-86f8-e73d2ebe0ed8.png)
Fig 20
<br> D flip flop with synchronous reset
<br> Digital circuit
![3d](https://user-images.githubusercontent.com/62790565/183303349-fa789de6-d17f-4743-b836-d3b67626e152.jpeg)
<br> Fig 21
<br> Code of design d flip flop with synchronous reset
```
module dff_syncres ( input clk , input async_reset , input sync_reset , input d , output reg q );
always @ (posedge clk )
begin
	if (sync_reset)
		q <= 1'b0;
	else	
		q <= d;
end
endmodule
```
<br> Simulation result
![srd](https://user-images.githubusercontent.com/62790565/183293341-d9962e3b-0694-4423-ae1a-41742eb91c8d.png)
Fig 22

<br>  Synthesized circuit
![d2](https://user-images.githubusercontent.com/62790565/183293370-17bfd9f9-f77a-4db3-a100-98b9edd0ace2.png)
<br> Fig 23
<br> D flip flop with asynchronous set
<br> Digital circuit
![2d](https://user-images.githubusercontent.com/62790565/183303417-fee8f31b-495f-49b0-8fde-c86c8c738c5a.jpeg)
<br> Fig 24
<br> Code of design d flip flop with asynchronous set
```
module dff_async_set ( input clk ,  input async_set , input d , output reg q );
always @ (posedge clk , posedge async_set)
begin
	if(async_set)
		q <= 1'b1;
	else	
		q <= d;
end
endmodule
```
<br> Simulation result
![asd](https://user-images.githubusercontent.com/62790565/183293778-ebc2de57-6199-4042-bdf1-d0938feac7df.png)
Fig 25

<br>  Synthesized circuit
![d3](https://user-images.githubusercontent.com/62790565/183293821-f7783ead-27f0-4b77-aa47-d0ada542aa00.png)
<br>Fig 26

<br> D flip flop with asynchronous and synchronous reset
<br> Digital circuit
![4d](https://user-images.githubusercontent.com/62790565/183303394-359d3499-a278-4e2b-aa4e-fde6b7026bf4.jpeg)
<br> Fig 27
<br> Code of design d flip flop with asynchronous and synchronous reset
```
module dff_asyncres_syncres ( input clk , input async_reset , input sync_reset , input d , output reg q );
always @ (posedge clk , posedge async_reset)
begin
	if(async_reset)
		q <= 1'b0;
	else if (sync_reset)
		q <= 1'b0;
	else	
		q <= d;
end
endmodule
```
<br> Simulation result
![arsrd](https://user-images.githubusercontent.com/62790565/183294416-f292d862-2a1f-4fad-9cba-fcefedcde2bc.png)
Fig 28

<br> Synthesized circuit
![d4](https://user-images.githubusercontent.com/62790565/183294460-90e5bb9a-dd85-4191-bd47-734f223fc6c3.png)
Fig 29

#### 2.3.5 SKY130RTL D2SK3 L5 Intresting optimizations part1
This lab session deals with some automatic and interesting optimisations of the circuits based on logic. In the below example, multiplying a number with 2 doesn't need any additional hardware and only needs connecting the bits from a to y and grounding the LSB bit of y is enough and the same is realized by Yosys.

![m2](https://user-images.githubusercontent.com/62790565/183295368-b59485b9-2fbd-443b-a67b-f32aec968272.jpeg)
Fig 30

```
module mul2 (input [2:0] a, output [3:0] y);
	assign y = a * 2;
endmodule
```
<br> Synthesized circuit
![m1](https://user-images.githubusercontent.com/62790565/183295275-32f2c0f1-24c7-4c82-b710-129a6cd78ab0.png)
<br> Fig 31
<br> Netlist
Fig 32
<br> When it comes to multiplying with powers of 2, it just needs shifting as shown below:
```
5   *  2  =  10
101          1010
5   *  4  =  20
101          10100
5   *  8  =  40
101          101000
```
Multiplying with 9
![m3](https://user-images.githubusercontent.com/62790565/183296373-91d02f8b-90ae-4853-9c6d-207d6e5045f8.jpeg)
<br>Fig 33
<br>Code
```
module mul2 (input [2:0] a, output [5:0] y);
	assign y = a * 9;
endmodule
```
Synthesized circuit

## 3. Day 3 - combinational and sequential optimizations
### 3.1 Introduction to optimizations
Combinational logic optimization is squeezing logic to get the most optimised design i.e. area and power savings. In can be done by 
1. constant propagation (direct optimization)
2. Boolean logic optimization can be achevied by K-map and Quine McKluskey
<br> Constant propagation
Consider following iilustration of combinational circuit with A, B, C as inputs and Y as output. If there is constant propagation '0' through input A then circuit can be modified as not gate and the number of MOS transistors required decreases, there by optimizing power and area.
![co1](https://user-images.githubusercontent.com/62790565/183302138-d7a5e671-baa7-4c80-b707-dd2f0432b9c1.jpeg)
Fig 34

<br>Boolean Optimization
Boolean optimization can be done in two ways one is K- map and the other is Quine McKluskey method.Consider following illustration of combinational circuit, optimizing boolean function minimized the number of gates used, hence optimized area and power used.
![co2](https://user-images.githubusercontent.com/62790565/183302157-8dedbd2f-d0a5-4287-81de-fbdb4fc09e44.jpeg)
Fig 35

<br>Sequential logic optimization can be done by
<br>1.Basic - Sequential constant propagation
<br>2.Advanced - State optimization, Retiming, Sequential logic cloning (Floor Plan Aware Synthesis)
<br>Sequential constant propagation
Consider the following illustration of sequential ciruit, here as the input D=0, for any value of reset the output Q=0, hence due to sequential constant propagation of Q=0 results in constant output Y=1. This optimizes the resources used.
![so1](https://user-images.githubusercontent.com/62790565/183302331-c213e6ff-028f-4423-b25d-554697b4434c.jpeg)
Fig 36

<br>State optimization - Optimization of unused states

<br> Sequential logic cloning (Floor Plan Aware Synthesis)
Consider following illustration of sequential circuit, flip flops B and C are at long ditsance from flip flop A hence there is large delay of reachhing output from A to B and C. If there is huge slack at input of flip flop A then flip flop A can be cloned aas two copies and can be placed near to flip flop B and C. This optimizes the time.
![so2](https://user-images.githubusercontent.com/62790565/183302341-bd2253cb-6ba6-4ac2-80dc-65ca163fa890.jpeg)
Fig 37

<br>Retiming
Consider following illustration of sequential ciruit.Here we can see that the combinatinal circuit between flipflop A & B  and B & C are different. Speed of operation depends on low delay circuit. Hence by retiming if we distribute logic in such a way that both combinational circuits between flip flop A & B and B & C have almotst same delay speed of operation increases and hence performance of the sequential circuit increases.
![so3](https://user-images.githubusercontent.com/62790565/183302348-24f5ecda-5eea-41f8-a548-35869653fdb1.jpeg)
Fig 38







