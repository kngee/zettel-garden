---
created: "2026-01-15 at 00:16"
tags:
  - permanent
publish: "true"
---

Using the earlier conclusion that the component of a vector along another vector can be approximated using the component along the target vector.

When extended to continuous time signals, it can be said that $$g(t)=c\cdot x(t)~~~~t_1\leq t\leq t_2$$
What we are interested in is minimizing the error signal, we know that this means minimizing the signal energy.

We know that signal energy is the integral with respect to time, however time is a dummy variable, we are trying to optimize for the selection of the scalar c such that error is minimal. The result of this minimization is that the optimum scalar can be chosen with the following equation $$c=\frac{1}{E_x}\int_{t_1}^{t_2}g(t)x(t)dt$$
in the case of real valued signals.

See Also:

- [[]]

---

B. P. Lathi and Z. Ding, _Modern Digital and Analog Communication Systems_, 4th International ed. New York, NY, USA: Oxford University Press, 2010.