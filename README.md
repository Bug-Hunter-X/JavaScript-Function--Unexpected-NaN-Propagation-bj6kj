# JavaScript Function: Unexpected NaN Propagation

This repository demonstrates a subtle bug in a JavaScript function that involves the unexpected propagation of NaN values. The function is designed to handle null values gracefully, but it fails to address NaN inputs, resulting in an incorrect output.  The solution provides a corrected version of the function that handles both null and NaN values appropriately.

## Bug Description
The original function `foo` correctly handles null inputs by returning 0. However, when either input is NaN, the addition operation results in NaN, which is then returned by the function.  This is unexpected behavior if the intent is to always return a numerical value (e.g., 0) in the case of invalid inputs.

## Solution
The solution involves adding a check to explicitly handle NaN values in addition to null values. This ensures that the function behaves consistently and returns a predictable result in all scenarios.
