---
layout: post
title: "Artin Section 10.1"
author: "Henrique Fonseca"
categories: journal
tags: [artin,algebra,solutions]

---

**1a.** Ditributive property gives $0 a = (0 + 0) a = 0 a + 0 a$. Using that $(R, +)$ is a group, cancel $0a$ to get $0 = 0a$.
**1b.** Distributive property gives $(-1)a + a = (-1)a + 1a = (-1 + 1) a = 0a = 0$, the last equality following from a).
**1c.** Use b) to write $(-a)b = ((-1)a)b$, so the result follows from the associative property.

**2.** Let $\alpha = \sqrt[3]{2} \in \mathbb{R}$. If $R \subset \mathbb{C}$ is a ring containing $\alpha$, then $\mathbb{Z}[\alpha] \subset R$, so the smallest such $R$ is $\mathbb{Z}[\alpha]$. Let's describe this ring explicitly, using the relation $\alpha^3 = 2 \in \mathbb{Z}$. Given a power $\alpha^n$, use the Euclidean algorithm to write $\alpha^n = \alpha^{q3 + r} = 2^q \alpha^r$ with $0 \leq r < 3$. Therefore any polynomial $p(\alpha) \in \mathbb{Z}[\alpha]$ can be written as $a + b \alpha + c \alpha^2$. This means $\mathbb{Z}[\alpha] = \mathbb{Z} + \mathbb{Z} \alpha + \mathbb{Z} \alpha^2$  (this is the best we can do, since $\lbrace 1, \alpha, \alpha^2 \rbrace$ is linearly independent over $\mathbb{Q}$).

**3.** Consider powers of $\alpha$:
$$\alpha^{2k} = \frac{(-1)^k}{2^{2k}}, \quad \alpha^{2k + 1} = \frac{(-1)^k}{2^{2k + 1}}i .$$
Let $\varepsilon > 0$. Since $\mathbb{Q}$ is dense in $\mathbb{R}$, it 
suffices to show that, for _rational_ coefficients $a$ and $b \in \mathbb{Q}$, there exist positive integers $k$, $k' > 0$ such that

$$
|(m\alpha^{2k} + n\alpha^{2k' + 1}) - (a + bi)| < \varepsilon ,
$$

for some $m$, $n \in \mathbb{Z}$.
Let's do it for the first coordinate: take $k$ such that $1/2^{2k} < \varepsilon$. But $a$ lies in an interval of the form

$$
\left[ \frac{m}{2^{2k}}, \frac{m + 1}{2^{2k}} \right],
$$

for some $m \in \mathbb{Z}$. Therefore $|m/2^{2k} - a| < \varepsilon$. Similarly, one can exhibit an integer $n \in \mathbb{Z}$ with $|n/2^{2k'} - b| < \varepsilon$ and the result follows from the triangle inequality.

**4.**
