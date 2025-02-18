<heading1> Samsung-Riscv </heading1>
<details>
Samsung Semiconductor India Research, in collaboration with VLSI System Design (VSD), has launched the SAMSUNG-RISCV program. This intensive six-week training program focuses on semiconductor technologies and the RISC-V architecture. Designed to equip participants with advanced knowledge and skills, it aims to meet the demands of the fast-growing semiconductor industry. With a strong emphasis on RISC-V design and its open-source nature, the program provides an excellent opportunity to explore VLSI chip design and innovation in RISC-V technology.

Basic Details
Name : Sai Pranathi R
College : Dayananda Sagar College of Engineering
Email : saipranathirdsce@gmail.com
github : pranathi-212
linkedn : Sai Pranathi R
</details>
<details>
  <summary>Task 1 : The given task is to install RISC V toolchain using VDI link by following the steps mentioned in the shared pdf and compile a simple C program referring the lab video</summary>
This task focuses on setting up a GitHub repository named *samsung-riscv*, installing the RISC-V toolchain, and completing hands-on exercises based on the provided lab videos. The objective is to help participants gain familiarity with the RISC-V architecture, its toolchain, and the process of executing programs written in C and RISC-V.  

## Steps to complete the task
- Watch the reference videos to understand the program workflow.  
- Install the RISC-V toolchain using the provided VDI link.  
- Follow the lab exercises and run them on a local system.  
- Capture dated snapshots of the implementation and upload them to the GitHub repository.

  ### Image
