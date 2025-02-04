# VHDL Counter Overflow Bug
This repository demonstrates a common error in VHDL code: an integer counter that can overflow.  The original code (`counter.vhdl`) lacks a mechanism to prevent the counter from exceeding its maximum value (15). The fixed version (`counter_fixed.vhdl`) addresses this issue.

## Bug Description
The `counter.vhdl` file contains a simple counter. However, when the counter reaches its maximum value (15), it wraps around to 0 without any indication or error. This is an unintended behavior that could cause issues in a larger system.

## Solution
The `counter_fixed.vhdl` file shows a corrected version of the counter.  It includes a check to prevent the overflow by stopping at the maximum value. This provides more robust and predictable behavior.
