# Integration by parts

Integration by parts is the product rule in reverse:

\[
\int u\, dv = uv - \int v\, du.
\]

Choose \(u\) so that it becomes simpler when differentiated, and choose \(dv\) so that it is easy to integrate. A common order of preference for \(u\) is a logarithm, an inverse trigonometric function, a polynomial, then a trigonometric or exponential factor (the LIATE reminder).

## Worked example

Evaluate \(\int x e^{2x}\, dx\).

Let \(u = x\) and \(dv = e^{2x}\, dx\). Then \(du = dx\) and \(v = \frac{1}{2}e^{2x}\). Substituting gives

\[
\int x e^{2x}\, dx = \frac{x}{2}e^{2x} - \int \frac{1}{2}e^{2x}\, dx = \frac{x}{2}e^{2x} - \frac{1}{4}e^{2x} + C = \frac{e^{2x}}{4}(2x - 1) + C.
\]

## Check by differentiating

\[
\frac{d}{dx}\left[\frac{e^{2x}}{4}(2x-1)\right] = \frac{1}{4}\bigl(2e^{2x}(2x-1) + 2e^{2x}\bigr) = \frac{e^{2x}}{4}(4x-2+2) = x e^{2x}.
\]

The original integrand is recovered, so the antiderivative is correct. Remember to include the constant \(C\) in an indefinite integral.

## A short follow-up

For \(\int x\cos x\, dx\), take \(u = x\) and \(dv = \cos x\, dx\). Then \(du = dx\) and \(v = \sin x\), so the integral is \(x\sin x - \int \sin x\, dx = x\sin x + \cos x + C\).
