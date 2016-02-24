# Exercise 1.6

The `if` is to eager. `sqrt-iter` never terminates because every
call will invoke another call when `new-if` is invoked:
`(sqrt-iter (improve guess x) x)`. Eventually, because this is
not an iterative process, but a recursive process, any real
implementation will run out of memory.

I think Alyssa's delight will quickly evaporate.
