#### src/makefile/Makefile.gfortran_mpi の編集

<p>
赤文字を消去する.  
</p>
<p>
$(FC) -DPARALLEL -O2 -fexternal-blas <span style="color:red;">-fallow-argument-mismatch</span> $(DEBUG) \ </br>
<span style="color:red;"> -fallow-argument-mismatch </span> $< -o $@
</p>

#### src/parallel.F90 の編集
