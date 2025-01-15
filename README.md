# Unexpected Behavior with Implicit Conversion Operators and Arithmetic Operations in C#

This code demonstrates a potential issue with implicit conversion operators in C# when combined with arithmetic operations.  The implicit conversions, while convenient, can sometimes lead to unexpected results that are not immediately obvious.

The `MyClass` example shows how implicit conversion between `MyClass` and `int` can interact unexpectedly with arithmetic. The addition operation in `value2 = obj2 + 5;` might be handled in an unexpected way by the compiler, depending on the specific version and settings.  This can lead to subtle and difficult-to-debug errors. 

The solution shows how explicit type casting can make the behavior more predictable and prevent unexpected results.

## How to Reproduce
1. Compile and run the provided `bug.cs` code.
2. Observe the output of `value2`.  The expected output is 25 but may vary.
3. Compare this with the output of the corrected code in `bugSolution.cs`.
