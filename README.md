# Hack Constant Folding Bug

This repository demonstrates a subtle bug in the Hack type system related to the lack of constant folding during compilation.  The bug leads to unexpected results in simple arithmetic operations involving function calls.

## Bug Description

The Hack compiler does not perform constant folding, resulting in intermediate calculations not being optimized.  This can lead to discrepancies between the expected and actual results.

## How to Reproduce

1. Clone this repository.
2. Compile and run `bug.hh`.
3. Observe the unexpected output.

## Solution

The `bugSolution.hh` file demonstrates that this isn't an issue with the compiler, but rather a lack of constant folding which could be a feature request or could be worked around with additional pre-compilation processing.