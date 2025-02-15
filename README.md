# Python: Incorrect Average Calculation for Edge Cases

This repository demonstrates a subtle bug in a Python function designed to calculate the average of a list of numbers. The bug surfaces when handling edge cases: empty lists and lists containing only zeros.

## Bug Description
The `calculate_average` function doesn't properly handle empty lists or lists consisting only of zeros, leading to incorrect results or errors.  The original code returns 0 for an empty list, which might be misleading. For lists containing only zeros, the average should be zero, but a naive sum/count calculation may not reflect this correctly.

## Solution
The improved `calculate_average` function now explicitly checks for an empty list, returning 0.  More importantly, a more robust check is included to handle lists containing only zero values, preventing division by zero errors and ensuring a correct return of zero.