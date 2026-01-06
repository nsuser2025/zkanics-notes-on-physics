<p>
LAMMPSインプットにfix bond/reactを指定するのは1回だけ.
反応AとBを同時にシミュレーションするときは fix bond/reactでreact A, react B
と記載する.
</p>

<p>
<strong>
fix bond/reactのワークフロー  
</strong></br>  
1. シミュレーションする反応を特定する.</br>
2. 反応が起こる前の反応部位の分子テンプレートを作成する.</br>
3. 反応が起こった後の反応部位の分子テンプレートを作成する.</br>
4. 反応前後の分子テンプレート間で, 各原子のテンプレートIDを対応付けるマップを作成する.</br>
5. シミュレーションボックスを分子で埋め, fix bond/reactを使ってシミュレーションを実行する.</br>  
</p>

#### stabilization

<p>
<span style="color: red;">
フォーマット: stabilization yes/no group-ID xmax
</span></br>
stabilization yes（デフォルトではno）を指定するとfix bond/react
は2つの原子グループを作成する.
</p>

<p>
<strong>第1グループ</strong> $\cdots$ 反応に関与しているすべての原子 </br>
インプットに明記されていなくてもnve/limitが自動で適用される.</br></br>
<strong>第2グループ</strong> $\cdots$ 反応に関与していないすべての原子 </br>
stabilizationキーワードで指定したgroup-IDに_REACTを付加したものとして定義される.  
</p>
