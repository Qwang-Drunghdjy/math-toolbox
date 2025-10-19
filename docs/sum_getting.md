# 求和方法

## 级数

### 常用等价无穷小量替换

```math
\begin{aligned}
    \sin x \sim \tan x & \sim x \\
    \arcsin x \sim \arctan x & \sim x \\
    \ln(1 + x) \sim e^x - 1 &\sim x \\
    \ln(x + \sqrt{1 + x^2}) & \sim x \\
\end{aligned}
```

```math
\begin{aligned}
    x - \ln(1 + x) & \sim \frac{1}{2}x^2 \\
    1 - \cos x & \sim \frac{1}{2}x^2 \\
\end{aligned}
```

```math
\begin{aligned}
    x - \sin x & \sim \frac{1}{6}x^3 \\
    \arcsin x - x &\sim \frac{1}{6}x^3 \\
\end{aligned}
```

```math
\begin{aligned}
    \tan - x &\sim \frac{1}{3}x^3 \\
    x - \arctan x &\sim \frac{1}{3}x^3 \\
\end{aligned}
```

```math
\begin{aligned}
    \log_a(1 + x) & \sim \frac{x}{\ln a} \\
    (1 + x)^\alpha - 1 &\sim \alpha x \\
    \tan x - \sin x &\sim \frac{1}{2}x^3 \\
\end{aligned}
```

### 连续自然数的平方和公式

```math
\begin{aligned}
    \sum_{k = 1}^{n} k^2 &= 1^2 + 2^2 + 3^2 + \cdots + n^2 \\
    &= \frac{n(n + 1)(2n + 1)}{6}
\end{aligned}
```

### $p$-级数和几何级数

> **定义: ($p$-级数)** 形如
>
> ```math
> \sum_{n = 1}^{\infty} \frac{1}{n^p}
> ```
>
> 的级数.

**$p$-级数的敛散性:**

- 当 $p \leq 1$, $p$-级数发散.
- 当 $p > 1$, $p$-级数收敛.

> **定义: (几何级数)** 形如
>
> ```math
> \sum_{n = 1}^{\infty} aq^{n}, \quad a \neq 0
> ```
>
> 的级数.

**几何级数的敛散性:**

- 当 $|q| < 1$, 几何级数收敛.
- 当 $|q| \geq 1$, 几何级数发散.

## 等差数列和等比数列求和

**等差数列前 $n$ 项求和公式:**

```math
S_n = \frac{1}{2}n(a_1 + a_n) = na_1 + \frac{n}{2}(n - 1)d
```

- 求和依赖项数 $n$ 的明确, 不适用于无穷项求和.

**等比数列前 $n$ 项求和公式:**

```math
S_n =
\begin{cases}
    \frac{a_1(1 - q^n)}{1 - q}, & (q \neq 1) \\
    na_1, & (q = 1)
\end{cases}
```

无穷等比数列求和公式:

```math
S_\infty = \frac{a_1}{1 - q}
```

- 其中 $q$ 是公比, 且 $|q| < 1$. 如果 $|q| \geq 1$, 等比数列的和是发散的.