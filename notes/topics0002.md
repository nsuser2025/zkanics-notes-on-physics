### Ergun式

<p>
固体粒子で満たされた充填層（packed bed）の圧損はErgun式で評価される.
</p>

$$
\begin{align}
\frac{\Delta P}{L}
&= \frac{150 \mu (1-\epsilon)^{2}}{D^{2}\_{p}\epsilon^{3}}u
+\frac{1.75 \rho (1-\epsilon)}{D\_{p} \epsilon^{3}}u^{2} \tag{1}
\end{align}
$$

$\Delta p / L$: 圧力勾配 [Pa/m]
$\mu$: 流体動粘性係数 [Pa$\cdot$s]
$\rho$: 流体密度 [kg/m$^{3}$]
$\epsilon$: 空隙率（0.36-0.40）
$D_{p}$: ペレット代表粒径 [m]
$u \equiv$ 体積流量/断面積: 表面流速（superficial velocity）[m/s]

<p>
第1項: 粘性抵抗項 ... 低流速な層流領域で支配的な抵抗で, 粘性摩擦に起因する（Kozeny-Carmanの式）.
</p>
<p>
第2項: 運動量抵抗項 ... 高流速な乱流領域で支配的な抵抗で, 流体の運動量変化に起因する（Burke-Plummerの式）.
</p>

<p>
空隙率は実験値から求める必要があるが, ランダムな充填であれば0.36-0.4が使われる.
規則配列ならより密につまるので更に小さくなる.

</p>

---
### 充填層を形成する固体粒子形状と生じる流れ

<p>
1. 粒間空隙を通る流れ $\rightarrow$ Ergun式で記述できる.
</p>
<p>
2. ペレットを流れる短絡流 $\rightarrow$ 実効圧損はErgun式の値より低くなる傾向がある.
</p>

---
### Brinkman-Forchheimer モデル

<p>
Navier–Stokes方程式を多孔質体に適用するために修正したモデル.
</p>

$$
\begin{align}
\frac{\Delta p}{L} &= \frac{\mu}{K} u
+ \frac{\rho F^{2}}{\sqrt{K}}
\end{align}
$$
