OPTIMIZATION IN SYNTHESIS

**1.If-else statements**

-Studied how if-else statements infer combinational vs sequential logic designs.
<img width="1273" height="913" alt="1" src="https://github.com/user-attachments/assets/487eae6a-a603-4a63-a9ca-a8d96c0ffe06" />
-Waveform of incomp_if using GTKWave.
<img width="1276" height="908" alt="2" src="https://github.com/user-attachments/assets/26b0ed7d-5d21-4007-a7fd-eb077eaa7ffc" />
-Synthesis of incomp_if using Yosys.
 <img width="1277" height="908" alt="3" src="https://github.com/user-attachments/assets/818b820b-c02b-412d-bd04-f1d89fc30263" />
 -Waveform of incomp_if2 using GTKWave.
 <img width="1278" height="908" alt="4" src="https://github.com/user-attachments/assets/95c8eee8-1f1b-47dd-9e42-c7179ef467b6" />
 -Synthesis of incomp_if2 using Yosys.
 <img width="1275" height="912" alt="5" src="https://github.com/user-attachments/assets/bb9e0134-c279-4e23-86d5-f4a1645d050f" />
- Synthesized and compared with complete if-else to see the difference in inferred hardware.

**2.Case statements**
  
- Studied various case statements styles and their synthesis implications:

**Incomp_case**
 - missing default causes latch inference, similar to incomplete_if.
- Always include a default case and assign all outputs in every branch to avoid unintended latches.
  <img width="1271" height="907" alt="6" src="https://github.com/user-attachments/assets/2d0eabcc-8bc4-41a2-80b6-e62c18f2891e" />
- Waveform of incomp_case using GTKWave
  <img width="1276" height="907" alt="7" src="https://github.com/user-attachments/assets/d80f1a90-6539-4729-b749-a2e4c902ccff" />
- Synthesis of incomp_case using Yosys
  <img width="1280" height="906" alt="8" src="https://github.com/user-attachments/assets/cb6907d9-d8f2-4298-8346-a11d5e0a3564" />
- Waveform of comp_case using GTKWave
 <img width="1280" height="908" alt="9" src="https://github.com/user-attachments/assets/6c2d5b57-acbe-43d4-91b4-d11d42525c76" />
- Synthesis of comp_case using Yosys
 <img width="1277" height="908" alt="10" src="https://github.com/user-attachments/assets/1908fc82-49c2-47a1-8a99-88b6ffe0efc5" />
- Waveform of partial_case_assign using GTKWave
 <img width="1581" height="912" alt="11" src="https://github.com/user-attachments/assets/4dabf630-9e72-4cfe-9d39-96fa4b18ca59" />
- Synthesis of partial_case_assign using Yosys
<img width="1578" height="907" alt="12" src="https://github.com/user-attachments/assets/c095926f-a00d-403f-9c88-7457c459fd7c" />
-Waveform of bad_case using GTKWave
<img width="1575" height="907" alt="13" src="https://github.com/user-attachments/assets/76acbbc7-ea5f-4538-af00-5304138b9f00" />
-Synthesis of bad_case using Yosys
<img width="1323" height="905" alt="14" src="https://github.com/user-attachments/assets/bf91da38-1895-4f8e-8b73-f9cdb42cad62" />

**3.For loop and vs For Generate**
- 
-  For Loop - used inside always block for behavioral iteration
-  
-  For Generate - used outside procedural blocks to instantiate hardware.

  **Implemented a mux using generate**
-  
   <img width="1327" height="913" alt="1" src="https://github.com/user-attachments/assets/cd7958d5-4095-4686-8894-799b5331742c" />
- Waveform of the implemented mux
  <img width="1327" height="908" alt="2" src="https://github.com/user-attachments/assets/12641f8e-720a-4dcc-9ac0-9cbe9f185a3a" />
- Synthesis using Yosys
  <img width="1322" height="910" alt="3" src="https://github.com/user-attachments/assets/2e3eeeee-152b-41e6-a7e9-79d47102b97e" />

 **Implemented a demux using case**
- 
- <img width="1327" height="913" alt="4" src="https://github.com/user-attachments/assets/1d7f162e-bfbb-4390-b109-beee6eb6ae6e" />
- Waveform of the implemented demux
- <img width="1322" height="907" alt="5" src="https://github.com/user-attachments/assets/1c4ebbd8-deaa-4fcb-b0bc-ad68b673e02b" />
- synthesis using Yosys
- <img width="1326" height="907" alt="7" src="https://github.com/user-attachments/assets/a379aa7f-7ff6-4ddf-b656-f8e9e804a39e" />

 **Implemented a demux using generate**
  
<img width="1327" height="913" alt="4" src="https://github.com/user-attachments/assets/a37e12ea-e9be-4c69-97de-b7af35e28fdb" />
-Waveform of the implemented demux
<img width="1325" height="920" alt="6" src="https://github.com/user-attachments/assets/b5444b14-2285-4bf0-9f64-71f2600ba7aa" />
synthesis using Yosys
<img width="1327" height="913" alt="8" src="https://github.com/user-attachments/assets/52b62ccd-373f-47eb-b142-40e11c3b66ed" />

**Ripple Carry Adder using Full Adder**

  <img width="1330" height="912" alt="9" src="https://github.com/user-attachments/assets/bb492417-5a73-4f82-9dc9-badc99e02319" />
Waveform using GTKWave
<img width="1327" height="912" alt="10" src="https://github.com/user-attachments/assets/dd2a43b8-9e53-40d4-b029-21c4f8757668" />
Synthesis using Yosys
<img width="1331" height="908" alt="11" src="https://github.com/user-attachments/assets/843163bd-caf7-4e74-97ab-ac99e34bdb1d" />

**GLS for Ripple Carry Adder**

<img width="1267" height="792" alt="rca gls" src="https://github.com/user-attachments/assets/21cc6db5-711d-4a41-8072-fd1fbae05d91" />
<img width="1146" height="732" alt="synth rca netlist" src="https://github.com/user-attachments/assets/9df3ca34-7368-40f2-ba3c-314977ba7d88" />

**GLS for Demux case**

<img width="1275" height="790" alt="demux case gls wf" src="https://github.com/user-attachments/assets/ba6d6364-20c1-4ffe-b37b-579fd7589e50" />
<img width="675" height="622" alt="demux case gls" src="https://github.com/user-attachments/assets/d29cc92b-79fa-4fb9-b606-f39401ce8bbe" />

**GLS for Demux generate**

<img width="1275" height="907" alt="demux_gn gls" src="https://github.com/user-attachments/assets/e86776d7-4945-4033-aaa2-43a3f1025232" />
<img width="892" height="891" alt="synth for gls" src="https://github.com/user-attachments/assets/db049d28-780f-44fa-863a-2fe280c406c1" />

  

