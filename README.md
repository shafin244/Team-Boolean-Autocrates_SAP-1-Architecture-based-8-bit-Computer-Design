# Team-Boolean-Autocrates_SAP-1-Architecture-based-8-bit-Computer-Design
Design and implement an 8-bit computer based on the architecture of SAP-1 (Simple-As-Possible) using combinational and sequential logic circuits. 
This project requires – 
1. Designing SAP-1 architecture using Proteus simulator as per the specifications.
2. Hardware Implementation of SAP-1 using PCB board(s) with allowable and available ICs.

For phase A of SAP-1, we have 3 modules to construct: 
1. Clock pulse generator. 
2. Program counter. 
3. Input unit and memory address register (MAR). 
Clock pulse generator basically generates clock pulse which is used to run the whole 
computer. Program counter counts from 0 to 15 using binary and sends it to the bus. 
Memory address register takes the counting and outputs it to other modules. We may 
use enable, reset etc as inputs in program counter or memory address register to 
enable or reset their behavior as per our necessity. 

For phase B of Sap-1, we have 2 types of modules to construct.
 1. Register:
 a) Accumulator
 b) B- register
 c) output register
 2. Ram
 Registers are our main part in Sap-1 which stores data and necessary instructions and
 releases it to the corresponding module for processing as per the clock cycle. On the other
 hand, ram holds the data, address, and instructions which will be processed in a structured
 way, unlike registers which store 4 or 8-bit data.

