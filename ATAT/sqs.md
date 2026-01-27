<p>
<u>Special Quasi-random Structure（SQS）</u></br>
SQS とは理想溶体の相関関数をスーパーセルで再現するように設計された構造である.
合金系の DFT や MD では理想溶体の初期構造が必要になるが,
結晶格子の各サイトに一様乱数で原子を配置するだけでは乱数シード依存性が現れてしまう.
この依存性は用意した多数のランダム配置に対して統計平均を取ることで低減できるが,
DFT や MD では計算コストが極めて高く現実的ではない.
また, 周期構造を用いると人工的な長距離相関（周期性誤差）
が入り込んでしまう. そこで, スーパーセルで理想溶体の相関関数をできるだけ正確に再現するよう設計された SQS 
が用いられる. 仮に理想溶体の全ての相関関数を完全に再現する SQS
が設計できたとすれば その単一構造から計算される物性は,
多数のランダム配置に対する統計平均の極限値と一致する.</br></br>
REFS/Zunger1990_Phys.Rev.Lett.vol65.353
</p>
<span style="color: blue;">
<p>
<u>二元理想溶体の相関関数</u></br>
二元理想溶体 A$_{1-x}$B$_{x}$ の 第 $m$ 近接の $k$
体クラスター相関関数 $\langle \Pi_{k,m} \rangle$ は</br> 
</p>
$$
\begin{align}
\langle \Pi_{k,m} \rangle 
&= \biggl\langle \prod_{i \in f(k,m)} S_{i} \biggr\rangle
= \prod_{i \in f(k,m)} \langle S_{i} \rangle 
= \langle S_{1} \rangle  \langle S_{2} \rangle \cdots \langle S_{k} \rangle
= (2x-1)^{k} \tag{1}
\end{align}
$$
ここで, 理想溶体の $\langle S_{i} \rangle$ は
$$
\begin{align}
\langle S_{i} \rangle &= S^{\rm A}_{i} P({\rm A}) + S^{\rm B}_{i} P({\rm B})
= (-1)(1-x) + (+1)x = 2x - 1 \tag{2}
\end{align}
$$

</span>
<span style="color: blue;">
<p>
<u>周期性誤差</u></br>
PBC を用いると, ランダムであれば隣のセルのある位置にどの原子が配置されるかは不確定であるはずだが,
周期性によりそれが確定してしまう. つまり, 長距離においてもランダムな相関は得られず,
人工的な相関が生じてしまう.
</p>
</span>
