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

#### IOZのLegendre多項式展開

<p>
$\theta_{1} = 0$, $\phi_{1} = 0$, $\phi_{2} = 0$ のときは
</p>

$$
\begin{align}
&{\bf e}\_{2} = (\sin\theta\_{2}, 0, \cos\theta\_{2}) \\\\
&{\bf e}\_{3} = (\sin\theta\_{3}\cos\phi\_{3}, \sin\theta\_{3}\sin\phi\_{3}, \cos\theta\_{3}) \\\\
&\cos\theta\_{32} = {\bf e}\_{2}\cdot{\bf e}\_{3} = \cos\theta\_{2}\cos\theta\_{3}
                    + \sin\theta\_{2}\sin\theta\_{3}\cos\phi\_{3} \tag{1}
\end{align}
$$

<p>
$x \equiv \cos\theta$ とすると
</p>

$$
\begin{align}
t(r\_{1},r\_{2},x\_{2})
&= \int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} ~\rho(r\_{3})
\int^{2\pi}\_{0} d\phi\_{3} \int^{1}\_{-1} dx\_{3}
~c(r\_{1},r\_{3},x\_{3}) ~h(r\_{3},r\_{2},x\_{32}) \tag{2}
\end{align}
$$

<p>
（2）のLegendre多項式展開
</p>

$$
\begin{align}
c(r\_{1},r\_{3},x\_{3})
&= \sum\_{i} \hat c\_{i}(r\_{1},r\_{3}) ~P\_{i}(x\_{3}) \tag{3} \\\\
h(r\_{3},r\_{2},x\_{32})
&= \sum\_{j} \hat h\_{j}(r\_{3},r\_{2}) ~\color{red}{P\_{j}(x\_{32})} \\\\
&= \sum\_{j} \hat h\_{j}(r\_{3},r\_{2}) ~\color{green}{P\_{j}(x\_{2})P\_{j}(x\_{3})} \tag{4} 
\end{align}
$$

$$
\begin{align}
\hat t\_{n}(r\_{1},r\_{2})
&= \frac{2n+1}{2} \sum\_{ij} \int^{1}\_{-1} dx\_{2}
\int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} \int^{2\pi}\_{0} d\phi\_{3}
\int^{1}\_{-1} dx\_{3} ~\hat c\_{i}(r\_{1},r\_{3}) ~\rho(r\_{3}) \\\\
&\times \hat h\_{j}(r\_{3},r\_{2}) 
~\color{red}{P\_{n}(x\_{2})P\_{j}(x\_{2})P\_{i}(x\_{3})P\_{j}(x\_{3})} \\\\ \\\\
&= \frac{2n+1}{2} \int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} \int^{2\pi}\_{0} d\phi\_{3}
~\hat c\_{n}(r\_{1},r\_{3}) ~\rho(r\_{3}) ~\hat h\_{n}(r\_{3},r\_{2})
\color{green}{\biggl(\frac{2}{2n+1}\biggr)^{2}} \\\\ \\\\
&= \frac{4\pi}{2n+1} \int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} 
~\hat c\_{n}(r\_{1},r\_{3}) ~\rho(r\_{3}) ~\hat h\_{n}(r\_{3},r\_{2}) \tag{5}
\end{align}
$$

<p>
<span style="color:blue">
※ Legendre多項式展開
</span>  
</p>

$$
\color{blue}{
\begin{align}
f(x) &= \sum^{\infty}\_{n=0} \hat f\_{n} P\_{n}(x) \tag{4} \\\\
\hat f\_{n} &= \frac{2n+1}{2} \int^{1}\_{-1} dx ~f(x)P_{n}(x) \tag{6}
\end{align}
}
$$

<p>
<span style="color:blue">
※ Legendre多項式の直交性
</span>  
</p>

$$
\color{blue}{
\begin{align}
\int^{1}\_{-1} dx ~P\_{n}(x) P\_{m}(x) = \frac{2}{2n+1} \delta\_{mn} \tag{7}
\end{align}
}
$$

<p>
<span style="color:blue">
※ Legendre多項式の加法定理  
</span>  
</p>

$$
\color{blue}{
\begin{align}
P\_{j}(x\_{32})
&= P\_{j}(x\_{2})P\_{j}(x\_{3}) + 2 \sum^{j}\_{m=1}
\frac{(j-m)!}{(j+m)!} P^{m}\_{j}(x\_{2})P^{m}\_{j}(x\_{3}) \cos [m(\phi\_{2}-\phi\_{3})] \tag{8}
\end{align}
}
$$

<p>
<span style="color:blue">
$P^{m}_{j}$: Legendre陪多項式（Associated Legendre polynomial） 
</span>  
</p>

<p>
<span style="color:blue">
$\phi_{2}=0$のとき, (10)の右辺第2項は $\int^{2\pi}_{0} d\phi_{3}$ でゼロになる.
</span>  
</p>

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
