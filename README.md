# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement  D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**D Flip-Flop**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

**Procedure**

/*Step 1: Open Quartus II in your laptop.

Step 2: Write code to implement SR flipflop using verilog and validating their functionality using their functional tables.

Step 3: Run compilation to check for errors.

Step 4: Open waveform output and load input values.

Step 5: Run simulation to get the output.

Step 6: Open in RTL viewers to get RTL diagram output.*/

**PROGRAM**
```
/* Program for flipflops and verify its truth table in quartus using Verilog programming. 
Developed by: M SATHYANARAYANAN
RegisterNumber: 212224040300

module D_FF(D,Clock,reset,Q);
input D,Clock,reset;
output reg Q;
always @ (negedge Clock)
if(!reset)
     Q <= 0;
	else
      Q <= D;	
 endmodule
*/
```
### RTL LOGIC FOR FLIPFLOPS

![Screenshot 2024-04-29 203528](https://github.com/23005672/D-FLIPDLOP-NEGEDGE/assets/138971519/665d8353-07b5-4268-92ae-53564c774be6)


### TIMING DIGRAMS FOR FLIP FLOPS

![Screenshot 2024-04-23 102206](https://github.com/23005672/D-FLIPDLOP-NEGEDGE/assets/138971519/1014a727-4453-4594-a441-aa99fb61f2a5)


### RESULTS:

Thus the D flipflop using verilog and validating their functionality using their functional tables was implemented.
