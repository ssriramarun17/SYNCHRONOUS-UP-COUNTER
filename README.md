### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by:SRIRAM ARUN RegisterNumber:25016000
*/

**RTL LOGIC UP COUNTER**

**TIMING DIAGRAM FOR IP COUNTER**

**TRUTH TABLE**

**RESULTS**
![rtlviewer(i) ex11](https://github.com/user-attachments/assets/852de8b5-5742-4a62-9ec7-4e0858227ae8)
![wavefrom(i) ex11](https://github.com/user-attachments/assets/bc0e623b-3afe-4d9c-8fd7-c5143a0e2a9d)
![rtlviewer (ii) ex 11](https://github.com/user-attachments/assets/ed3d485f-8d06-4c1a-8125-f58805af5346)
![waveform (ii) ex11](https://github.com/user-attachments/assets/f97d3ce8-0dcc-46bd-ad5e-732181a15ef9)




