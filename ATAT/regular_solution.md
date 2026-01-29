<p>
固溶体の Gibbs 自由エネルギーは $G=H-TS=E+pV-TS$ で与えられるが,
常温常圧下での固体では 1 原子あたりの $pV$ 項は $10^{-5}$ eV であるのに対し,
内部エネルギーはおよそ $1$ eV/atom であるため, $E >> pV$ が成り立ち,
$G \approx E-TS$ と近似できる. </br>
ここで, $N_{\rm A}$ ヶの元素 A と $N_{\rm B}$ ヶの元素 B からなる二元固溶体の
混合 Gibbs 自由エネルギーは
$G_{\rm mix} \equiv G - x_{\rm A}{}^{0}G_{A} - x_{\rm B}{}^{0}G_{\rm B}$
で定義される.
</p>
<p>
正則溶体近似とは, Bragg-Williams 近似（平均場近似）によるエンタルピー項
とランダム分布仮定（理想混合エントロピー）にもとづくエントロピー項
から構成される固溶体の自由エネルギーモデルである.
Bragg-Williams 近似では最近接原子との結合エネルギーのみを固溶体のエンタルピーに取り入れる.
また, ランダム分布を仮定すると, 各サイトに A 元素の原子が存在する確率はモル分率 $x_{\rm A}$
に等しくなる. もちろん, この近似や仮定は厳密な固体モデルではないが,
物理的整合性と汎用性を兼ね備えたモデルとして CALPHAD の基礎式として用いられている.
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
$N_{\rm Avo}$ $\cdots$ アボガドロ定数, $N = N_{\rm A} + N_{\rm B}$ $\cdots$ 全粒子数 </br>
$x_{\rm A} \equiv N_{\rm A} / N$ $\cdots$ 元素 A のモル分率 </br>
${}^{0}G_{\rm m}^{\rm A}$ $\cdots$ 元素 A（純物質）のモル Gibbs 自由エネルギー </br>
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
