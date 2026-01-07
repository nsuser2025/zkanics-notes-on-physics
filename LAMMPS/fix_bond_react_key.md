#### stabilizationキーワード  

<p>
stabilization yes/no group-ID xmax </br>
yes（デフォルトではno）を指定すると2つの原子グループが作成される.
</p>
<p>
1. 反応に関与している原子グループ: nve/limit が自動で適用される.</br>
xmax は fix nve/limit で指定する xmax と同じ.
</p>
<p>
2. 反応に関与していない原子グループ:
group-ID に _REACT を付加したgroup-IDとして定義される.  
</p>
<p>
<span style="color: blue;">
fix ID group-ID nve/limit xmax </br>
group-IDに含まれる原子に対してNVEアンサンブルのMDを行う.
ただし, 1ステップで原子が移動できる最大距離はxmaxまで.
</span> 
</p>

---

<p>
<strong>
reactキーワード  
</strong>  
</p>
<p>  
LAMMPSインプットにfix bond/reactを指定するのは1回だけ.反応AとBを同時にシミュレーションするときは
fix bond/reactでreact A & react Bと記載する.
</p>
<p>
react react-ID react-group-ID Nevery Rmin Rmax \ </br>
template-ID(pre-reacted) template-ID(post-reacted) map_file individual_keyword values &</br>
react react-ID react-group-ID Nevery Rmin Rmax \ </br>
template-ID(pre-reacted) template-ID(post-reacted) map_file individual_keyword values </br>
</p>
<p>
Rmin $\cdots$ Rminより近い距離にある原子同士は反応候補から除外する.</br>
Rmax $\cdots$ Rmaxより遠い距離にある原子同士は反応候補から除外する.
</p>
