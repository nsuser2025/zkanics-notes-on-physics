#### Krieger-Dougherty 粘度推算モデル

$$
\begin{align}
\eta &= \eta_{0} \biggl( 1 - \frac{\phi}{\phi_{\rm max}} \biggr)^{-[\eta]\phi_{\rm max}} \tag{1}
\end{align}
$$
<p>
$\eta_{0}$ $\cdots$ 基材粘度（粉体を一切含まない基材の粘度）</br> 
$[\eta]$ $\cdots$ 固有粘度（粉体が球体であれば2.5のままでOK）</br>
$\phi_{\rm max}$ $\cdots$ 最大充填体積分率（固体粒子を隙間なく詰めたときの上限）</br></br>
$\rightarrow$ 懸濁液の粘度は $\phi$ と $\phi_{\rm max}$ が決める.
</p>

<span style="color: blue;">
<p>
$\phi_{\rm max} = 0.74$（最密充填, 理論限界）</br>
$\phi_{\rm max} = 0.64$（単文散, 剛体球）</br>
$\phi_{\rm max} = 0.55-0.64$（高分散）</br>
$\phi_{\rm max} = 0.45-0.55$（相互作用が強く, 有効半径が大きい）
</p>
</span>

---

#### 吸着層の厚さと粘度の関係

<p>
吸着層が厚いほど粘度は高くなる.</br>
固体粒子の半径 $70$ nm, 固体粒子密度 $2.2$, 液体密度 $1.15$, 質量分率 $50$ wt% のとき,</br>
吸着層をもたない固体粒子の体積分率は $\phi_{\rm eff} = 0.549$. </br>
一方、吸着層の厚さ $\delta = 1$ nm をもつ固体粒子では,
有効体積分率は $\phi_{\rm eff} = 0.564$ になる.
(1)より, 吸着層がないときと比べて粘度は 1.3 倍になる. 
</p>
$$
\begin{align}
\biggl(\frac{1-0.564/0.64}{1-0.549/0.64}\biggr)^{-2.5\times0.64}
&\approx 1.33
\end{align}
$$


