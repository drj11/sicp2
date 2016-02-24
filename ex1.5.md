# Exercise 1.5

In applicative order the `(p)` subexpression in `(test 0 (p))`
will get evaluated. This will not terminate.

In normal order the `(p)` subexpression will only get evaluated
if the "when false" part of the if gets selected, which it does
not in the call `(test 0 (p))`. So the result will be `0`.

## Reflection

The computation might just be proceeding very slowly. How can
we tell if the computation is merely very very slow, or if it
will not terminate?
