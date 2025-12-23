### ランダウの相転移理論

<p>
秩序パラメータ（フェーズフィールド法ではフェーズフィールド変数）を用いて自由エネルギーを定式化する
相転移の現象論である. 特に2次相転移の記述に有効である.
しかし, 秩序パラメータの平均値のみを用いる平均場理論であるため, 
臨界揺らぎが支配的となる臨界温度 $T_{\rm c}$ 付近では破綻する. 
</p>

### フェーズフィールド法の計算フロー

<p>
1. 相変数 $\phi$ に対する自由エネルギー汎関数 $F[\phi]$ を定義する.
</p>
<p>
2. 変分により化学ポテンシャル $\mu = \delta F / \delta \phi$ を導出する.
</p>
<p>
3. 系の保存性に応じてAllen-Cahn方程式とCahn-Hilliard方程式を用いて $\phi$ の時間発展を数値的に解く.
</p>
 
---

### Allen-Cahn方程式（非保存量の時間発展）

$$
\begin{align}
\frac{\partial \phi}{\partial t}
&= -L \mu
\end{align}
$$

---

### Cahn-Hilliard方程式（保存量の時間発展）

$$
\begin{align}
\frac{\partial \phi}{\partial t}
&= \nabla\cdot(M\nabla \mu)
\end{align}
$$

---
