# Uninitialized Signal in VHDL

This repository demonstrates a common error in VHDL: uninitialized signals.  Uninitialized signals can lead to unpredictable behavior and simulation results that differ from actual hardware implementation.

The `bug.vhdl` file contains the erroneous code. The `bugSolution.vhdl` file provides the corrected code.

## Problem

The signal `internal_reg` in the original code is declared but not initialized.  Its initial value is undefined, leading to unpredictable results during simulation and synthesis.

## Solution

The solution initializes `internal_reg` to a known value (all 0s in this example). This ensures predictable and consistent behavior.

## How to reproduce

1.  Clone this repository.
2.  Simulate `bug.vhdl` to observe the unpredictable behavior of the uninitialized signal.
3.  Simulate `bugSolution.vhdl` to see the corrected behavior with the properly initialized signal.

This example highlights the importance of initializing all signals in VHDL to avoid potential issues.