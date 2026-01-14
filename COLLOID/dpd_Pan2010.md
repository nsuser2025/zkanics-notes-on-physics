#### Pan2010 によるコロイド懸濁液のDPDシミュレーション

<p>
Ref. Pan2010_Langmuir.vol26.133  
</p>
<p>
コロイド―コロイド, コロイド―溶媒間の保存力:  
</p>
$$
\begin{align}
{\bf F}_{ij} &= -\frac{du(r)}{dr} {\bf e}_{ij} 
= \frac{a_{ij}}{(1-e^{-b_{ij}})} \bigl[
\exp(-b_{ij}r_{ij}/r_{\rm c}) - \exp(-b_{ij}) \bigr] 
{\bf e}_{ij} \tag{1}
\end{align}
$$
<p>
$r_{ij} = r_{\rm c}$ ではゼロになる. </br>  
ソフトコアポテンシャルでは粒子間のすり抜けが許されるが, コロイドではすり抜けは起きない.
(1)を用いればコロイドと溶媒のすり抜けは起こらない（Ref. の Fig. 2）.
</p>
<p>
体積分率:  
</p>
$$
\begin{align}
\phi &\equiv \frac{4\pi N a^{3}}{3V_{\rm total}} \tag{2}
\end{align}
$$
<p>
$a$: コロイド粒子の半径（$a = 0.98$）,
$N$: コロイド粒子の数（$N = 200$～$1300$）</br>
$V_{\rm total}$: シミュレーションボックスの体積（$20^{3}$）
</p>
<p>
$N=200 \cdots \phi=4\pi \cdot 200 \cdot (0.98)^{3}/(3 \cdot 20^{3}) = 0.098 \approx 0.1$ </br>
$N=1300 \cdots \phi=0.64$
</p>

---

#### Ornstein-Zernike 理論による解析
$$
\begin{align}
u(r) &= \frac{a_{ij}}{(1-e^{-b_{ij}})}\biggl[
\biggl(\frac{r_{\rm c}}{b_{ij}}\biggr) \exp (-b_{ij}r/r_{\rm c}) + \exp (-b_{ij}) r
\biggr]
\tag{3}
\end{align}
$$
<p>
(3) のままでは不連続点が発生して OZ 計算は発散してしまう.
Ishizuka2023_J.Mol.Liq.vol384.122246の方法を用いることで発散を回避できる:
</p>
$$
\begin{align}
u'(r) &= u(r) - u(r_{\rm c}) \tag{4}
\end{align}
$$
<p>
コロイド密度:  
</p>
$$
\begin{align}
\rho &= \frac{3\phi}{(4\pi a^{3})} \tag{5}
\end{align}
$$
