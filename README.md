# RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY
## Table of Contents
[1. Day 1 - Introduction to Verilog RTL design and synthesis](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#1-day-1---introduction-to-verilog-rtl-design-and-synthesis)<br>
  * [1.1. Introduction to open-source simulator iverilog](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#11-introduction-to-open-source-simulator-iverilog)<br>
    - [1.1.1. Introduction iverilog design and test bench](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#111-introduction-iverilog-design-and-test-bench)<br>
  * [1.2.  Labs using iverilog and gtkwave](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#labs-using-iverilog-and-gtkwave)<br>
  * [1.3. Introduction to Yosys and Logic synthesis](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#13-introduction-to-yosys-and-logic-synthesis)<br>
    - [1.3.1. Introduction to yosys](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#131-introduction-to-yosys)<br>
    - [1.3.2. Introduction to logic synthesis](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#132-introduction-to-logic-synthesis)<br>
  * [1.4.Labs using Yosys and SKY130PDK's](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#14-labs-using-yosys-and-sky130pdks)<br>
 
[2. Day 2 -Timing libs, hierarchial vs flat synthesis and efficient flop coding styles](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#2-day-2-timing-libs-hierarchial-vs-flat-synthesis-and-efficient-flop-coding-styles)<br>
  * [2.1. Introduction to timing.libs](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#21-introduction-to-timinglibs)<br>
    - [2.1.1. Introduction to dot lib](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#211-sky130rtl-d2sk1-l1-lab4-introduction-to-dot-lib-part1)<br>
  * [2.2. Hierarchial vs Flat Synthesis](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#22-hierarchial-vs-flat-synthesis)<br>
    - [2.2.1. Lab on hierarchial vs flat synthesis part1](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#221-lab-on-hierarchial-vs-flat-synthesis-part1)<br>
    - [2.2.2. Lab on hierarchial vs flat synthesis part2](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#222-lab-on-hierarchial-vs-flat-synthesis-part2)<br>
  * [2.3. Various Flop Coding Styles and optimization](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#23-various-flop-coding-styles-and-optimization)<br>
    - [2.3.1.Why Flops and Flop coding styles](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#231-why-flops-and-flop-coding-styles23)<br>
    - [2.3.2. Labs on flop synthesis simulations](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#231-why-flops-and-flop-coding-styles23)<br>
    - [2.3.3. Intresting optimizations](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#233-intresting-optimizations)<br>
 
[3. Day 3 - combinational and sequential optimizations](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#3-day-3---combinational-and-sequential-optimizations)<br>
 * [3.1. Introduction to optimizations](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#31-introduction-to-optimizations)<br>
 * [3.2. Combinational logic optimizations](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#32-combinational-logic-optimizations)<br>
 * [3.3. Sequential logic optimizations](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#33-sequential-logic-optimizations)<br>
 * [3.4. Sequential optimizations for unused outputs](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#34-sequential-optimizations-for-unused-outputs)<br>

[4. Day 4 - GLS, blocking vs non-blocking and Synthesis-Simulation mismatch](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#4-day4--gls-blocking-vs-non-blocking-and-synthesis-simulation-mismatch)<br>
 * [4.1. GLS, Synthesis-Simulation mismatch and Blocking, Non-blocking statements](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#41-gls-synthesis-simulation-mismatch-and-blocking-non-blocking-statements)<br>
   - [4.1.1. GLS Concepts And Flow Using Iverilog](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#411-gls-concepts-and-flow-using-iverilog)<br>
   - [4.1.2. Synthesis Simulation Mismatch](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#412-synthesis-simulation-mismatch)<br>
   - [4.1.3.Blocking and Non-Blocking statements in verilog](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#413-blocking-and-non-blocking-statements-in-verilog)<br>
 * [4.2. Labs on GLS and synthesis-simulation mismatch](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#labs-on-gls-and-synthesis-simulation-mismatch)<br>
 * [4.3. Lab on Synthesis Simulation Mismatch for Blocking Statement](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#43-lab-on-synthesis-simulation-mismatch-for-blocking-statement)<br>

[5.Day 5 - if, case, for loop and for generate](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#5-day5--if-case-for-loop-and-for-generate)<br>
  * [5.1. If and Case constructs](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#51-if-and-case-constructs)<br>
    - [5.1.1. If construct](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#511-if-construct)<br>
    - [5.1.2. Case construct](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#512-case-construct)<br>
  * [5.2. Labs on incomplete if](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#52-labs-on-incomplete-if)<br>
  * [5.3. Labs on incomplete overlapping case](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#53-labs-on-incomplete-overlapping-case)<br>
  * [5.4. For Loop and For Generate For Loop](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#55-for-loop-and-for-generate)<br>
    - [5.4.1. Labs on for loop and for generate](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#551-labs-on-for-loop-and-for-generate)<br>

[Contributors](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#contributors)<br>

[Acknowledgement](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#acknowledgement)<br>

[Contact Information](https://github.com/Bandaanusha/RTL-DESIGN-USING-VERILOG-WITH-SKY130-TECHNOLOGY#contact-information)

## 1. Day 1 - Introduction to Verilog RTL design and synthesis
### 1.1. Introduction to open-source simulator iverilog
Simulator is tool used for simulating the design. iverilog is a open source simulator. Simulating Register transfer level (RTL) design checks adherence of RTL design to specifications. 
#### 1.1.1. Introduction iverilog design and test bench
Design is a verilog code intended for particular functionality to meet with the required specifications.TestBench is the setup to apply stimulus to the design to check its functionality. Fig 1 shows working of testbench.

![1](https://user-images.githubusercontent.com/62790565/183249511-3da7501f-e4a4-4fa0-90a3-cf6888604666.jpeg)
<br>Fig 1


<br>Simulator looks for the changes on the input signals, upon changes to the input the output is evaluated. Fig 2 shows iverilog based simulation flow, Applying Design and testbench to iverilog simulator generates value Change Dump (vcd) file indicates that any changes in the input are dumped to output. gtkwave tool is used to view the input and output waveforms.

![2](https://user-images.githubusercontent.com/62790565/183249896-56e0d3bc-885d-40b6-8c9a-a75ccb72ca6a.jpeg)
<br>Fig 2

###  Labs using iverilog and gtkwave
Fig 3 shows terminal window creating a directory VLSI and git clone sky130RTLDesignAndSynthesisWorkshop directory from https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git and walking through files in sky130RTLDesignAndSynthesisWorkshop directory. lib folder consists of all sky130 library cells and verilog_model consits of verilog code for all the standard cells.

![ter](https://user-images.githubusercontent.com/62790565/183941964-075f3385-5c41-4187-a49e-43818fb445db.png)
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
<br>Fig 4

## 1.3. Introduction to Yosys and Logic synthesis
#### 1.3.1 Introduction to yosys
Yosys is a synthesizer, a tool used for converting the RTL to netlist.Fig 5 shows the flow of yosys,applying design and .lib files to yosys we get netlist as output.read_verilog command is used to read the design, read_liberty command to read the .lib file and write_verilog command to write out the netlist file.Netlist is representation of the design in form of cells present in .lib.

![5](https://user-images.githubusercontent.com/62790565/183275983-e5d109b6-a27e-4dc2-ab8b-1d9cacadafb6.jpeg)
<br>Fig 5

<br>Output of simulating by applying netlist and testbench to iverilog and viewing generated vcd file on gtkwave toolshould be same as output of simulating by applying design and testbench to iverilog and viewing generated vcd file on gtkwave provided testbench applied in both the cases should is same, then the sysnthesis is said to be verified.

![6](https://user-images.githubusercontent.com/62790565/183276366-111784a5-b222-4721-90f6-b44a21aa0112.jpeg)
Fig 6

#### 1.3.2 Introduction to logic synthesis
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

### 1.4. Labs using Yosys and SKY130PDK's
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
Fig 9 shows the netlist

![fig9](https://user-images.githubusercontent.com/62790565/183942214-6a99f747-8072-448d-b3d8-749a0ac7ff95.png)
<br>Fig 9

## 2. Day 2-Timing libs, hierarchial vs flat synthesis and efficient flop coding styles
### 2.1. Introduction to timing.libs
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

### 2.2. Hierarchial vs Flat Synthesis
#### 2.2.1. Lab on hierarchial vs flat synthesis part1
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

#### 2.2.2. Lab on hierarchial vs flat synthesis part2
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
### 2.3. Various Flop Coding Styles and optimization
#### 2.3.1. Why Flops and Flop coding styles2.3.

![17](https://user-images.githubusercontent.com/62790565/183291263-1754b75b-1e00-410f-b12a-11c683db9d6b.jpeg)

consider the digital circuit shown in Fig 17, changes in inputs a,b,c are propagated to the output Y with propagation delay with a glitch. If there are more combinatinal circuits output of which is input to the other, there will more glitches in the output makes it unstable. Hence we need flops to store which restricts glitches in output as output changes with clock. Flops are initialized by set and reset inputs. set=1 sets the output to 1 and reset=1 sets the output to 0.
<br> Four types of flop initialization by set and reset inputs
<br> 1.asynchronous reset
<br> 2. synchronous reset
<br> 3. asynchronous set
<br> 4. synchronous set

###2.3.2. Labs on flop synthesis simulations
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

#### 2.3.3. Intresting optimizations
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

![mul2net](https://user-images.githubusercontent.com/62790565/183943265-11e0dd78-b801-42f5-b8fe-661c3facc3b5.png)
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
module mult_8 (input [2:0] a, output [5:0] y);
	assign y = a * 9;
endmodule
```
<br>Synthesized circuit

![mul9s](https://user-images.githubusercontent.com/62790565/183942788-4f50847e-8ba6-41b0-8d5c-0608ceb541e5.png)

<br>Netlist Simulation

![nmul9](https://user-images.githubusercontent.com/62790565/183943161-55af02e4-d4ad-4d39-b5ad-c14c88d0e4b1.png)

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
<br>Consider following illustration of sequential circuit, flip flops B and C are at long ditsance from flip flop A hence there is large delay of reachhing output from A to B and C. If there is huge slack at input of flip flop A then flip flop A can be cloned aas two copies and can be placed near to flip flop B and C. This optimizes the time.

![so2](https://user-images.githubusercontent.com/62790565/183302341-bd2253cb-6ba6-4ac2-80dc-65ca163fa890.jpeg)
Fig 37

<br>Retiming
<br>Consider following illustration of sequential ciruit.Here we can see that the combinatinal circuit between flipflop A & B  and B & C are different. Speed of operation depends on low delay circuit. Hence by retiming if we distribute logic in such a way that both combinational circuits between flip flop A & B and B & C have almotst same delay speed of operation increases and hence performance of the sequential circuit increases.

![so3](https://user-images.githubusercontent.com/62790565/183302348-24f5ecda-5eea-41f8-a548-35869653fdb1.jpeg)
Fig 38

### 3.2 Combinational logic optimizations

<br>Example 1
<br>Code
```
module opt_check (input a , input b , output y);
	assign y = a?b:0;
endmodule

```
<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog opt_check.v
>synth -top opt_check
>opt_clean -purge
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```

<br>Optimized circuit

![o1](https://user-images.githubusercontent.com/62790565/183862125-7921cbd6-d206-4f2f-b4cd-31fd0eaf7d7c.png)
<br>Fig 39

<br>Example 2
<br>Code
```
module opt_check2 (input a , input b , output y);
	assign y = a?1:b;
endmodule

```
<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog opt_check2.v
>synth -top opt_check2
>opt_clean -purge
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Optimized circuit

![o2](https://user-images.githubusercontent.com/62790565/183862455-0ed0cd9c-5e7f-42a0-9d52-88d146d3e217.png)
<br>Fig 40

<br>Example 3
<br>Code
```
module opt_check3 (input a , input b, input c , output y);
	assign y = a?(c?b:0):0;
endmodule
```
<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog opt_check3.v
>synth -top opt_check3
>opt_clean -purge
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Optimized circuit

![o3](https://user-images.githubusercontent.com/62790565/183862935-d1d0001d-f9df-4365-b6fd-20a825b4de50.png)
<br>Fig 41

<br>Example 4
<br>Code
```
module opt_check4 (input a , input b , input c , output y);
	assign y = a?(b?(a & c ):c):(!c);
endmodule
```
<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog opt_check4.v
>synth -top opt_check4
>opt_clean -purge
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Optimized circuit

![o4](https://user-images.githubusercontent.com/62790565/183863676-5847fc4d-a30c-46b8-b4c8-9a5d052f6a6a.png)
<br>Fig 42

<br>Example 5
<br>Code
```
module sub_module(input a , input b , output y);
	assign y = a & b;
endmodule

module multiple_module_opt2(input a , input b , input c , input d , output y);
	wire n1,n2,n3;
	sub_module U1 (.a(a) , .b(1'b0) , .y(n1));
	sub_module U2 (.a(b), .b(c) , .y(n2));
	sub_module U3 (.a(n2), .b(d) , .y(n3));
	sub_module U4 (.a(n3), .b(n1) , .y(y));
endmodule
```
<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog opt_check.v
>synth -top opt_check
>flatten
>opt_clean -purge
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Optimized circuit

![mmo](https://user-images.githubusercontent.com/62790565/183864423-6e2056c5-46a0-4c8e-b6f8-f700116fb888.png)
<br>Fig 43

### 3.3 Sequential logic optimizations
<br>Example 1
<br>Code
```
module dff_const1(input clk, input reset, output reg q);
	always @(posedge clk, posedge reset)
	begin
		if(reset)
			q <= 1'b0;
		else
			q <= 1'b1;
	end
endmodule
```
<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog dff_const1.v
>synth -top dff_const1
>dfflibmap -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Simulated waveforms

![so1](https://user-images.githubusercontent.com/62790565/183865775-ea29aebd-1521-4e4a-9b59-932ec657fa44.png)
<br>Fig 44

<br>Optimized circuit

![soo1](https://user-images.githubusercontent.com/62790565/183866124-e8f556e5-420d-4802-86f8-54c973fbe2d4.png)
<br>Fig 45

<br>Example 2
<br>Code
```
module dff_const2(input clk, input reset, output reg q);
	always @(posedge clk, posedge reset)
	begin
		if(reset)
			q <= 1'b1;
		else
			q <= 1'b1;
	end
endmodule
```
<br>Simulated waveforms

![so2](https://user-images.githubusercontent.com/62790565/183866883-9b399b1b-8fd2-4256-82b9-4cf4319be366.png)
<br>Fig 46

<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog dff_const2.v
>synth -top dff_const2
>dfflibmap -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Optimized circuit

<br>![soo2](https://user-images.githubusercontent.com/62790565/183867774-6acf2986-e0c8-404c-8fc9-64e7230225a6.png)
<br>Fig 47

Example 3
<Code>
```
module dff_const3(input clk, input reset, output reg q);
	reg q1;

	always @(posedge clk, posedge reset)
	begin
		if(reset)
		begin
			q <= 1'b1;
			q1 <= 1'b0;
		end
		else
		begin
			q1 <= 1'b1;
			q <= q1;
		end
	end
	endmodule
```

<br>Simulated waveforms

![so3](https://user-images.githubusercontent.com/62790565/183867649-ddb6aeb4-a52d-4d7c-b2ff-e890740dec8e.png)
<br>Fig 48

<br>Commands for synthesis
```
>read_liberty -lib /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>read_verilog dff_const3.v
>synth -top dff_const3
>dfflibmap -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>abc -liberty /home/anusha/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
>show
```
<br>Optimized circuit

![soo3](https://user-images.githubusercontent.com/62790565/183874123-692be01e-de1c-4d7a-95f7-8d0a76134168.png)
<br>Fig 49

### 3.4. Sequential optimizations for unused outputs
Example 1
<br>Code
```
	module counter_opt (input clk , input reset , output q);
	reg [2:0] count;
	assign q = count[0];
	always @(posedge clk ,posedge reset)
	begin
		if(reset)
			count <= 3'b000;
		else
			count <= count + 1;
	end
	endmodule
```
<br>Optimized circuit

![co](https://user-images.githubusercontent.com/62790565/183869004-469d4e60-cd80-4a73-9181-9db84422e066.png)
<br>Fig 50

## 4. DAY4- GLS, blocking vs non-blocking and Synthesis-Simulation mismatch
### 4.1. GLS, Synthesis-Simulation mismatch and Blocking, Non-blocking statements
#### 4.1.1. GLS Concepts And Flow Using Iverilog
GLS(Gate level Synthesis) is generating the simulation output by running test bench with netlist file generated from synthesis as design under test. Netlist is logically same as RTL code, therefore, same test bench can be used for it.We perform this to verify logical correctness of the design after synthesizing it. Also ensuring the timing of the design is met.
<br>Below picture gives an insight of the procedure. Here while using iverilog, we also include gate level verilog models to generate GLS simulation.

![gls](https://user-images.githubusercontent.com/62790565/183870267-82c8393a-6ec8-462f-bcf7-44d9015262c3.png)
<br>Fig 51

#### 4.1.2 Synthesis Simulation Mismatch
There are three main reasons for Synthesis Simulation Mismatch:
- Missing sensitivity list in always block
- Blocking vs Non-Blocking Assignments
- Non standard Verilog coding

<br>Missing sensitivity list in always block:

<br>If the consider - Example-2, we can see the only sel is mentioned in the sensitivity list. During the simulation, the waveforms will resemble a latched output but the simulation of netlist will not infer this as the synthesizer will only look at the statements with in the procedural block and not the sensitivity list.As the synthesizer doesn't look for sensitivity list and it looks only for the statements in procedural block, it infers correct circuit and if we simulate the netlist code, there will be a synthesis simulation mismatch.
<br>To avoid the synthesis and simulation mismatch. It is very important to check the behaviour of the circuit first and then match it with the expected output seen in simulation and make sure there are no synthesis and simulation mismatches. This is why we use GLS.

#### 4.1.3 Blocking and Non-Blocking statements in verilog
Blocking statements execute the statemetns in the order they are written inside the always block. Non-Blocking statements execute all the RHS and once always block is entered, the values are assigned to LHS. This will give mismatch as sometimes, improper use of blocking statements can create latches.

### Labs on GLS and synthesis-simulation mismatch
Example 1
<br>Code
```
module ternary_operator_mux (input i0 , input i1 , input sel , output y);
	assign y = sel?i1:i0;
endmodule
```
<br>Simulation

![gl1](https://user-images.githubusercontent.com/62790565/183882685-8d7a42eb-236e-4a57-ac3e-8f9f72f6380c.png)
<br>Fig 52

<br>Synthesis

![sgl1](https://user-images.githubusercontent.com/62790565/183882853-9e870804-1ecc-4bc3-a371-198868735af6.png)
<br>Fig 53

<br>Netlist Simulation

![ngl1](https://user-images.githubusercontent.com/62790565/183883505-8db3e0fb-a29b-4392-8e91-6430b151289a.png)
<br>Fig 54

<br>Example 2
<br>Code
```
module bad_mux (input i0 , input i1 , input sel , output reg y);
	always @ (sel)
	begin
		if(sel)
			y <= i1;
		else 
			y <= i0;
	end
endmodule
```
<br>Simulation

![gl2](https://user-images.githubusercontent.com/62790565/183883852-2f4a3ada-0ad3-4ce9-ad15-049d9fb8311e.png)
<br>Fig 55

<br>Netlist Simulation

![ngl2](https://user-images.githubusercontent.com/62790565/183884041-4a0eeda3-1687-4055-a1dd-39c42e5f3b60.png)
<br>Fig 54

<br>Sysnthesis simulation mismatch

![mis1](https://user-images.githubusercontent.com/62790565/183884649-e73d1d6f-fb55-4fd8-a499-f466240b8c52.JPG)
<br>Fig 55

### 4.3. Lab on Synthesis Simulation Mismatch for Blocking Statement
Here the output is depending on the past value of x which is dependednt on a and b and it appears like a flop.
<br>Example 1
<br>Code
```
module blocking_caveat (input a , input b , input  c, output reg d); 
reg x;
always @ (*)
	begin
	d = x & c;
	x = a | b;
end
endmodule
```

<br>Simulation

![bl1](https://user-images.githubusercontent.com/62790565/183885115-83da01a7-55b3-461f-93bc-95c2dab6f069.png)
<br>Fig 56

<br>Netlist simulation

![nbl1](https://user-images.githubusercontent.com/62790565/183885341-a841d833-13a9-4dc2-b12c-833249c8380e.png)
<br>Fig 57

<br>Simulation mismatch

![mis2](https://user-images.githubusercontent.com/62790565/183885550-7a1a87b7-3f10-4b8e-9a26-16f1d3c57ea9.JPG)
<br>Fig 58

## 5. DAY5- if, case, for loop and for generate
### 5.1. If and Case constructs
#### 5.1.1 If construct
The construct if is mainly used to create priority logic. In a nested if else construct, the conditions are given priority from top to bottom. Only if the condition is satisfied, if statement is executed and the compiler comes out of the block. If condition fails, it checks for next condition and so on as shown below.
<br>Syntax for nested if else
```
if (<condition 1>)
begin
-----------
-----------
end
else if (<condition 2>)
begin
-----------
-----------
end
else if (<condition 3>)
.
.
.
```
<br>Dangers with If
<br>If use a bad coding style i.e, using incomplete if else constructs will infer a latch. We definetly don't require an unwanted latch in a combinational circuit. When an incomplete construct is used, if all the conditions are failed, the input is latched to the output and hence we don't get desired output unless we need a latch.

#### 5.1.2. Case construct
In case construct, the execution checks for all the case statements and whichever satisfies the statement, that particular statement is executed.If there is no match, the default statement is executed. But here unlike if construct, the execution doesn't stop once statement is satisfied, but it continues further.
<br>Syntax for case construct
```
case(statement)
  case1: begin
       --------
	 --------
	 end
 case2: begin
	     --------
	 --------
	 end
 default:
 endcase
 ```
<br>Dangers with case
<br>Caveats in case occur due to two reasons. One is incomplete case statements and the other is partial assignments in case statements.
 
### 5.2. Labs on incomplete if
This incomplete if construct forms a connection between i0 and output y i.e, D-latch with input as i1 and i0 will be the enable for it.
<br>Example 1
<br>Code
```
module incomp_if (input i0 , input i1 , input i2 , output reg y);
always @ (*)
begin
	if(i0)
		y <= i1;
end
endmodule	
```
<br>Simulated waveforms

![if1](https://user-images.githubusercontent.com/62790565/183900400-2b804b7e-8b2c-4f5f-9605-1d3e7bb6388c.png)
<br> Fig 59

<br>Synthesis

![sif1](https://user-images.githubusercontent.com/62790565/183900649-10da0138-0d2c-4f69-a84a-6b8b50746fcc.png)
<br>Fig 60

<br>Example 2
The below code is equivalent to two 2:1 mux with i0 and i2 as select lines with i1 and i3 as inputs respectively. Here as well, the output is connected back to input in the form of a latch with an enable input of OR of i0 and i2.	
<br>Code
```
module incomp_if2 (input i0 , input i1 , input i2 , input i3, output reg y);
	always @ (*)
	begin
		if(i0)
			y <= i1;
		else if (i2)
			y <= i3;
	end
endmodule
```
	
<br>Simulation waveforms

![if2](https://user-images.githubusercontent.com/62790565/183901341-18c138eb-0292-43f2-93a5-5dccb07b12f3.png)
<br>Fig	61
	
<br>Synthesis

![sif2](https://user-images.githubusercontent.com/62790565/183901590-03ddbe7a-6b67-4777-a023-4f7a292e61ca.png)
<br>Fig 62

### 5.3 Labs on incomplete overlapping case
<br>Example 1	
<br>This is an example of incomplete case where other two combinations 10 and 11 were not included. This is infer a latch for the multiplexer and connect i2 and i3 with the output.
	
<br>Code
```
module incomp_case (input i0 , input i1 , input i2 , input [1:0] sel, output reg y);
	always @ (*)
	begin
	case(sel)
		2'b00 : y = i0;
		2'b01 : y = i1;
	endcase
	end
endmodule
```	

<Simulaion waveforms>

![case1](https://user-images.githubusercontent.com/62790565/183903890-bb0943d0-1fe0-43bb-a336-583298892729.png)
<br>Fig 63	
	
<Synthesis>

![scase1](https://user-images.githubusercontent.com/62790565/183904074-09eeca19-2760-47e6-80cb-1aa3254660c9.png)
<br>Fig 64
	
<br>Example 2
<br>This is the case of complete case statements as the default case is given. If the actual case statements don't execute, the compiler directly executes the default statements and a latch is not inferred.
<br>Code	
```
module comp_case (input i0 , input i1 , input i2 , input [1:0] sel, output reg y);
always @ (*)
begin
	case(sel)
		2'b00 : y = i0;
		2'b01 : y = i1;
		default : y = i2;
	endcase
end
endmodule
```	
<br>Simulation waaveforms

![case1](https://user-images.githubusercontent.com/62790565/183904578-88cc944a-d882-4e49-a5f0-3a33b0036a41.png)
<br>Fig 65	

<br>Synthesis

![scase2](https://user-images.githubusercontent.com/62790565/183904877-7d8b4ef9-f35f-4284-8ea8-3f994d0e73a7.png
<br>Fig 66

<br>Example 3
<br>In the below example, y is present in all the case statements and it had particular outut for all cases. There no latch is inferred in case of y. When it comes to x, it is not assigned for the input 01, therefore a latch is inferred here.
<br>Code
```
module partial_case_assign (input i0 , input i1 , input i2 , input [1:0] sel, output reg y , output reg x);
always @ (*)
begin
	case(sel)
		2'b00 : begin
			y = i0;
			x = i2;
			end
		2'b01 : y = i1;
		default : begin
	         	  x = i1;
			  y = i2;
		 	 end
	endcase
end
endmodule	
```	
<br>Synthesis

![scase3](https://user-images.githubusercontent.com/62790565/183905565-ed739ad5-f6d7-4565-a23a-e8878538130b.png)
<br>Fig 67

<br>Example 4	
<br>Code
```
module bad_case (input i0 , input i1, input i2, input i3 , input [1:0] sel, output reg y);
always @(*)
begin
	case(sel)
		2'b00: y = i0;
		2'b01: y = i1;
		2'b10: y = i2;
		2'b1?: y = i3;
		//2'b11: y = i3;
	endcase
end
endmodule
	
```
<br>Simulation waveforms

![case4](https://user-images.githubusercontent.com/62790565/183906145-82d47508-8b17-4550-a33d-ef16b80b082b.png)
<br>Fig 68
	
<br>Synthesis

![scase4](https://user-images.githubusercontent.com/62790565/183906269-8c770602-f04c-4c22-ac28-a68e9f04e86a.pn9)
<br>Fig 69

<br>Netlist Simulation

![ncase4](https://user-images.githubusercontent.com/62790565/183906756-d9632ada-88cb-4cf2-b1a4-38f7cdc4ec8d.png)
<br>Fig 70

### 5.4. For Loop and For Generate
For Loop
- For look is used in always block
- It is used for excecuting expressions alone

<br>Generate For loop
- Generate for loop is used for instantaing hardware
- It should be used only outside always block

<br>For loop can be used to generate larger circuits like 256:1 multiplexer or 1-256 demultiplexer where the coding style of smaller mux is not feasible and can have human errors since we would need to include huge number of combinations.

<br>For Generate can be used to instantiate any number of sub modules with in a top module. For example, if we need a 32 bit ripple carry adder, instead of instantiating 32 full adders, we can write a generate for loop and connect the full adders appropriately.	
	
#### 5.4.1. Labs on for loop and for generate
Example 1-Mux using generate
<br>Here for loop is used to design a 4:1 mux. This can also be written using case or if else block, however, for a large size mux, only for loop model is feasible.
<br>Code
```
module mux_for (input i0 , input i1, input i2 , input i3 , input [1:0] sel  , output reg y);
	wire [3:0] i_int;
	assign i_int = {i3,i2,i1,i0};
	integer k;
always @ (*)
	begin
	for(k = 0; k < 4; k=k+1) begin
		if(k == sel)
		y = i_int[k];
		end
	end
endmodule
```
<br>Simulation

![for1](https://user-images.githubusercontent.com/62790565/183915788-23eb8eda-30c8-4c12-87db-f7ab479d8fc0.png)
<br>Fig 71

<br>Synthesis

![sfor1](https://user-images.githubusercontent.com/62790565/183915538-2a48e0d9-d804-424b-974f-4e035011cf73.png)
<br>Fig 72	

<br>Netlist simulation

![nfor1](https://user-images.githubusercontent.com/62790565/183915647-8d801fc6-bfbc-406f-a3c4-97e25cf01ea4.png
<br>Fig 73	

<br>Example 2-Demux using case
<br>Code
```
module demux_case (output o0 , output o1, output o2 , output o3, output o4, output o5, output o6 , output o7 , input [2:0] sel  , input i);
reg [7:0]y_int;
assign {o7,o6,o5,o4,o3,o2,o1,o0} = y_int;
integer k;
always @ (*)
begin
y_int = 8'b0;
case(sel)
	3'b000 : y_int[0] = i;
	3'b001 : y_int[1] = i;
	3'b010 : y_int[2] = i;
	3'b011 : y_int[3] = i;
	3'b100 : y_int[4] = i;
	3'b101 : y_int[5] = i;
	3'b110 : y_int[6] = i;
	3'b111 : y_int[7] = i;
endcase
end
endmodule
```

<br>Simulation

![for2](https://user-images.githubusercontent.com/62790565/183915810-5f2f6f8d-d92d-4f6e-9597-b94b155acd94.png)	
<br>Fig 74

<br>Synthesis

![sfor2](https://user-images.githubusercontent.com/62790565/183915571-85b16122-23fd-4061-aa74-0bd248341e79.png)
<br>Fig 75

<br>Netlist Simulation

![nfor2](https://user-images.githubusercontent.com/62790565/183915741-c5906cab-0a76-4088-8c30-e02a10d7e692.png)
<br>Fig 76

<br>Example 3-Demux using generate	
<br>The code in above example is big and also there is a chance of human error wile writing the code. However, using for loop as shown below, this drawback can be elimiated to a great extent.
<br>Code
```
module demux_generate (output o0 , output o1, output o2 , output o3, output o4, output o5, output o6 , output o7 , input [2:0] sel  , input i);
reg [7:0]y_int;
assign {o7,o6,o5,o4,o3,o2,o1,o0} = y_int;
integer k;
always @ (*)
begin
	y_int = 8'b0;
	for(k = 0; k < 8; k++) begin
		if(k == sel)
		y_int[k] = i;
	end
end
endmodule	
```

<br>Simulation

![for3](https://user-images.githubusercontent.com/62790565/183915829-5006c4e7-e206-4da4-aa9f-2bd75c894514.png)
<br>Fig 77

<br>Synthesis

![sfor3](https://user-images.githubusercontent.com/62790565/183915582-59ef95a8-b82b-400f-8c6c-ca7e28f39b1d.png)
<br>Fig 78

<br>Netlist Simulation

![nfor3](https://user-images.githubusercontent.com/62790565/183915756-d7efe8d6-550c-41b4-89f4-de6fec5c84b3.png)
<br>Fig 79	
	
<br>Example 4-	Ripple carry adder using full adder
<br>In this Ripple carry adder example, unlike instantiating fulladder for 8 times, generate for loop is used to instantiate the fulladder for 7 times and only for first full adder, it is instantiated seperately. Using the same code, just by changing bus sizes and condition of for loop, we can design any required size of ripple carry adder.
<br>Code
```
module rca (input [7:0] num1 , input [7:0] num2 , output [8:0] sum);
wire [7:0] int_sum;
wire [7:0]int_co;

genvar i;
generate
	for (i = 1 ; i < 8; i=i+1) begin
		fa u_fa_1 (.a(num1[i]),.b(num2[i]),.c(int_co[i-1]),.co(int_co[i]),.sum(int_sum[i]));
	end

endgenerate
fa u_fa_0 (.a(num1[0]),.b(num2[0]),.c(1'b0),.co(int_co[0]),.sum(int_sum[0]));


assign sum[7:0] = int_sum;
assign sum[8] = int_co[7];
endmodule

module fa (input a , input b , input c, output co , output sum);
endmodule
```	
<br>Simulation

![for4](https://user-images.githubusercontent.com/62790565/183915843-f9c979d0-b343-4f37-857b-147a23674d7d.png)
<br>Fig 80

<br>Synthesis

![sfor4](https://user-images.githubusercontent.com/62790565/183920788-0a65e949-dd77-4557-855a-bc52935c5c0c.png)
<br>Fig 81

<br>Netlist Simulation

![nfor4](https://user-images.githubusercontent.com/62790565/183920762-84191856-728b-4551-8660-2dfa4422e6da.png) 
<br>Fig 82

## Contributors
- Banda Anusha
- Kunal Ghosh

## Acknowledgement
A well structured workshop for individuals who is aspiring to start their career in VLSI. Heartfelt thanks to the team of VLSI System Design for this wonderful workshop, lots to be learnt and looking forward for more such workshops. Special thanks to??Kunal Ghosh??for helping throughout the workshop and ease for flow.
		
## Contact Information
- Banda Anusha, Post Graduate student, International Institute of Information Technology, Bangalore Banda.Anusha@iiitb.ac.in.
- Kunal Ghosh,Director, VSD Corp. Pvt. Ltd. kunalghosh@gmail.com.		
