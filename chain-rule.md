# The derivative chain rule

If a function is a composition, \(y = f(g(x))\), the chain rule says

\[
\frac{dy}{dx} = f'(g(x)) \cdot g'(x).
\]

Differentiate the outer function, leave the inner expression in place, and then multiply by the inner derivative. Forgetting that last factor is the most common error.

## Worked example

Differentiate \(y = \sin(3x^2 + 1)\).

Let \(f(u) = \sin u\) and \(u = g(x) = 3x^2 + 1\). Then \(f'(u) = \cos u\) and \(g'(x) = 6x\), so

\[
y' = \cos(3x^2 + 1) \cdot 6x = 6x\cos(3x^2 + 1).
\]

## Checks

- The cosine should still be evaluated at \(3x^2 + 1\), not at \(x\).
- The extra factor must be \(6x\), the derivative of the inner polynomial.
- At \(x = 0\), the inner derivative is zero, so \(y' = 0\), which matches \(6(0)\cos(1) = 0\).

## A short follow-up

Differentiate \(y = (4x + 1)^5\). The outer power rule gives \(5(4x+1)^4\), and the inner derivative is 4, so \(y' = 20(4x+1)^4\).
