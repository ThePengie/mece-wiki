---
sidebar_position: 3
---

# Use Mathematical Formulas in your Pages

KaTeX is installed and enabled on this site. You can use it by surrounding your equations with `$` characters.

For example:

```
Let $f\colon[a,b]\to\R$ be Riemann integrable. Let $F\colon[a,b]\to\R$ be
$F(x)=\int_{a}^{x} f(t)\,dt$. Then $F$ is continuous, and at all $x$ such that
$f$ is continuous at $x$, $F$ is differentiable at $x$ with $F'(x)=f(x)$.
```

Becomes

Let $f\colon[a,b]\to\R$ be Riemann integrable. Let $F\colon[a,b]\to\R$ be
$F(x)=\int_{a}^{x} f(t)\,dt$. Then $F$ is continuous, and at all $x$ such that
$f$ is continuous at $x$, $F$ is differentiable at $x$ with $F'(x)=f(x)$.

## Technical Notes

[KaTeX](https://github.com/KaTeX/KaTeX) [0.16.11](https://github.com/KaTeX/KaTeX/releases/tag/v0.16.11) is the currently installed version that is included with the markdown plugins.
If this version is upgraded, then the new version should be copied to the
`/static/katex/#.##.##` folder. Only the `katex.min.css` and the `fonts/*.woff2` files are required.
