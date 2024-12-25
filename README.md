# Julia Function Bug: Unexpected Results with Negative Inputs

This repository demonstrates a common error in Julia involving operator precedence that leads to unexpected function behavior when handling negative inputs.

The `bug.jl` file contains a function with a flaw in its handling of negative numbers due to the way the `-` operator is interpreted in the `else` block.  The `bugSolution.jl` file provides a corrected version. 

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `bug.jl` using the Julia REPL.  Note the incorrect output for negative inputs.
4. Run `bugSolution.jl` to observe the correct output.

## Solution

The issue is resolved by explicitly using parentheses to control the order of operations. This ensures the squaring operation is performed before the negation.