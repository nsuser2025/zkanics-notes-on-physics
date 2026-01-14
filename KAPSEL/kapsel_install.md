#### ライブラリ設定（Octa）
<p>
OCTA を展開（$HOME/OCTA/OCTA84）</br>
GOURMET/lib/linux_64/libplatform.a を libplatform_gcc.a にコピーする.
</p>

---

#### FFTW インストール
<p>
./configure CC=gcc CXX=g++ --prefix="XXX" CFLAGS="-O3" \ </br>
FFLAGS="-O3" --enable-openmp --enable-threads \ </br>
--enable-shared --disable-fortran </br>
make & make install
</p>

---

#### HDF5 インストール
<p>
./configure CC=gcc CXX=g++ CFLAGS="-O3" FFLAGS="-O3" \ </br>
--disable-fortran --enable-cxx --prefix="XXX" </br>
make & make install
</p>

---

#### LIS インストール
<p>
./configure CC=gcc CXX=g++ --prefix="XXX" </br>
make & make install
</p>

---

#### KAPSEL インストール
<p>
LIS=ON のコメントを外す. GCC_OMP のライブラリリンクを FFTW, HDF5, LIS の
prefix path に変更する. </br>
make ENV=GCC_OMP FFT=FFTW
</p>
