#### Inhomogeneous Ornstein-Zernike Equation (IOZ)

<p>
Pair potentialが $u(r_{1},r_{2},\theta_{12})$ のときのIOZ方程式$^{1}$.
</p>

$$
\begin{align}
h(r\_{1},r\_{2},\theta\_{12})
&= c(r\_{1},r\_{2},\theta\_{12}) + \int d{\bf r}\_{3}
~c(r\_{1},r\_{3},\theta\_{13}) ~\rho(r_{3}) ~h(r\_{3},r\_{2},\theta\_{32}) \tag{1}
\end{align}
$$

<p>
Inhomogeneous solvent-solvent相関関数を仮定したときのsolute-solvent OZ方程式  
</p>

$$
\begin{align}
h(r\_{2})
&= c(r\_{2}) + \int d{\bf r}\_{3}
~c(r\_{3}) ~\rho(r_{3}) ~h(r\_{3},r\_{2},\theta\_{32}) \tag{1'}
\end{align}
$$

---

#### 数値解法

<p>
Gauss-Legendre積分を用いたLegendre多項式展開  
</p>

$$
\begin{align}
\hat f\_{n} &= \frac{2n+1}{2} \sum^{N}\_{i=1} \omega\_{i} f\_{i} ~P\_{n}(x\_{i}) \tag{11} \\\\
f\_{i} &= \sum^{N-1}\_{n=0} \hat f\_{n} P\_{n}(x\_{i}) \tag{12}
\end{align}
$$

$$
\begin{align}
&\sum^{N}\_{i=1} \omega_{i} P\_{n}(x\_{i})P\_{m}(x\_{i}) 
= \frac{2}{2n+1} \delta\_{nm} \tag{13} \\\\ \\\\
&\sum^{N-1}\_{n=0} \frac{2n+1}{2} P\_{n}(x\_{i}) P\_{n}(x\_{j}) 
= \omega^{-1}\_{i} \delta\_{ij} \tag{14}
\end{align}
$$

<p>
<span style="color:blue">
※ Numerical ReceipeのGauss-Legendre積分
</span>
</p>

$$
\color{blue}{
\begin{align}
\int^{x\_{2}}\_{x\_{1}} f(x) dx
&= \sum^{N}\_{j=1} \omega\_{j} f(x\_{j}) \tag{15}
\end{align}
}
$$

<p>
<span style="color:blue">
$x_{1} \rightarrow -1$, $x_{2} \rightarrow 1$, $N \rightarrow n$, $\cos\theta \rightarrow x$
</span>
</p>

<p>
<span style="color:blue">
※ Legendre多項式の再帰関係を用いた数値計算
</span>
</p>

$$
\color{blue}{
\begin{align}
&P\_{0}(x) = 1, P\_{1}(x) = x, \\\\ \\\\
&P\_{n}(x) = \frac{2n-1}{n}xP\_{n-1}(x) - \frac{n-1}{n}P\_{n-2}(x) \tag{16}
\end{align}
}
$$

---

#### References

<p>
1. Attard1989_J.Chem.Phys.vol91.3072  
</p>
