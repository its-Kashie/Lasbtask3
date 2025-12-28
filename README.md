# Assignment  
## Random Variables – Continuous Case

---

## Question (Part b)

A continuous random variable \(X\) has the probability density function (p.d.f.):

\[
f(x) =
\begin{cases}
A(2-x)(2+x), & 0 \le x \le 2 \\
0, & \text{elsewhere}
\end{cases}
\]

Find:  
(i) the value of \(A\)  
(ii) \(P(X = \tfrac{1}{2})\)  
(iii) \(P(X \le 1)\)  
(iv) \(P(X \ge 2)\)  
(v) \(P(1 \le X \le 2)\)

---

## Solution

### (i) Finding the value of \(A\)

For a valid probability density function,

\[
\int_{-\infty}^{\infty} f(x)\,dx = 1
\]

\[
\int_0^2 A(2-x)(2+x)\,dx = 1
\]

**Simplify:**

\[
(2-x)(2+x) = 4 - x^2
\]

\[
A\int_0^2 (4 - x^2)\,dx = 1
\]

\[
A\left[4x - \frac{x^3}{3}\right]_0^2 = 1
\]

\[
A\left(8 - \frac{8}{3}\right) = 1
\]

\[
A\left(\frac{16}{3}\right) = 1
\]

\[
\boxed{A = \frac{3}{16}}
\]

---

### (ii) Finding \(P(X = \tfrac{1}{2})\)

Since \(X\) is a continuous random variable, the probability at a single point is zero.

\[
\boxed{P(X = \tfrac{1}{2}) = 0}
\]

---

### (iii) Finding \(P(X \le 1)\)

\[
P(X \le 1) = \int_0^1 \frac{3}{16}(4 - x^2)\,dx
\]

\[
= \frac{3}{16}\left[4x - \frac{x^3}{3}\right]_0^1
\]

\[
= \frac{3}{16}\left(4 - \frac{1}{3}\right)
\]

\[
= \frac{3}{16} \cdot \frac{11}{3}
\]

\[
\boxed{P(X \le 1) = \frac{11}{16}}
\]

---

### (iv) Finding \(P(X \ge 2)\)

The p.d.f. is zero for \(x > 2\), and the probability at \(x = 2\) is also zero.

\[
\boxed{P(X \ge 2) = 0}
\]

---

### (v) Finding \(P(1 \le X \le 2)\)

\[
P(1 \le X \le 2) = 1 - P(X \le 1)
\]

\[
= 1 - \frac{11}{16}
\]

\[
\boxed{P(1 \le X \le 2) = \frac{5}{16}}
\]

---

## Final Answers

\[
\begin{aligned}
\text{(i)}\;& A = \frac{3}{16} \\
\text{(ii)}\;& P(X = \tfrac{1}{2}) = 0 \\
\text{(iii)}\;& P(X \le 1) = \frac{11}{16} \\
\text{(iv)}\;& P(X \ge 2) = 0 \\
\text{(v)}\;& P(1 \le X \le 2) = \frac{5}{16}
\end{aligned}
\]