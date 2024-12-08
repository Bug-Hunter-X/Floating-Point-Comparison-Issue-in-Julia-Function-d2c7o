# Floating-Point Comparison Issue in Julia
This repository demonstrates a potential issue with floating-point comparisons in Julia. The `myfunction` function aims to calculate the square of a number, handling positive, zero, and negative inputs correctly. However, due to the nature of floating-point numbers, comparisons can sometimes produce unexpected results. 

The `bug.jl` file contains the original code with the potential issue, while `bugSolution.jl` offers a solution to mitigate the problem.

## Problem Description:
Floating-point numbers are not always represented exactly in computers. This can lead to inaccuracies when comparing floating-point numbers directly, as in the `elseif x == 0` condition. The solution addresses this issue by using an appropriate tolerance to compare floating-point numbers instead of direct equality.