![image alt](https://github.com/user-attachments/assets/06b57407-d9f6-401d-9570-a9cb0e9519b3)
![image alt](https://github.com/user-attachments/assets/a561749f-c288-416f-9ba9-caef6376bde0)
![image alt](https://github.com/user-attachments/assets/44174925-71a2-40e0-a236-24d14e280b03)

</details>

<details>
  <summary>Task 2: This task is to compile a new simple C program and collect the RISC V object dunp using both -O1 and -Ofast</summary>
 This task focuses on SPIKE Simulation, compiler optimizations, and analyzing RISC-V object dumps. The goal is to explore how different compiler optimization levels impact the generated machine code and execution performance.  

## Steps to complete the task
- Watch the SPIKE Simulation reference video to understand the workflow.  
- Conduct simulation experiments using *-O1* and *-Ofast* optimization flags.  
- Write a simple C program as a test case.  
- Compile the program using *RISC-V GCC/SPIKE* with varying optimization levels.  
- Generate and examine the *RISC-V object dumps* for both *-O1* and *-Ofast*.  
- Capture and upload snapshots of the compiled code and object dumps to the GitHub repository.

  ### Image
![image alt](https://github.com/user-attachments/assets/78c346f8-6f94-4417-9f28-0078f875f730)
![image alt](https://github.com/user-attachments/assets/d56b5eb7-58e9-4a7a-9e8e-3e23dbbb3276)
![image alt](https://github.com/user-attachments/assets/dfdb8adb-3d10-44ce-af36-47abeecb3aed)
  

</details>

<details>
  <summary>Task 3: The task is to identify **15 unique RISC V instructions and determine the 32 bit instruction** code</summary>
This task aims to enhance the understanding of RISC-V instruction formats by analyzing and decoding instructions from an application's riscv-objdump output.

## Steps to complete the task
- Study the *RISC-V software documentation* to understand the *R, I, S, B, U, and J* instruction formats.  
- Explore a sample *GitHub repository* to visualize *RISC-V instruction decoding*.  
- Extract *15 unique RISC-V instructions* from the *riscv-objdump* output of the application code.  
- Determine the *32-bit binary representation* of each instruction based on its format.  
- Upload the extracted instruction patterns to the GitHub repository.

### Instruction set
1. I-Type Instructions 
• Size: 12 bits. 
• Placement: Bit positions 20–31. 
• Usage: For arithmetic, logical operations, and memory addressing. 
• Example: addi x5, x6, 10 
o Encodes the immediate value 10 (12 bits) in bits 20–31. 
o Adds 10 to the value in x6 and stores it in x5. 

2. S-Type Instructions 
• Size: 12 bits (split into two parts). 
• Placement: 
o Lower 5 bits (imm[4:0]): Bit positions 7–11. 
o Upper 7 bits (imm[11:5]): Bit positions 25–31. 
• Usage: For memory store instructions like sw. 
• Example: sw x7, 16(x8) 
o Encodes 16 as the immediate value, split across bits 7–11 and 25–31. 

3. B-Type Instructions 
• Size: 12 bits (split across multiple positions). 
• Placement: 
o Bit 11 (imm[11]): Bit position 7. 
o Bits 4–1 (imm[4:1]): Bit positions 8–11. 
o Bits 10–5 (imm[10:5]): Bit positions 25–30. 
o Bit 12 (imm[12]): Bit position 31. 
• Usage: For branch instructions like beq and bne. 
• Example: beq x1, x2, label 
o Encodes the offset to label in the immediate field, split into the specified positions. 

4. U-Type Instructions 
• Size: 20 bits. 
• Placement: Bit positions 12–31. 
• Usage: For instructions like lui (Load Upper Immediate). 
• Example: lui x5, 0x12345 
o Encodes 0x12345 in the upper 20 bits, with the lower 12 bits set to zero. 

5. J-Type Instructions 
• Size: 20 bits (split across multiple positions). 
• Placement: 
o Bit 20 (imm[20]): Bit position 31. 
o Bits 10–1 (imm[10:1]): Bit positions 21–30. 
o Bit 11 (imm[11]): Bit position 20. 
o Bits 19–12 (imm[19:12]): Bit positions 12–19. 
• Usage: For jump instructions like jal. 
• Example: jal x1, label 
o Encodes the offset to label in the immediate field, split into the specified positions.



</details>

<details>
  <summary>Task 4: The task 4 is to perform a functional simulation of the given RISC V Core Verilog netlist and testbench</summary>

The goal of this task is to *simulate a RISC-V Core Verilog netlist* using a testbench to verify its functional correctness by analyzing output signals and waveforms.  

## Steps to complete the task

- Download the required files, including the *Verilog netlist* and *testbench* for the RISC-V Core.  
- Configure the simulation environment using tools like *Icarus Verilog (iverilog)* and *GTKWave*.  
- Execute the *functional simulation*, ensuring the core operates as expected.  
- Monitor and verify the *output signals* to confirm correct execution.  
- Capture and save waveform snapshots to examine the core’s behavior.  
- Upload the simulation results, including waveforms, output logs, and descriptions, to the GitHub repository.

### Image
![image alt](https://github.com/user-attachments/assets/08d944d1-f9f3-420b-8453-a99b81a3b286)
![image alt](https://github.com/user-attachments/assets/69481f98-895b-4028-91d6-2f71f67d9af8)
</details>

<details>
  <summary>Task 5: Blinking the Built-in LED on VSDSquadron Mini   </summary>


## Overview  
In this task, I learned about the VSDSquadron Mini (CH32V003F4U6) board and wrote a simple program to blink the built-in LED.  

## Steps Followed  
1. Set up VS Code with the VSDSquadron toolchain.  
2. Identified that the built-in LED is connected to PC13.  
3. Wrote a C program to toggle the LED with a 500ms delay.  
4. Compiled and uploaded the code

</details>

<details>
  <summary>Task 6 : 7-Segment Display with VSDSquadron Mini   </summary>


##  Overview  
In this task, I connected a 7-segment display to the VSDSquadron Mini (CH32V003F4U6) and programmed it to show the numbers 1, 3, and 7, each for 3 seconds.  

##  Connections  
- VSDSquadron Mini GPIOs are connected to the segments (A-G, DP) of the 7-segment display.  
- A current-limiting resistor (220Ω) is used for each segment.  
- The common cathode is connected to GND.

</details>













