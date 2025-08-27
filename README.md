# Team-Boolean-Autocrates_SAP-1-Architecture-based-8-bit-Computer-Design
Design and implement an 8-bit computer based on the architecture of SAP-1 (Simple-As-Possible) using combinational and sequential logic circuits. 
This project requires – 
1. Designing SAP-1 architecture using Proteus simulator as per the specifications.
2. Hardware Implementation of SAP-1 using PCB board(s) with allowable and available ICs.

<img width="1659" height="1226" alt="BOOLEAN AUTOCRATS_SAP 1_FINAL" src="https://github.com/user-attachments/assets/9030f3e2-5b43-4337-8171-bc38820260f1" />

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

For phase C of Sap-1, we have 2 modules to construct: the Controller/Sequencer and the Instruction Register. 

The Instruction Register is responsible for holding the fetched instruction from memory by separating it into two parts — the opcode and the operand. The opcode is used to identify the type of operation to be performed, while the operand provides the data address or value needed for that operation.

On the other hand, the Controller/Sequencer generates the required control signals step by step with each clock pulse (T-states), ensuring that all modules such as the program counter, memory, registers, and ALU work in proper order. Together, these two modules allow the system to fetch, decode, and execute instructions, completing the full operational cycle of the SAP-1 computer.

For phase D of Sap-1, we have 1 main module to construct: the Arithmetic Logic Unit (ALU). 
The ALU is the heart of the SAP-1 architecture as it carries out the actual arithmetic operations required by the instructions. In our design, the ALU is simple and limited to two operations — addition and subtraction — which are sufficient for demonstrating the working principle of the computer. 

The ALU receives one input directly from the Accumulator and the other from the B-register, and based on the control signal (`SU` for subtract or default for addition), it performs the required operation. The output of the ALU can then be placed back on the data bus and stored into the Accumulator or sent to the Output Register depending on the instruction sequence. Architecturally, the ALU works in synchronization with the Controller/Sequencer, ensuring that the right operation is performed at the right clock cycle. Although minimal, this ALU design demonstrates the basic computational capability of SAP-1 and serves as the processing engine around which the rest of the modules function.

