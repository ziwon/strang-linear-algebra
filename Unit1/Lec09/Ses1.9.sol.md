# 9.1

Find the largest possible number of independent vectors among:

v1 = [ 1; -1;  0;  0],
v2 = [ 1;  0; -1;  0],
v3 = [ 1;  0;  0; -1],
v4 = [ 0;  1; -1;  0],
v5 = [ 0;  1;  0; -1],
v6 = [ 0;  0;  1; -1]

    A =  [1 1 1 0 0 0; -1 0 0 1 1 0; 0 -1 -0 -1 0 1; 0 0 -1 0 -1 -1]

      => [1 1 1 0 0 0; -1 0 0 1 1 0; 0 -1 0 -1 0 1; 0 0 -1 0 -1 -1]

      => [1 1 1 0 0 0; 0 1 1 1 1 0; 0 -1 0 -1 0 1; 0 0 -1 0 -1 -1]

      => [1 1 1 0 0 0; 0 1 1 1 1 0; 0 0 1 0 1 1; 0 0 0 0 0 0]

There are 3 pivots, therefore the largest number of independent vectors
is 3.

# 9.2

Find a basis for the plane x -2y + 3z = 0 in R^3. Then find a basis for
the intersection of that plane with the xy plane. Then find a basis for
all vectors perpendicular to the plane.

    A = [1 -2 3; 0 0 0; 0 0 0]

To find a basis, Set Ax = 0 as the nullspace of the matrix:

    Ax = [-1 2 3; 0 0 0; 0 0 0] * [x1 x2 x3] = [0 0 0]

Then the special solutions is:

    v1 = [2; 1; 0] with x2 = 1, x3 = 0,
    v2 = [-3; 0 1] with x2 = 0, x3 = 1

The intersection of the plane is a line, since v1 with x = 2 and y = 1 is
lies in xy plane, the basis is v1.


To find a basic for all vectors perpendicular to the plane is to find
the cross product of vectors:

    v1 x v2 = [1 - 0;0 - 2; 0 -(-3)] = [1; -2; 3]
