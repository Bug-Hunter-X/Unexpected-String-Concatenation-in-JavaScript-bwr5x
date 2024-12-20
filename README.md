# Unexpected String Concatenation in JavaScript

This repository demonstrates a common JavaScript bug caused by the language's loose typing system.  When adding numbers, if one operand is a string, JavaScript performs string concatenation rather than numerical addition.  This can lead to unexpected results and is a source of errors in many JavaScript applications. 

## Bug
The provided `bug.js` file contains a function `foo` that attempts to add two numbers. However, if one of the inputs is a string, the function returns a string concatenation instead of the expected numerical sum.  This is a classic example of type coercion issues in JavaScript.

## Solution
The `bugSolution.js` file offers a fix for this issue by explicitly converting both inputs to numbers before performing addition. This ensures that the addition is performed numerically regardless of the input types, resulting in the correct output.  Always validate and type-check your inputs to avoid unexpected behavior from loose typing.