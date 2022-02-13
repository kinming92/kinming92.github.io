---
layout: post
title: 9 Bit Instruction Architeture Set
date: 2019-03-29
categories: jekyll update
excerpt_separator: <!--more-->
---

The goal of this project was to build a hardware stimulation to solve simple Math problems which include multiplication and long division. 
We designed a new set of assembly set using the accumulator method that handles the 9 bit instruction.

<!-- ![Assembly Set](/assets/9bitInstructions/assemly-operation.png) -->

We designed the datapath and the control logic of the hardware with System Verilog module.
SystemVerilog Modules were then implemented based on the diagram above.
Each module was unit-tested individually to ensure that we got the correct output.
Quartus was used to generate the schematic.

![DataPath](/assets/9bitInstructions/top-schematic.PNG)

Technologies and Tools Used
- C++
- GDB
- SystemVerilog
- Quartus Prime Lite
- ModelSim
    
Repo
- [C++ implementation for inverse and division](https://github.com/kinming92/divvy_assembler)
- [Final Code](https://github.com/kinming92/Divvy_FinalProject)
