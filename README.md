# Javascript Type Coercion Bug
This repository demonstrates a common but easily overlooked issue in Javascript: type coercion during arithmetic operations.  The bug arises from Javascript's implicit type conversion, where it automatically converts data types during operations leading to unexpected outcomes if not handled carefully. This example showcases how adding numbers and strings leads to string concatenation rather than numerical addition. The solution offers a method to avoid this using explicit type checking.

## How to Reproduce
1. Clone the repository.
2. Run `bug.js`. Observe the unexpected output.
3. Run `bugSolution.js` to see the corrected behavior.

## Bug Explanation
Javascript's loose typing allows operations between different types without throwing errors. In this specific case, the `+` operator behaves differently based on the operands.  If one operand is a string, the other is automatically converted to a string, resulting in string concatenation instead of numerical addition. This leads to unexpected outputs in calculations. 

## Solution
The solution explicitly converts both operands to numbers before the addition. This forces numerical addition and prevents the unexpected concatenation.  Always ensure the correct data types in your calculations to avoid such surprises.