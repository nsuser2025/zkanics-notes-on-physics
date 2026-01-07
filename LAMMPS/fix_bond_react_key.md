#### stabilization キーワード  

<p>
stabilization yes/no group-ID xmax </br>
yes（デフォルトではno）を指定すると2つの原子グループが作成される.
</p>
<p>
1. 反応に関与している原子グループ </br> 
nve/limit が自動で適用され, xmax は fix nve/limit で指定する xmax と同じ.
</p>
<p>
2. 反応に関与していない原子グループ </br>
group-ID に _REACT を付加した新規 group-ID が定義される.
</p>
<p>
<span style="color: blue;">
fix ID group-ID nve/limit xmax </br>
group-ID に含まれる原子に対して NVE アンサンブルの MD を行う. </br>
ただし, 1 ステップで原子が移動できる最大距離は xmax まで.
</span> 
</p>

---

#### react キーワード  

<p>  
LAMMPS インプットに fix bond/react を指定するのは 1 度だけ. </br>
複数反応を取り扱うときは fix bond/react で下記のようにリストする.
</p>
<p>
react react-ID react-group-ID Nevery Rmin Rmax \ </br>
template-ID(pre-reacted) template-ID(post-reacted) map_file individual_keyword values &</br>
react react-ID react-group-ID Nevery Rmin Rmax \ </br>
template-ID(pre-reacted) template-ID(post-reacted) map_file individual_keyword values </br>
</p>
<p>
Rmin $\cdots$ Rmin より近い距離にある原子同士は反応候補から除外する. </br>
Rmax $\cdots$ Rmax より遠い距離にある原子同士は反応候補から除外 する.
</p>
