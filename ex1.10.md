# Exercise 1.10

`(f n)` is `(* 2 n)`: "2 times n"

`(g n)` is `(** 2 n)`: "2 raised to the power n"

`(h n)` is `(tetration 2 n)`: Where "tetration" is the thing I
had to look up on wikipedia.
```
(** 2 (** 2 (** 2 ... (** 2 n) ...)))
\                                  /
 ------ n times -------------------
 ```

## Reflection

This seems a bit naughty.
Tetration is not an operation that
most people will have heard of,
and it doesn't really have a well defined mathematical name.
