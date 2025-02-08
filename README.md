# Dart List Index Out of Bounds Bug

This repository demonstrates a common error in Dart: accessing an index beyond the bounds of a list.  The `bug.dart` file contains code that produces this error. The solution, found in `bugSolution.dart`, corrects this issue.

## Bug Description
The `for` loop in `bug.dart` iterates from 0 up to and *including* the length of the list.  Since list indices start at 0, this leads to an attempt to access an index that doesn't exist, resulting in an `RangeError` exception.

## Solution
The corrected code in `bugSolution.dart` fixes the loop condition to iterate only up to (but not including) the length of the list, avoiding the out-of-bounds access.