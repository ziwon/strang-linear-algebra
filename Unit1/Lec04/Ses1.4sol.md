# 4.1
What is E and A = LU?

From Gauss elimitation method, we can get each of these

E21 = [1 0 0; -2 1 0; 0 0 1]

E31 = [1 0 0; 0 1 0; -2 0 1]

E32 = [1 0 0; 0 1 0; 0 -3 1]

To find out E, mutitply all of elimitation

E32 * E31 * E21 = [1 0 0; -2 1 0; 4 -3 1] = E

And upper bound matrix U is E * A,

U = [1 3 0; 0 -2 0; 0 0 1]

To find out E^-1 which is lower bound matrix, just use E*E^-1 = I

E^-1 = E21^-1 * E31^-1 * E32^-1

Therefore E^-1 = [1 0 0; 2 1 0; 2 3 1] = L

Therefore A = LU = [1 0 0; 2 1 0; 2 3 1] * [1 3 0; 0 -2 0; 0 0 1]

# 4. 2

Find four conditions on a, b, c, d to get A = LU with four pivots.

From R2 = R2 - R1, R3 = R3 - R1, R4 = R4 - R1

A = [ a a a a; 0 b-a b-a b-a; 0 b-a c-a c-a; 0 b-a c-a d-a]

From R3 = R3 - R2, R4 = R4 - R2

A = [ a a a a; 0 b-a b-a b-a; 0 0 c-b c-b; 0 0 c-b d-b]

From R4 = R4 - R3

A = [ a a a a; 0 b-a b-a b-a; 0 0 c-b c-b; 0 0 0 d-c] = U

From LU = I,

Therefore L = [1 0 0 0; 1 1 0 0; 1 1 1 0; 1 1 1 1]

So a != 0, b != a, c != b, d != c.
