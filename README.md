# Incorrect Array Access in Ada Loop
This example demonstrates a common error in Ada when working with arrays: incorrect access to array elements within a loop.  The original code attempts to use the array variable name directly in a conditional statement instead of accessing the specific element using the index.  The solution shows the correct way to access and process array elements.

## Bug
The bug lies in the `if` condition inside the loop.  The code attempts to directly compare `My_Arr` (the array itself) rather than accessing individual elements `My_Arr(I)`.

## Solution
The solution involves accessing individual array elements using the loop counter `I` as the index (i.e., `My_Arr(I)`). This corrects the array access, ensuring that the code compares individual integer values against 5.