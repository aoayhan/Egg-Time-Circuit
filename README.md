# Egg-Timer-Circuit
Egg Timer Logic Circuit and Verilog Code

To start the egg timer, RST button should be pressed first. After pressing RST, we can flip the switches to set the timer as we want and when we press PRESET, we load the time on to our counter. Frequency of the clock is 1000 hz or 1 khz. Max time possible for the counter is 99 minutes 59 seconds.
Downcounter gets the 4-input load we choose and transfers that to the 7 segment display. We created the downwards counter using nested if and else commands.
Controller circuit allows us to use the inputs however we want. The program has 3 states 0,1 and 2. 0’th state is when RST and PRESET are pressed and the downcounter loads and the program proceeds to state 1. At state 1 the downcounter begins counting and goes to state 2. At the final state, if we press RST during the down-counting, 7 segment display shows 0. And if the counter finishes naturally, it gets ready for another input and goes back to state 0.
