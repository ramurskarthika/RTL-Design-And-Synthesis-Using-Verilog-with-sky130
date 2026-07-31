**GLS, BLOCKING VS NON-BLOCKING AND SYNTHESIS SIMULATION MISMATCH**
**1. Gate-Level Simulation**
- Simualting  the synthesized gate-level netlist along with gat-level standard cell models, to verify that synthesis has preserved the design's functionality.
- In GLS we provide , The synthesized netlist , Gate-level standard cell models and the testbench, this is run through iverilog, which produces .vcd file for waveform viewing in GTKWave

**Ternary_operator_mux**
<img width="1276" height="882" alt="1" src="https://github.com/user-attachments/assets/42174bfb-4251-44aa-8b69-18877b007df3" />
<img width="1277" height="883" alt="2" src="https://github.com/user-attachments/assets/aca19740-98d3-4a78-a9eb-25b12a86a8be" />
<img width="1276" height="887" alt="3" src="https://github.com/user-attachments/assets/1eb86fb5-84a6-4685-8ca5-d5feeb57a212" />
<img width="1273" height="885" alt="4" src="https://github.com/user-attachments/assets/5a77d150-6dec-4f0b-98fc-ba937ea8450a" />
  
**bad_mux**
<img width="1272" height="887" alt="5" src="https://github.com/user-attachments/assets/2c7cc9c9-360d-4447-b548-b0f31ab63724" />
<img width="1277" height="888" alt="6" src="https://github.com/user-attachments/assets/dd8867ab-dee0-4925-895a-7a5c5ff69c2b" />
<img width="1277" height="881" alt="7" src="https://github.com/user-attachments/assets/40923ecb-5bbf-4e9a-884e-53dc2bb2dc0a" />

 **2.Synthesis and Simulation Mismatch**
 - A mismatch can happen due to three main reasons:
 **1.Missing sensivity list**
   - Using always@(sel) instead of always@(*), causing simulator to not update outputs on all relevant input changes, while the synthsized hardware behaves combinationally regardless.
 **2.Blocking vs Non-Blocking statemtents**
   - = -> blocking statement , <= -> non-blocking statement
   - Using blocking assignments in sequential logic or in a way that creates unintended ordering dependcies, leads to simulation mismatch vs actual synthesized hardware.
  **Non-standard Verilog coding styles**
     -Simulator intrepret one way but synthesis tool infer differently.

  <img width="1281" height="882" alt="8" src="https://github.com/user-attachments/assets/e02364e8-14a1-47c8-b788-2f8222d4d8e8" />
  <img width="1278" height="887" alt="9" src="https://github.com/user-attachments/assets/10c300a5-10b0-42dc-89b2-a46336cc7fcd" />
  <img width="1276" height="887" alt="10" src="https://github.com/user-attachments/assets/b1ec5c93-e8e4-4f0e-98ab-c22d9926a0e5" />
  <img width="1276" height="902" alt="11" src="https://github.com/user-attachments/assets/70626171-1d17-4f5e-8734-715e9c6d4bd1" />


     

