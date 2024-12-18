# TypeScript Type Coercion Leading to NaN
This example demonstrates a potential pitfall in TypeScript: type coercion during addition can lead to unexpected NaN results without explicit compiler errors.

The `add` function is declared to accept two numbers and return a number. However, it silently coerces the string "2" to a number when passed as an argument, resulting in NaN.

The solution involves adding type guards or stricter type checking to prevent this behavior.