#### src/makefile/Makefile.gfortran_mpi の編集
<p>
変更箇所 1: </br>   
NUMLIB = -L/home/XXX/MATHLIB/lapack-3.5.0 -llapack -lrefblas に変更する.  
</p>  
<p>
変更箇所 2: </br>  
&#36;(FC) -DPARALLEL -O2 -fexternal-blas <span style="color:red;">-fallow-argument-mismatch</span> &#36;(DEBUG) \ </br>
<span style="color:red;"> -fallow-argument-mismatch </span> ...　</br> </br>
mpif90のバージョンによっては, -fallow-argument-mismatch（赤文字）が廃止されているので消去する.
</p>

#### src/parallel.F90 の編集
