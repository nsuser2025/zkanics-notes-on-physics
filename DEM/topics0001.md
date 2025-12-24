#### 離散要素法（Discrete Element Method）

#### LAMMPS GRANULAR (examples/granular/in.pour.drum)

<p>
回転ドラム粉体特性試験の DEM 再現  
</p>

<p>
1. 円筒ドラム形状を region で定義  
</p>
<p>
2. 2種類の球状粒子を上から投入（pour）  
</p>
<p>
Type 1: 非凝集  
</p>
<p>
Type 2: 凝集性あり（JKR）  
</p>

<p>
3. z 方向重力で充填  
</p>
<p>
4. 余分な粒子を削除  
</p>
<p>
5. 上蓋を追加  
</p>
<p>
6. 重力方向を切り替えてドラムを「横倒し」  
</p>
<p>
7. region の回転＋重力切替で回転ドラム実験を模擬  
</p>
