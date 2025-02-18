Samsung-riscv
The program focuses on the RISC-V architecture and leverages open-source tools to educate participants about VLSI chip design and RISC-V. The internship is led by Kunal Ghosh Sir.

Basic Details
Name: Sai Pranathi R

College: Dayananda Sagar College Of Engineering 

Email ID: saipranathirdsce@gmail.com

GitHub Profile: pranathi-212

LinkedIN Profile: https://www.linkedin.com/in/pranathi-r-031415253?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app

Task 1:
I have successfully completed all the steps for the task 1. I created the GitHub repository named "samsung-riscv" and documented the entire process. The RISC-V toolchain was installed, and the C code for summing numbers was compiled and executed using both GCC and RISC-V GCC. The assembly code was generated using riscv64-unknown-elf-objdump and analyzed. All snapshots with date/time were captured and uploaded to the repository along with detailed documentation.

Task 2:
 I watched the SPIKE simulation video and observed how the performance changes with the -O1 and -Ofast compiler optimization flags. After that, I wrote a simple calculator program in C that performs basic arithmetic operations. Then I compiled this program using both the regular GCC compiler and the RISC-V GCC compiler. Then, I generated the RISC-V object dumps for both -O1 and -Ofast format. Finally, I used SPIKE to see the output of the RISC-V Assembly code and performed debug to analyze the RISC-V object dumps for both optimization levels (-O1 and -Ofast) to compare the differences in the generated assembly code and see how the optimizations affected the program’s performance.

Task 3:
Review the RISC-V software documentation to understand the R, I, S, B, U, and J instruction types. Then, from the riscv-objdump output of your application code, identify 15 unique RISC-V instructions and determine their exact 32-bit instruction codes in the respective formats.

Task 4:
Functional Simulation of RISC-V Core
Perform a functional simulation of the RISC-V Core by downloading the Verilog netlist and testbench files. Set up a simulation environment using tools like Icarus Verilog (iverilog) and GTKWave, and run the simulation to verify the functional correctness by analyzing the output signals.

Task 5:
Blinking the Built-in LED on VSDSquadron Mini  

In this task, I learned about the VSDSquadron Mini (CH32V003F4U6) board and wrote a simple program to blink the built-in LED.  
 
1. Set up VS Code with the VSDSquadron toolchain.  
2. Identified that the built-in LED is connected to PC13.  
3. Wrote a C program to toggle the LED with a 500ms delay.  
4. Compiled and uploaded the code

Task 6:
 7-Segment Display with VSDSquadron Mini  
 
In this task, I connected a 7-segment display to the VSDSquadron Mini (CH32V003F4U6) and programmed it to show the numbers 1, 3, and 7, each for 3 seconds.  

## 🔧 Connections  
- VSDSquadron Mini GPIOs are connected to the segments (A-G, DP) of the 7-segment display.  
- A current-limiting resistor (220Ω) is used for each segment.  
- The common cathode is connected to GND.
