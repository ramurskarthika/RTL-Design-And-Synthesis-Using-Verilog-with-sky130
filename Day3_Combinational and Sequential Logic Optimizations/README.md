COMBINATIONAL AND SEQUENTIAL LOGIC OPTIMIZATIONS

**1.Combinational Logic Optimization**
- Went through the following examples designs and synthesized each in Yosys:
- opt_check
 <img width="1280" height="895" alt="1" src="https://github.com/user-attachments/assets/a5f847dc-d724-457e-8d63-c16478969391" />
 <img width="1278" height="890" alt="2" src="https://github.com/user-attachments/assets/ba6da880-4fe2-401f-9311-494dac8628ac" />
- opt_check2
  <img width="1280" height="910" alt="3" src="https://github.com/user-attachments/assets/705d5356-d3fd-480f-9dcc-9b761bdc84e5" />
- opt_check3
   <img width="1277" height="890" alt="4" src="https://github.com/user-attachments/assets/11146aa6-428f-4461-94ae-202250ac4388" />
- opt_check4
  <img width="1275" height="886" alt="5" src="https://github.com/user-attachments/assets/0cb02f84-28ba-4711-9a02-85f41827dcc7" />
- multiple_module_opt
  <img width="1277" height="892" alt="6" src="https://github.com/user-attachments/assets/01be1cfd-ed22-4801-993f-e4d8b7fe1d50" />
- mutliple_module_opt2
  <img width="1282" height="881" alt="7" src="https://github.com/user-attachments/assets/6208bd36-89f4-467f-afa1-0241897f01a7" />
 - The command opt_clean -purge  removes reduntant/unused logic and propagates constants to simplify the circuit to its minimal gate-level form.


   **2. Sequential Logic Optimization**
  - Studied flip-flop based constant optimization and ran simulation to view the waveform behaviour, then synthesis to see how the flop and logic get optimized
  - dff_const1
     <img width="1273" height="885" alt="8" src="https://github.com/user-attachments/assets/7ecafc6b-df69-48d5-a9d5-8664cde58866" />
     <img width="1272" height="890" alt="9" src="https://github.com/user-attachments/assets/27c45ea9-4679-495b-ad6f-db617754a325" />
     <img width="1276" height="890" alt="11" src="https://github.com/user-attachments/assets/d52191b3-e567-447e-8ab6-2b9bf3989810" />
  -dff_const2
     <img width="1282" height="886" alt="10" src="https://github.com/user-attachments/assets/e28fbccc-9d4c-4d14-bc6c-0fba467b1c85" />
     <img width="1280" height="887" alt="12" src="https://github.com/user-attachments/assets/2fb6ed7a-9502-42a6-bb44-d1cb0c6242c6" />
  -dff_const3
     <img width="1277" height="887" alt="13" src="https://github.com/user-attachments/assets/df33e790-2b39-4805-b9e0-0f38f37d3e6e" />
     <img width="1271" height="891" alt="16" src="https://github.com/user-attachments/assets/99500cca-f16d-471c-8551-76a4c2f5571b" />
     <img width="1278" height="878" alt="15" src="https://github.com/user-attachments/assets/d484ba4c-1549-4929-aae2-6b0b3bc7e0c4" />
  -dff_const4
     <img width="1275" height="890" alt="17" src="https://github.com/user-attachments/assets/9644e34d-b48e-4785-a626-f7ef7a243507" />
     <img width="1282" height="888" alt="19" src="https://github.com/user-attachments/assets/eb46f7ed-d531-4982-b42b-5ba27de480d9" />
  -dff_const5
     <img width="1280" height="891" alt="18" src="https://github.com/user-attachments/assets/812c0086-66f1-4d9b-bca3-fc615074e1e7" />
     <img width="1282" height="883" alt="20" src="https://github.com/user-attachments/assets/010c517e-d2cc-4aca-885e-68d98903a004" />


