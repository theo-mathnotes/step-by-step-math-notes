# Step-by-Step Math Notes

A short, free study resource with worked examples in algebra and calculus. Each problem is solved in plain language, with every algebraic move written out so you can follow the reasoning and then try a similar exercise on your own. The notes are meant for high-school and early college students who want to see the method, not just the final answer.

The five examples below cover equations you are likely to meet in class: a quadratic, a chain-rule derivative, an integration-by-parts integral, a two-variable linear system, and a percentage word problem. Longer write-ups: [quadratic equations](quadratic-equations.md), [chain rule](chain-rule.md), [integration by parts](integration-by-parts.md), [systems of linear equations](systems-of-linear-equations.md), [percentage problems](percentage-problems.md).

## 1. Solving a quadratic equation

Solve \(2x^2 - 7x - 15 = 0\).

Here \(a = 2\), \(b = -7\), and \(c = -15\). The quadratic formula is

\[
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}.
\]

The discriminant is \(b^2 - 4ac = (-7)^2 - 4(2)(-15) = 49 + 120 = 169 = 13^2\). Substituting the values gives

\[
x = \frac{7 \pm 13}{4}.
\]

So \(x = 20/4 = 5\) or \(x = -6/4 = -3/2\).

To confirm, plug each root back into the original equation:

- For \(x = 5\): \(2(25) - 7(5) - 15 = 50 - 35 - 15 = 0\).
- For \(x = -3/2\): \(2(9/4) - 7(-3/2) - 15 = 9/2 + 21/2 - 15 = 15 - 15 = 0\).

Both roots check out. When the discriminant is a perfect square, as it is here, the solutions are rational and a factoring check is also possible: \(2x^2 - 7x - 15 = (2x + 3)(x - 5)\).

## 2. The derivative chain rule

Differentiate \(y = \sin(3x^2 + 1)\).

The chain rule says that if \(y = f(g(x))\), then \(y' = f'(g(x)) \cdot g'(x)\). Think of the sine as the outer function and \(3x^2 + 1\) as the inner function.

- The derivative of \(\sin u\) with respect to \(u\) is \(\cos u\).
- The derivative of the inner function \(u = 3x^2 + 1\) is \(6x\).

Therefore

\[
\frac{dy}{dx} = \cos(3x^2 + 1) \cdot 6x = 6x\cos(3x^2 + 1).
\]

A quick structure check: the answer should still contain a cosine of the original inner expression, multiplied by the inner derivative \(6x\). If you had forgotten the \(6x\), you would have differentiated only the outer function.

## 3. Integration by parts

Evaluate \(\int x e^{2x}\, dx\).

Integration by parts comes from the product rule and is usually written \(\int u\, dv = uv - \int v\, du\). Choose \(u\) to become simpler when differentiated and \(dv\) to be easy to integrate. Here, let \(u = x\) and \(dv = e^{2x}\, dx\). Then \(du = dx\) and \(v = \frac{1}{2}e^{2x}\).

\[
\int x e^{2x}\, dx = x \cdot \frac{1}{2}e^{2x} - \int \frac{1}{2}e^{2x}\, dx = \frac{x}{2}e^{2x} - \frac{1}{4}e^{2x} + C = \frac{e^{2x}}{4}(2x - 1) + C.
\]

Differentiate the antiderivative to check:

\[
\frac{d}{dx}\left[\frac{e^{2x}}{4}(2x-1)\right] = \frac{1}{4}\left(2e^{2x}(2x-1) + e^{2x}\cdot 2\right) = \frac{e^{2x}}{4}(4x - 2 + 2) = x e^{2x}.
\]

The original integrand comes back, so the antiderivative is correct.

## 4. A system of linear equations

Solve the system

\[
\begin{cases}
3x + 2y = 13 \\
2x - y = 4.
\end{cases}
\]

Solve the second equation for \(y\): \(y = 2x - 4\). Substitute into the first equation:

\[
3x + 2(2x - 4) = 13 \implies 3x + 4x - 8 = 13 \implies 7x = 21 \implies x = 3.
\]

Then \(y = 2(3) - 4 = 2\). The solution is \((x, y) = (3, 2)\).

Check both original equations: \(3(3) + 2(2) = 9 + 4 = 13\) and \(2(3) - 2 = 4\). Both hold, so the pair is consistent.

Substitution is convenient when one variable is easy to isolate. If both equations are already arranged neatly, elimination is just as good: multiplying the second equation by 2 and adding would cancel \(y\) and lead to the same value of \(x\).

## 5. A percentage problem

A jacket is priced at \$80. The store takes 25% off, and then 8% sales tax is added to the discounted price. What is the final amount paid?

A 25% discount leaves 75% of the original price: \(0.75 \times 80 = 60\). The tax is 8% of the discounted price, not of the original \$80: \(0.08 \times 60 = 4.80\). The total is \(60 + 4.80 = 64.80\).

Equivalently, multiply once by the combined factor \(0.75 \times 1.08 = 0.81\), so \(80 \times 0.81 = 64.80\). A common mistake is to subtract 25% and then add 8% of the original price, which would overstate the tax.

## Check your work

After you finish a problem by hand, it helps to verify the algebra with a second method: substitute a root, differentiate an antiderivative, or recompute a percentage with the combined factor, as in the examples above. For extra practice problems, or when you want to compare your steps with another worked solution, you can also check answers with the free step-by-step AI math solver at [MathGPT – Free AI Math Solver](https://mathssolvergpt.com/en). Use it to confirm your work, then try a nearby problem without looking at the hints.

## License

These notes are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You may share and adapt them with attribution.
