#### Pan2010 によるコロイド懸濁液のDPDシミュレーション
<p>
Ref. Pan2010_Langmuir.vol26.133  
</p>
<p>
colloid-colloid, colloid-solvent の conservative force  
</p>
$$
\begin{align}
{\bf F}_{ij} = \frac{a_{ij}}{(1-e^{-b_{ij}})} \tag{1}
\end{align}
$$
<p>
soft coreポテンシャルは粒子間のすり抜けが許されるが, コロイドではすり抜けは起きない.
(1)を用いればコロイドと溶媒のすり抜けは起こらない.
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
コロイドの密度:  
</p>
$$
\begin{align}
\rho &= \frac{3\phi}{(4\pi a^{3}} \tag{5}
\end{align}
$$
