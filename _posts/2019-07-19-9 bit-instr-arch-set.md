---
layout: post
title: 9 Bit Instruction Architeture Set
date: 2019-03-29
project: true
categories: jekyll update
excerpt_separator: <!--more-->
---

### Summary 
The goal of this project is to build a hardware stimulation to solve simple Math problem which 
includes multiplication and long division. 
We desgined a new set of assembly set using the accumulator method that handle the 9 bit instruction.

<!-- ![Assembly Set](/assets/9bitInstructions/assemly-operation.png) -->

We designed the datapath and the control logic of the hardware System Verilog module in a diagram.
SystemVerilog Modules are implemented based the diagram above.
Each module is unit tested individually to ensure that we get the correct output.
Quartus is used to generate the schematic

![DataPath](/assets/9bitInstructions/top-schematic.PNG)

### Technologies and Tools Used
- C++
- GDB
- SystemVerilog
- Quartus Prime Lite
- ModelSim
    
### Github Repo
- [C++ implementation for inverse and division](https://github.com/kinming92/divvy_assembler)
- [Final Code](https://github.com/kinming92/Divvy_FinalProject)

<hr>