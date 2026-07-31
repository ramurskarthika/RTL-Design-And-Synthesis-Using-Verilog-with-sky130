Day 2 : TIMING LIBRARIES AND HIERARCHIAL Vs FLAT SYNTHESIS

**1.Hierarchieal Synthesis**
- Used the multiple_modules verilog file to study hierarchieal design.

- Ran Yosys synthesis on multiple_modules and obsereved the hierarcieal netlist,where sub-module instances remain separately identifiable, by this we can inspect the design at the sub-module level rather than one flattend file.

- This shows how each sub-module's logic is synthesized and mapped independtly.
<img width="1541" height="847" alt="1" src="https://github.com/user-attachments/assets/a53330bc-dddc-4012-ad40-18f1fee7b94b" />

<img width="1537" height="837" alt="3" src="https://github.com/user-attachments/assets/caa97969-c20d-478d-94e7-0d569f9718c1" />

**2.Flat synthesis**

-Used the flatten command to collapse the hierarchy into single level netilst.

-After flattening ,sub modules dissappera, all logic merges into one flat netlist, useful for cross-module optimization.
<img width="1537" height="836" alt="2" src="https://github.com/user-attachments/assets/ca3f1626-6416-4601-972c-fd43a9809899" />


**3.Why Flip-Flops in design**
- We need Flip-Flops in design in order to avoid glitches propagating through combinational logic and to hold stable output between clock edges.

**4.Synthesis and Simulation of D Flip-flops**
- Performed simulation and synthesis of D Flip-Flops with asynchronous reset/set , sycnhronous behaviour.
- Waveform of D Flip-Flop asynchronous using GTKWave
 <img width="1280" height="886" alt="4" src="https://github.com/user-attachments/assets/fb8f1e1c-5c39-4d85-a720-cd052f162cf4" />
- Waveform of D Flip-Flop asynchronous set using GTKWave
 <img width="1278" height="892" alt="5" src="https://github.com/user-attachments/assets/598e6810-3b4c-4ecb-aae6-40df63769b96" />
-Waveform of D Flip-Flop sychronous using GTKWave
<img width="1278" height="885" alt="6" src="https://github.com/user-attachments/assets/e0b95705-dd95-461a-9452-62546993b18c" />
-D Flip-Flop assynchronous synthesis using yosys
<img width="1276" height="892" alt="7" src="https://github.com/user-attachments/assets/cae8ee27-1b4f-4adf-82c9-b8676727622c" />
-D Flip-Flop assynchronous set synthesis using yosys
<img width="1280" height="887" alt="8" src="https://github.com/user-attachments/assets/e2dd2ab9-d3b4-4e7e-a4ba-ea0d26ce2506" />
-D Flip-Flop synchronous synthesis using yosys
<img width="1277" height="888" alt="9" src="https://github.com/user-attachments/assets/2d24f827-5108-4ede-9993-845e198f8a91" />

**5.Multiplier Optimization**
- Synthesized mult_2, mult_8 modules to observe how multiplication by powers of 2 gets optimized during synthesis
<img width="1278" height="888" alt="10" src="https://github.com/user-attachments/assets/4de581d7-f07d-49d4-98f8-f508173fcd41" />
<img width="1272" height="891" alt="12" src="https://github.com/user-attachments/assets/85fcf120-04fd-42de-af2b-6e6c82e82a91" />
<img width="1272" height="886" alt="11" src="https://github.com/user-attachments/assets/1bdb8e19-82f4-4e45-af43-f082cc568361" />


  
