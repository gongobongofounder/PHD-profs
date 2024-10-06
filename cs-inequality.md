@import "style.css";

# CS Inequality Overview

## The Cauchy–Schwarz inequality (also called Cauchy–Bunyakovsky–Schwarz inequality)

### Statement:
Let $a_1,a_2,\cdots,a_n,b_1,b_2,\cdots,b_n \in \mathbb{C}$ then we have the following:

$$\left|\sum_{i=1}^n a_i\overline b_i\right|^2\leq \left(\sum_{i=1}^n|a_i|^2 \right)\left(\sum_{i=1}^n|b_i|^2\right)$$
and equality holds iff $a_i=tb_i$ for some $t\in \mathbb{C}$ $\forall i\in \{1,2,3,\cdots n \}$

### Proof:
Consider the function $f:\mathbb{R} \rightarrow \mathbb{R}$ defined by

$$
\begin{equation}
    f(t)=\sum_{i=1}^n |a_i-tb_i|^2 \quad (Remember)
\end{equation}
$$

**Note:**
$$
\begin{equation}
|z|^2=z\overline z 
\end{equation}
$$

Using (2) in (1) we get,

$$
\begin{align*}
    f(t)=\sum_{i=1}^n (a_i-tb_i)(\overline{a_i-tb_i}) \\
    =\sum_{i=1}^n (a_i-tb_i)(\overline{a_i}-\overline{t}\overline{b_i})\\
    =\sum_{i=1}^n \left(|a_i|^2-(a_i\overline{b_i}+\overline{a_i}b_i)t+|b_i|t^2\right)\\
    =\sum_{i=1}^n \left(|a_i|^2-Re(a_i\overline{b_i})t+|b_i|t^2\right)\\
    =\sum_{i=1}^n |a_i|^2-2Re\left(\sum_{i=1}^na_i\overline{b_i}\right)t+\left(\sum_{i=1}^n|b_i|\right)t^2
\end{align*}
$$

Hence we get,
$$
\begin{equation}
    f(t)=\sum_{i=1}^n |a_i|^2-2Re\left(\sum_{i=1}^na_i\overline{b_i}\right)t+\left(\sum_{i=1}^n|b_i|\right)t^2
\end{equation}
$$

**Note:** Notice that $f(t)\geq 0$ $\forall t\in \mathbb{R}$, hence by the property of quadratic equation we get, $b^2-4ac\leq0$. Then apply this to equation (3) we get,

$$
\begin{equation}
    \left(2Re\left(\sum_{i=1}^na_i\overline{b_i}\right)\right)^2\leq 4\left(\sum_{i=1}^n|a_i|^2 \right)\left(\sum_{i=1}^n|b_i|^2\right)
\end{equation}
$$

Now, making $g: \mathbb{R}\rightarrow \mathbb{R}$ defined by 
$$
\begin{equation*}
    g(t)=\sum_{j=1}^n |a_j-itb_j|^2 \quad (i=\sqrt{-1})
\end{equation*}
$$

And proceeding similarly we get, 

$$
\begin{equation}
    \left(2Im\left(\sum_{i=1}^na_i\overline{b_i}\right)\right)^2\leq 4\left(\sum_{i=1}^n|a_i|^2 \right)\left(\sum_{i=1}^n|b_i|^2\right)
\end{equation}
$$

Adding (4) and (5) we get,

$$\left|\sum_{i=1}^n a_i\overline b_i\right|^2\leq \left(\sum_{i=1}^n|a_i|^2 \right)\left(\sum_{i=1}^n|b_i|^2\right)$$

Now, for the equality we have, $f(t)=0$ happens only if two of its roots are same, otherwise it could n't be always non-negative.
 Hence we have, $b^2-4ac=0$ and this happens iff the equality happens in C-S inequality.

 But, from definition of $f$ we have $a_i=tb_i$ $\forall i=1,2,\cdots, n$ or 
