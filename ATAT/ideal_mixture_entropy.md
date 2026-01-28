<p>
$N$ ヶの原子を原子サイトに配置させるときの状態数 $W_{\rm mix}$ は同種原子を含む順列問題である.
従って, ランダム分布を仮定した二元固溶体の状態数は次式で表される.
</p>
$$
\begin{align}
W_{\rm mix} &= \frac{N!}{N_{\rm A}!N_{\rm B}!} \tag{1}
\end{align}
$$
<p>
Boltzmann の混合エントロピー $S_{\rm mix} = k\ln W_{\rm mix}$
に代入すると
</p>
$$
\begin{align}
S_{\rm mix} &= k(\ln N! - \ln N_{\rm A}! - \ln N_{\rm B}!) \\
&\approx k(N\ln N - N - (N_{\rm A}\ln N_{\rm A} - N_{\rm A}) 
- (N_{\rm B}\ln N_{\rm B} - N_{\rm B})) \\
&= kN(\ln N - x_{\rm A}\ln N_{\rm A} - x_{\rm B}\ln N_{\rm B}) \\
&= kN((x_{\rm A} + x_{\rm B}) \ln N - x_{\rm A} \ln N_{\rm A} - x_{\rm B} \ln N_{\rm B}) \\
&= -kN (x_{\rm A} \ln x_{\rm A} + x_{\rm B} \ln x_{\rm B}) \tag{2}
\end{align}
$$
<p>
従って, モル混合エントロピー $S_{\rm m}$ は次式となる.
ここで気体定数とボルツマン定数の関係式 $R=kN_{\rm Avo}$ を用いた.
</p>
$$
\begin{align}
S_{\rm m}^{\rm mix} &= N_{\rm Avo} S_{\rm mix} / N \\
&= -kN_{\rm Avo} (x_{\rm A} \ln x_{\rm A} + x_{\rm B} \ln x_{\rm B}) \\
&= -R (x_{\rm A} \ln x_{\rm A} + x_{\rm B} \ln x_{\rm B}) \tag{3}
\end{align}
$$
