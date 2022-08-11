# IIITB_Car_Parking_System -> Car parking system using Verilog

A car parking system using Verilog. A sensor is
triggered and gate opens if the the correct password is entered
else the gate remains locked. Unless the correct password is
entered, the exit door will not allowed incoming cars to enter.

# Introduction

![Verilog_code_For_Car_parking_system](https://user-images.githubusercontent.com/74352735/184111740-1fae9489-2635-40b6-881e-fe1c09dd469c.jpg)
The state diagram above explains the entire car parking
system. A sensor detects whether a vehicle is coming or not.
Upon being triggered, the gate opens if the correct password
is entered else the gate remains locked.

# About iverilog
Icarus Verilog is an implementation of the Verilog hardware description language.

# About GTKWave
GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing

# Installing iverilog and GTKWave
 ## For Ubuntu
 Open your terminal and type the following to install iverilog and GTKWave
 
 ```
$   sudo apt-get update
$   sudo apt-get install iverilog gtkwave
```


### Functional Simulation
To clone the Repository and download the Netlist files for Simulation, enter the following commands in your terminal.
```
$   sudo apt install -y git
$   git clone https://github.com/nasty-little-hobbitses/IIITB_Car_Parking_System
$   cd IIITB_Car_Parking_System
$   iverilog iiitb_parking_system.v iiitb_tb_parking_system.v
$   ./a.out
$   gtkwave pcs.vcd
```
## synthesis of verilog code

#### About Yosys
Yosys is a framework for Verilog RTL synthesis. It currently has extensive Verilog-2005 support and provides a basic set of synthesis algorithms for various application domains.

- more at https://yosyshq.net/yosys/

To install yosys follow the instructions in  this github repository

https://github.com/YosysHQ/yosys

- note: Identify the .lib file path in cloned folder and change the path in highlighted text to indentified path

<img width="1119" alt="image" src="https://user-images.githubusercontent.com/110079648/182905357-064fec34-3c2b-4997-a0b7-30453f505ddd.png">



#### to synthesize
```
$   yosys
$   yosys>    script yosys_run.sh
```

#### to see diffarent types of cells after synthesys
```
$   yosys>    stat
```
#### to generate schematics
```
$   yosys>    show
```


## Contributors 

- **Sanampudi Gopala Krishna Reddy** 
- **Kunal Ghosh** 



## Acknowledgments


- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd.

## Contact Information

- Sanampudi Gopala Krishna Reddy, Postgraduate Student, International Institute of Information Technology, Bangalore  svgkr7@gmail.com
- Kunal Ghosh, Director, VSD Corp. Pvt. Ltd. kunalghosh@gmail.com

## References:
- FPGA4Student
 https://www.fpga4student.com/2016/11/verilog-code-for-parking-system-using.html
