# 7.1

a) Find the row reduced form of:

A = [1 5 7 9; 0 4 1 7; 2 -2 11 -3]

The first step of elimination gives us:

=> R3 - 2R1

= [1 5 7 9; 0 4 1 7; 0 -12 -3 -21]

=> R2 * 1/4

= [1 5 7 9; 0 1 1/4 7/4; 0 -12 -3 -21]

=> R1 - 5R2

= [1 0 23/4 1/4; 0 1 1/4 7/4; 0 0 0 0]

= rref(A)

= [1.00000 0.00000 5.75000 0.25000; 0.00000 1.00000 0.25000 1.75000; 0.00000 0.000000 0.000000 0.000000]


b) What is the rank of this matrix?

The rank of A equals the number of pivot columns.

A = m * n = 3 * 4

rank r = 2

And the number of free columns is n - r, then 4 - 2 = 2

c) Find any special solutions to the equation Ax = 0

Set free variable to x3 = 1, x4 = 0,

1 * x1 + 0 * x2 + 23/4 * x3 + 1/4 * x4 = 0

=> 1 * x1 + 23/4 * x3 + 1/4 * x4 = 0

=> 1 * x1 + 23/4 = 0

=> x1 = -23/4

0 * x1 + 1 * x2 + 1/4 * x3 + 4/7 * x4 = 0

=> 1 * x2 + 1/4 * x3 + 4/7 * x4 = 0

=> 1 * x2 + 1/4 = 0

=> x2 = -1/4

So one solutions is [-23/4 -1/4 1 0]

And by setting free variables to x3 = 0 with x4 = 1

x1 = -1/4, x2 = -7/4

So the other solution is [-1/4 -7/4 0 1]

# 7.2

Find A1 and A2 so that rank(A1B) = 1 and rank(A2B) = 0 for B = [1 1;1 1]

A1 = [1 1; 0 0] A2 = [-1 0; -1 0]
