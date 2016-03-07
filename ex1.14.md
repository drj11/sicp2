# Exercise 1.14

For 1 coin the time is linear
(each step subtracts an amount from the total)

For k coins the time is
whatever the order (in `n`) of (k-1) coins is,
times `n`
(because there are O(n) steps where we solve the k-1 coin problem).
So that's O(n^k)

Space used is simply how many coins we use. So that's O(n).
