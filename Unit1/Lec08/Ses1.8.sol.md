# 8.1

Explain why these are all false:

a) The complete solution is any linear combination of Xp and Xn.

Any linear combination would be any combination of Xp and Xn using
addition and scala multiplications. But only Xn can have any
coefficents.

b) The system Ax = b has at the most one particular solution.

is that so?

c) If A is invertiable there is no solution Xn in the nullspace.

If A is invertiable, it means that A has full row and column rank and R
is the identity matrix. Even in case of this, Xn exists as a zero dimension
which means Xn = 0

# 8.2

U = [1 2 3 ; 0 0 4] and c = [5; 8]


from [U 0] to [R 0]:

 => [1 2 3 0 ; 0 0 4 0]

 => R2/4 => [1 2 3 0 ; 0 0 1 0]

 => R1 - 3R2 => [1 2 0 0 ; 0 0 1 0] <= [R 0]

solve Rx = 0:

 [1 2 0 ; 0 0 1] * [x1; x2; x3] = [0 ; 0]

 => [x1 + 2 * x2 = 0 ; x3 = 0]

therefore, x = [1; -1/2; 0] where x2 = -1/2 as a free variable

check the answer:

 [1 2 3 ; 0 0 4] * [1; -1/2; 0] = [0 ; 0]


from [U c] to [R d]

 => [1 2 3 5 ; 0 0 4 8]

 => R2/4 => [1 2 3 0 ; 0 0 1 2]

 => R1 - 3R2 => [1 2 0 -1 ; 0 0 1 2] <= [R d]

solve Rx = d,

 [1 2 0 ; 0 0 1] * [x1; x2; x3] = [-1 ; 2]

 => [x1 + 2 * x2 = -1 ; x3 = 2]

therefore, x = [-1; 0; 2] where x2 = 0 as a free variable

check the answer:

 [1 2 3; 0 0 4] * [-1; 0; 2] = [5 ; 8]


# 8.3

Is is true that A = C if Ax = b and Cx = b?

True, because Ax = Cx = b
