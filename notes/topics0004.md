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
                    + \sin\theta\_{2}\sin\theta\_{3}\cos\phi\_{3} \tag{2}
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
~c(r\_{1},r\_{3},x\_{3}) ~h(r\_{3},r\_{2},x\_{32}) \tag{3}
\end{align}
$$

<p>
<span style="color:blue">
Legendre多項式展開  
</span>  
</p>

$$
\color{blue}{
\begin{align}
f(x) &= \sum^{\infty}\_{n=0} \hat f\_{n} P\_{n}(x) \tag{4} \\\\
\hat f\_{n} &= \frac{2n+1}{2} \int^{1}\_{-1} dx ~f(x)P_{n}(x) \tag{5}
\end{align}
}
$$

<p>
<span style="color:blue">
Legendre多項式の直交性  
</span>  
</p>

$$
\color{blue}{
\begin{align}
\int^{1}\_{-1} dx ~P\_{n}(x) P\_{m}(x) = \frac{2}{2n+1} \delta\_{mn} \tag{6}
\end{align}
}
$$



---

#### References

<p>
1. Attard1989_J.Chem.Phys.vol91.3072  
</p>
