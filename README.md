# Pipelined-MIPS-Processor
## Introduction:
In this project, I have implemented a 32-bit Pipelined microarchitecture MIPS processor based on Harvard Architecture. The single-cycle microarchitecture executes an entire instruction in one cycle. In other words instruction fetch, instruction decode, execute, write back, and program counter update occurs within a single clock cycle.
## Objective:
Referring to the figure below. I have written the RTL Verilog files for all submodules of the MIPS processor (e.g. Contol Unit, Hazard Unit, Instruction Memory, etc.). Then, implemented the top module of the MIPS processor.
![image](https://user-images.githubusercontent.com/54054905/190707040-33d23e58-b550-4ffd-a6b2-1f81f4dcb104.png)
## Top Module View:
The processor is composed of a datapath, a control unit and a hazard unit. The datapath block consists of instruction memory, register file, ALU, data memory, sign extend, some shifters, some pipline registers and some multiplexers. The control unit is internally composed of the main decoder and the ALU decoder. The hazard unit handles both data and control hazards by Forwarding, Stalling or Flushing. The figure below shows a a result from RTL viewer desgined by Quartus Software for the Pipelined MIPS processor.
![image](https://user-images.githubusercontent.com/54054905/190708797-6e301b1f-0e31-49fd-a6fc-c3d64c0b4959.png)
## Data Path Unit:
![image](https://user-images.githubusercontent.com/54054905/190712569-7377d96f-bd23-4fb2-b230-5a5ade2c67d8.png)
## Control Unit:
![image](https://user-images.githubusercontent.com/54054905/190712685-3123f1be-7539-4faa-8282-5e9d1b7cd292.png)
## Hazard Unit:
![image](https://user-images.githubusercontent.com/54054905/190712782-01fe82e2-ce6a-48a1-990a-5656facf16a0.png)
## Simulation Results:
### Calculating the GCD of Numbers (120 , 180)
![image](https://user-images.githubusercontent.com/54054905/190713781-5ed77d6b-382b-486e-b43f-c7f7b042a6a2.png)
### Calculating the Factorial of 6
![image](https://user-images.githubusercontent.com/54054905/190714226-37282beb-dc18-4ccb-b3bd-a38a45639a8a.png)
### Generating Fibonacci Sequence
![image](https://user-images.githubusercontent.com/54054905/190714718-7d4c74ce-ec75-4689-8cca-a820f7d3da38.png)
