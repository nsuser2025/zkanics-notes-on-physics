#### インストール

<p>
cp -r ./aenet-lammps/USER-AENET ./lammps-stable_2Aug2023/src/ </br>
cp -r ./aenet-lammps/aenet ./lammps-stable_2Aug2023/lib/ </br>
cp -r aenet-master ./lammps-stable_2Aug2023/lib/aenet/aenet </br>
cd lammps-stable_2Aug2023/lib/aenet </br>
patch -u -p1 -d aenet/ < aenet_lammps.patch </br>
cd aenet/src </br>
make -f makefiles/Makefile.gfortran_serial lib </br>
LAMMPS の src ディレクトリに移動 </br>
make yes-user-aenet </br>
make mpi
</p>
<p>
Makefile.gfortran_serial は AENET インストールに従って編集する. </br>  
LAMMPS の version は 2Aug2023 を用いる. 
</p>

---

#### チュートリアル

<p>
Ref. Shimamura2021_Chem.Phys.Lett.vol778.138748 </br>
Supp. Info. に AIMD で生成したトレーニングデータが公開されている.
AENET公式の TiO$_{2}$ チュートリアルには応力テンソルの学習が含まれていないが,
この文献で公開されている xsf ファイルには pressure 行の下に応力テンソルが記載されている.
</p>
