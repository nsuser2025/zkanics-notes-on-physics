#### src/makefile/Makefile.gfortran_mpi の編集
<p>
変更箇所 1: </br>   
NUMLIB = -L/home/XXX/MATHLIB/lapack-3.5.0 -llapack -lrefblas に変更する.  
</p>  
<p>
変更箇所 2: </br>  
&#36;(FC) -DPARALLEL -O2 -fexternal-blas <span style="color:red;"><s>-fallow-argument-mismatch</s></span> &#36;(DEBUG) \ </br>
<span style="color:red;"><s>-fallow-argument-mismatch</s></span> ...　</br> </br>
mpif90によっては -fallow-argument-mismatch（赤文字）が廃止されていることがあるので消去する.
</p>

---

#### src/parallel.F90 の編集
<p>
integer, dimension(MPI_STATUS_SIZE) :: status </br>
$\rightarrow$ type(MPI_Status) :: status </br> </br>
use mpi_f08 では stauts の宣言は後者を用いる.   
</p>

---

#### インストール
<p>
cd aenet-master </br>  
cd lib </br>
make </br>
cd ../src </br>
make -f makefile/Makefile.gfortran_mpi </br>
make -f makefile/Makefile.gfortran_mpi lib </br> </br>
aenet-master/bin に generate（single core）, train（MPI）,
predict（MPI）の実行ファイルが生成される.
</p>
