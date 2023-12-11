# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![Screenshot 2023-11-26 172417](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/865dea3a-55c5-4a22-bfc4-34a97347fe81)
![Screenshot 2023-11-26 171915](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/17666a16-00fa-43fd-a8ed-b72b6ef6ada4)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![Screenshot 2023-11-26 171804](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/4724f977-54bb-4e5d-ab5f-cc2e2eb7eb58)

![Screenshot 2023-11-26 171521](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/c4063cb1-3f7b-4076-bdde-3d78610556ae)

4-bit Count Down Counter
### Procedure
/* write all the steps invloved */
![Screenshot 2023-11-26 171402](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/07ad828e-caf8-4c43-bd37-1838ee533f97)

![Screenshot 2023-11-26 171857](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/3643611f-22c2-46a0-9344-6dc2c7132762)


### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/






### RTL LOGIC UP COUNTER AND DOWN COUNTER  









### TIMING DIGRAMS FOR COUNTER  





### TRUTH TABLE 


![th](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/7ee66d71-5b2c-491a-bd8e-47056a31e1b6)

![download](https://github.com/Mohanraj2006/Exp-7-Synchornous-counters-/assets/152195759/bb12ffd1-839a-4314-a1e5-404a2a537453)




### RESULTS 
