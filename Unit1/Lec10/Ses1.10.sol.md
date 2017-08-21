# 10.1

A is an `m` by `n` matrix of rank `r`. Suppose there are right sides b
for which `Ax = b` has no solution.

a) What are all the inequalities that must be true between `m`, `n`,
and `r`?

b) How do you know that `A^T*y = 0` has solutions other than `y = 0`?


a) The rank `r` of a matrix equals the number of pivots of the matrix. So `r`
<= `m` and `r` <= `n` for A that is `m` by `n` matrix. And `Ax = b` has
no solution means that `b` is not in the column space C(A) which is a
subspace of `R^m`, therefore r < m.

b) Because `N(A^T)` have dimensions `m - r` as the left nullpsace of `A`.

# 10.2

`A^T*y = d` is solvable when d is in which of the four subspaces? The
solution `y` is unique when the (      ) contains only the zero vector

Definitely, it is solvable when `d` is in the row space C(A^T) which is a subspace of
`R^n` as the system is `n` by `m`. Like the null space of A, When the left
null space of A N(A^T) contains only the zero vector, `y` is unique
solution.
