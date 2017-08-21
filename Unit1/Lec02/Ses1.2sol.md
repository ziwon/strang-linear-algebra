### 2.1

```
2x + 3y = 5
6x + 15y = 12
```

From the point of vector, let say `Ax = b` which is `Ax` is a combination `b` of the columns of `A`.


`A` is

```
  A = [2 3; 6 15] 
```

`b` is
```
  b = [5; 12]
```

Then, the elimination matrix will be:
```
  E_21 = [1 0; -3 1] 
```
where `l` is -3 in the (2,1) position, as the first pivot to eliminate the second column.

Let's apply `E_21` to this matrix `A`,
```
  U = E_21 * A
```  
Do the same to the right side `b` = (5, 12) that gives a new equation which is `Ux=c`
```
  c = E_21 * b
```  
Therefore, `y` = -(1/2) and `x` = 13/4.

The answer should fulfill the first equation; 
```
  x = [13/4; -1/2]
```
So the result of `A*x` should end up with the same value of 'b':
```
  isequal(A*x, b)
  ans = 1 // Check!
```  

### 2.2
Suppose we have
```
P1 = [1 0 0 0; 1 1 0 0; 1 2 1 0; 1 3 3 1] 
P2 = [1 0 0 0; 0 1 0 0; 0 1 1 0; 0 1 2 1]
```

Then, what kind of `E` that satisfies `E*P1 = P2`?

Let's start with the elimination matrix `E = [ 1 0 0 0; -1 1 0 0; 0 -1 1 0; 0 0 -1 1]`

Then, we get `E_21` which can substract the first column from the second column:

```
E_21 = [1 0 0 0; 0 1 0 0; 0 -1 1 0; 0 0 -1 1]
```

And `E_32` is
```
E_32 = [1 0 0 0; 0 1 0 0; 0 0 1 0; 0 0 -1 1]
```

By producting these matrixes at once like `E32(E21(E))`
```
M = E_32 * E_21 * E
```

So is the same with the inverse matrix of `P1`
```
>> isequal(M, inv(P1))
ans = 1 // Check
```
