#### fix bond/reactの動作イメージ

<p>
1. 指定原子対間の距離 r が Rmin $\le$ r $\le$ Rmax にあるかをチェックする.</br>
2. 近づいたら, 結合ネットワークが反応前テンプレートと一致しているかを検証する.</br>
3. 一致していたら, 反応後テンプレートに記載の構造に置き換える.</br>
4. 結合が生成した瞬間の不自然な構造歪みを nve/limit で安定化させる.</br>
</p>

<p>
4 を実行するには stabilization yes にする.</br>
$\rightarrow$ no にしてしまうと置き換え直後の原子の挙動が不自然になることがある.
</p>

---

#### fix bond/reactのワークフロー

<p>  
1. シミュレーションする反応を定義する.</br>
2. 反応前の反応部位テンプレートを作成する.</br>
3. 反応後の反応部位テンプレートを作成する.</br>
4. 反応前後のテンプレートで, 同一原子を対応付けたマップを作成する.</br>
5. fix bond/react を使ってシミュレーションを実行する.</br>  
</p>

<p>
反応前後のテンプレイートとマップの作製を自動で行うツール $\cdots$ AutoMapper  
</p>

---

#### Refs.

<p>
Gissinger2017_Polymer.vol128.211 </br>
Gissinger2020_Macromolecules.vol53.9953 </br>
Gissinger2024_Comput.Phys.Commun.vol304.109287 </br>
Gissinger2024_J.Phys.Chem.B.vol128.3282 </br> 
</p>
