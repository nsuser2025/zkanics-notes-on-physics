<p>
Bragg-Williams 近似にもとづき, 最近接原子との結合エネルギーのみで
二元正則固溶体のエンタルピーを表すと次式となる.
ただし, $N_{\alpha\beta}$ は $\alpha$-$\beta$ 対の数,
$e_{\alpha\beta}$ は $\alpha$-$\beta$ 間の結合エネルギーとする.
</p>
$$
\begin{align}
E &= N_{\rm AA}e_{\rm AA} + N_{\rm BB}e_{\rm BB} + N_{\rm AB}e_{\rm AB} \tag{1}
\end{align}
$$
<p>
第 1 近接の結合原子数（配位数）を $z$ とすると $N_{\rm AA}$ と $N_{\rm BB}$
は次式で表される.
</p>
$$
\begin{align}
N_{\rm AA} &= \frac{1}{2}zN_{\rm A} - \frac{1}{2}N_{\rm AB} \\
N_{\rm BB} &= \frac{1}{2}zN_{\rm B} - \frac{1}{2}N_{\rm AB} \tag{2}
\end{align}
$$
<p>
（2）を（1）に代入すると, Bragg-Williams 近似の混合エンタルピーが得られる. 
</p>
$$
\begin{align}
E &= \biggl(\frac{1}{2}zN_{\rm A} - \frac{1}{2}N_{\rm AB}\biggr)e_{\rm AA}
+ \biggl(\frac{1}{2}zN_{\rm B} - \frac{1}{2}N_{\rm AB}\biggr)e_{\rm BB}
+ N_{\rm AB}e_{\rm AB} \\
&= \frac{1}{2}z \textcolor{green}{N_{\rm A}} e_{\rm AA} + \frac{1}{2}z \textcolor{green}{N_{\rm B}} e_{\rm BB}
+ \textcolor{green}{N_{\rm AB}} \biggl\{ e_{\rm AB} - \frac{e_{\rm AA} + e_{\rm BB}}{2}\biggr\} \\
&= \frac{1}{2}z \textcolor{red}{N x_{\rm A}} e_{\rm AA}  + \frac{1}{2} z \textcolor{red}{N x_{\rm B}} e_{\rm BB} 
+\textcolor{red}{z N x_{\rm A}x_{\rm B}} \biggl\{ e_{\rm AB} - \frac{e_{\rm AA} + e_{\rm BB}}{2}\biggr\} \\
&\equiv E_{\rm m}^{\rm A}Nx_{\rm A} + E_{\rm m}^{\rm B}Nx_{\rm B} + \Omega_{AB}Nx_{\rm A}x_{\rm B} \tag{3}
\end{align}
$$
<span style="color: blue;">
<p>
<u>（2）の導出</u></br></br>
B 元素 1 ヶに近接する A 元素の平均数は $zx_{A}$ なので, B 元素 $N_{\rm B}$ ヶと結合を形成する
A - B 対の平均数 $N_{\rm AB}$ は $N_{\rm AB} = N_{\rm B}zx_{\rm A} = zNx_{\rm A}x_{\rm B}$ となる.
このように原子対の平均数でエンタルピーを表すので平均場近似とよばれる.
</p> 
<p>
$N_{\rm AA}$ についても同様に $N_{\rm AA}=N_{\rm A}zx_{\rm A}/2$ となる.
$1/2$ は結合数のダブルカウントを打ち消すために必要である. $N_{\rm A} = Nx_{\rm A} = (1-x_{\rm B})N$ より,
$N_{\rm AA} = zN(1-x_{\rm B})x_{\rm A}/2 = zNx_{\rm A}/2-zNx_{\rm A}x_{\rm B}/2 = zN_{\rm A}/2-N_{\rm AB}/2$.
</p>
</span>

