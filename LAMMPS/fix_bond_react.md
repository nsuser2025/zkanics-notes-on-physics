#### fix bond/reactの動作イメージ

<p>
1. スキャン $\cdots$ スキャン対象として指定した原子対の距離rがRmin$\geq$ r $leq$ Rmax 
にあるかをチェック.</br>
2. 検証 $\cdots$ 
</p>
#### fix bond/reactのワークフロー
<p>  
1. シミュレーションする反応を特定する.</br>
2. 反応が起こる前の反応部位の分子テンプレートを作成する.</br>
3. 反応が起こった後の反応部位の分子テンプレートを作成する.</br>
4. 反応前後の分子テンプレート間で, 各原子のテンプレートIDを対応付けるマップを作成する.</br>
5. シミュレーションボックスを分子で埋め, fix bond/reactを使ってシミュレーションを実行する.</br>  
</p>

---

#### stabilizationキーワード  

<p>
stabilization yes/no group-ID xmax </br>
stabilization yes（デフォルトではno）を指定するとfix bond/react
は2つの原子グループを作成する.
</p>
<p>
第1グループ: 反応に関与しているすべての原子.
インプットに明記されていなくてもnve/limitが自動で適用される.
xmaxはfix nve/limitで指定するxmaxと同じ.</br>
第2グループ: 反応に関与していないすべての原子.
group-IDに_REACTを付加したものとして定義される.  
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
