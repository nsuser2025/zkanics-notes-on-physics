#### src/makefile/Makefile.gfortran_mpi の編集

<p>
赤文字を消去する.  
</p>
<p>
&#36;(FC) -DPARALLEL -O2 -fexternal-blas <span style="color:red;">-fallow-argument-mismatch</span> &#36;(DEBUG) \ </br>
<span style="color:red;"> -fallow-argument-mismatch </span> &#36;< -o &#36;@
</p>

#### src/parallel.F90 の編集
