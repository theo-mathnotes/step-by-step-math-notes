# Systems of linear equations

A two-equation, two-unknown linear system can be solved by substitution or by elimination. Both methods are valid; use whichever makes the arithmetic lighter. After you have a candidate pair \((x, y)\), substitute it into both original equations. If either equation fails, an algebra slip occurred.

## Worked example

Solve

\[
\begin{cases}
3x + 2y = 13 \\
2x - y = 4.
\end{cases}
\]

From the second equation, \(y = 2x - 4\). Substitute into the first:

\[
3x + 2(2x - 4) = 13 \implies 3x + 4x - 8 = 13 \implies 7x = 21 \implies x = 3.
\]

Then \(y = 2(3) - 4 = 2\). The solution is \((3, 2)\).

## Checks

- \(3(3) + 2(2) = 9 + 4 = 13\).
- \(2(3) - 2 = 4\).

Elimination gives the same result: multiply the second equation by 2 to get \(4x - 2y = 8\), add this to \(3x + 2y = 13\), and obtain \(7x = 21\), so \(x = 3\) again.

If the two equations represent the same line, there are infinitely many solutions. If they represent parallel distinct lines, there is no solution. Here the unique pair \((3, 2)\) means the lines meet at a single point.

## A short follow-up

Solve \(x + y = 5\) and \(x - y = 1\). Adding the equations gives \(2x = 6\), so \(x = 3\) and \(y = 2\).
