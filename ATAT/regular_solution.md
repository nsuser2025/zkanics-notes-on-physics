<p>
固溶体の Gibbs 自由エネルギーは $G=H-TS=E+pV-TS$ で与えられるが,
常温常圧下での固体では 1 原子あたりの $pV$ 項は $10^{-5}$ eV であるのに対し,
内部エネルギーはおよそ $1$ eV/atom であるため, $E >> pV$ が成り立ち,
$G \approx E-TS$ と近似できる. </br>
ここで, $N_{\rm A}$ ヶの元素 A と $N_{\rm B}$ ヶの元素 B からなる二元固溶体の
混合モル Gibbs 自由エネルギーは次式で定義される. 
</p>
$$
\begin{align}
G_{\rm m}^{\rm mix} &\equiv G_{\rm m} - N_{\rm A}{}^{0}G_{A} - N_{\rm B}{}^{0}G_{\rm B} \tag{1}
\end{align}
$$
<p>
$N = N_{\rm A} + N_{\rm B}$ $\cdots$ 全原子数,
$x_{\rm A} = N_{\rm A}/N$ $\cdots$ 元素 A のモル分率 </br>
${}^{0}G_{\rm A}$ $\cdots$ 元素 A からなる純物質の Gibbs 自由エネルギー  
</p>
<p>
正則溶体モデルでは, 混合エントロピーを理想混合とし,
混合エンタルピーを組成の二次関数として表す.
従って, 正則溶体は厳密な理論ではなく, 自由エネルギーをどう分解し,
どう近似するかというモデリングのプラットフォームである.
Bragg–Williams 近似は, そのような混合エンタルピーを与える
最も単純なモデルであり, CALPHAD の発展以前によく用いられた近似である.
</p>

<span style="color: blue;">
<p>
<u>二元正則溶体のモル Gibbs 自由エネルギー</u>  
</p>
$$
\begin{align}
G_{\rm m} &\equiv N_{\rm Avo}\frac{G}{N} = N_{\rm Avo} \hat G \\ \\
&= x_{\rm A} {}^{0}G_{\rm m}^{\rm A} + x_{\rm B} {}^{0}G_{\rm m}^{\rm B} 
   + \Omega_{\rm AB} x_{\rm A}x_{\rm B} + RT (x_{\rm A}\ln x_{\rm A}
   + x_{\rm B} \ln x_{\rm B}) \tag{1}
\end{align}
$$
<p>
$\hat G$ $\cdots$ 1 原子あたりの Gibbs 自由エネルギー </br>
$N_{\rm Avo}$ $\cdots$ アボガドロ定数 </br>
$\Omega_{\rm AB} = z (e_{\rm AB} - (e_{\rm AA} + e_{\rm BB})/2) N_{\rm Avo}$ $\cdots$ 相互作用パラメータ</br>
</p>
<p>
<u>二元理想溶体のモル Gibbs 自由エネルギー</u>  
</p>
<p>
$\Omega_{\rm AB}=0$ のとき（1）は理想溶体のモル Gibbs 自由エネルギーになる.  
</p>
$$
\begin{align}
G_{\rm m} &= x_{\rm A} {}^{0}G_{\rm m}^{\rm A} + x_{\rm B} {}^{0}G_{\rm m}^{\rm B} 
  + RT (x_{\rm A}\ln x_{\rm A} + x_{\rm B} \ln x_{\rm B}) \tag{2}
\end{align}
$$
<p>
相互作用パラメータ $\Omega_{AB}$ がゼロになるということは, 元素 A と B の相互作用がゼロである
という意味ではなく, A - A, B - B, A - B 間の結合エネルギーが等しいということを意味していることに注意する.
全ての原子対の結合エネルギーが等しいとき, 熱力学的に完全ランダムな固溶体が安定となる.
</p>
</span>
