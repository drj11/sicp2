# Exercise 1.7

Small numbers are problematic because the `good-enough?` test
uses an absolute difference that will be large compared to the
exact answer, thus, accuracy in the result will be destroyed.

For example, the square root of 0.0001 is 0.01.
Consider that the number 0.02 will pass the `good-enough?` test, 
but its square is 0.0004. None of the digits are correct.

For large numbers the problem can be that the best square root
(given the limited precision) may have a square that is more
than 0.001 away from the radicand. `sqrt-iter` will never
terminate.

For example, consider the radicand 8.11296384146067e+31
In 64 bit doubles the best square root is 9007199254740992.0
The square of this number is 8.112963841460668e+31.
Which differs from the radicand by 1.8014398509481984e+16.
It will never be `good-enough?`.

## Reflection

I had to do my experiments in Python because the Chicken Scheme
interpreter does not print floating point values to full
precision.
