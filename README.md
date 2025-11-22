# Traffic Light Controller (Verilog HDL)
This project implements a traffic light controller using Verilog HDL.  
The design is based on a 6-state finite state machine (FSM) that controls
four different light outputs: M1, M2, MT, and S. Each state represents a
different traffic phase with specific timing requirements.

The repository includes:
- Verilog RTL design 
- Testbench 
- waveform 

## Design Overview

The controller cycles through six states (S1–S6).  
Each state runs for a fixed number of clock cycles:

- S1 → 7 seconds  
- S2 → 2 seconds  
- S3 → 5 seconds  
- S4 → 2 seconds  
- S5 → 3 seconds  
- S6 → 2 seconds  

For each state, the module drives four sets of 3-bit traffic lights:
- light_M1
- light_M2
- light_MT
- light_S

Each light uses:
- 3'b100 → RED  
- 3'b010 → YELLOW  
- 3'b001 → GREEN  

## Simulation Waveform
![Waveform](images/Screenshot%20(230).png)
