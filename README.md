# VHDL Counter Bug
This repository demonstrates a common off-by-one error in VHDL and its solution.

## Bug Description
The `buggy_counter.vhdl` file contains a counter that might exhibit unexpected behavior.  The counter is intended to count from 0 to 15 and then roll over. However, there's a subtle error in the rollover condition which might cause it to stop prematurely at 15 instead of cycling back to 0.

## Solution
The corrected code is provided in `fixed_counter.vhdl`. This version accurately handles the rollover condition and counts correctly from 0 to 15, then back to 0.

## How to Reproduce
1. Synthesize and simulate both `buggy_counter.vhdl` and `fixed_counter.vhdl` using your preferred VHDL simulator.
2. Observe the behavior of both counters to see the difference in their rollover behavior.