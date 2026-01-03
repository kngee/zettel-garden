---
created: 2025-12-31 at 14:46
tags:
  - fleeting
  - telecommunications
---
B. P. Lathi and Z. Ding, _Modern Digital and Analog Communication Systems_, 4th International ed. New York, NY, USA: Oxford University Press, 2010.

---

- Systems extract meaning or additional information from input signals to create a set of more signals.
- We interested in measuring the size of a signal, because the size of the signal indicates its strength.
- Signal energy, $$E_g=\int_{-\infty}^{\infty}|g(t)|^2dt$$
- Signal energy is really only useful for us for signal that have finite energy. Signals that aren't become indistinguishable from one another.
- Practically, all signals are finite -> we are unable to guarantee a signal that propagates for eternity. At the moment, our understanding of finite energy is, $$g(t) \rightarrow 0~as~|t|\rightarrow\infty$$
- For signals that are periodic or have a statistical regularity, we can define a finite signal power $$P_g=\lim_{T\rightarrow\infty}\frac{1}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}g^2(t)dt$$
- Messages are random signals as opposed to deterministic signal.
- The unit impulse function is unacceptable in pure mathematics.
- The Sampling Property of the unit impulse function is pretty important.
- We use vector space operations and definitions when working with signals in time.
- Everything starts with trying to determine the similarity between vectors. This is where we quantify error and derive a formula for the minimal error approximation of a target vector.
- Signals are orthogonal when the area of their product when integrated with time is zero.
- The norm of a signal is a recurring measure of a signal, I don't yet really understand why.
- When moving from real valued to complex valued signals, the conditions for orthogonality become generalised and the real valued case becomes a special case.
- We take advantage of orthogonality when determining the sum energy of N signals.
- We define a new measure for signal similarity that can be proven with Cauchhy-Swarz inequality. However, the similarity definition needs improving and so we defined a cross-correlation function that can find the similarity of signals that have been shifted in time which is really useful in any sort of transceiver system.
- If we are able to represent signals as the sum of the set of orthogonal signals, we can create an orthogonal signal space called a complete orthogonal basis of a vector space.
- Parseval's theorem allows us to take advantage of a complete orthogonal basis to find the total energy of a set of N mutually orthogonal signals.
- The Fourier Series is a powerful tool for approximating signals, how does it take advantage of orthogonality in Euler's Identity and what more can it do? Ie. We learn about Parseval's Theorem in the Fourier Series, what does it allow us to do.