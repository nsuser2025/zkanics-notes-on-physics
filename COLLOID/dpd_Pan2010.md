#### Pan2010 によるコロイド懸濁液のDPDシミュレーション
<p>
Ref. Pan2010_Langmuir.vol26.133  
</p>
<p>
colloid-colloid, colloid-solvent の conservative force:  
</p>
$$
\begin{align}
{\bf F}_{ij} = \frac{a_{ij}}{(1-e^{-b_{ij}})} \bigl[
\exp(-b_{ij}r_{ij}/r_{\rm c}) - \exp(-b_{ij}) \bigr] 
{\bf e}_{ij} \tag{1}
\end{align}
$$
<p>
soft coreポテンシャルでは粒子間のすり抜けが許されるが, コロイドではすり抜けは起きない.
(1)を用いればコロイドと溶媒のすり抜けは起こらない.
</p>
<p>
Volume fraction:  
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

---

#### Ornstein-Zernike 理論による解析
$$
\begin{align}
u(r) &= \frac{a_{ij}}{(1-e^{-b_{ij}})} \tag{2}
\end{align}
$$
<p>
(2) のままでは不連続点が発生してOZ計算は発散してしまう.
Ishizuka2023_J.Mol.Liq.vol384.122246の方法を用いることで発散を回避できる:
</p>
$$
\begin{align}
u'(r) &= u(r) - u(r_{\rm c}) \tag{3}
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
