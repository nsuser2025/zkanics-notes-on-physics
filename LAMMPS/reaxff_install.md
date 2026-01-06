#### ReaxFFとfix bond/reactを使うためのLAMMPSインストール

<p>
cmake ../cmake -D BUILD_MPI=on \ </br>
-D PKG_MOLECULE=on \ </br> 
-D PKG_MC=on \ </br>
-D PKG_MISC=on \ </br>
-D PKG_EXTRA-FIX=on \ </br>
-D PKG_KSPACE=on \ </br>
-D PKG_REAXFF=on \ </br>
-D PKG_CLASS2=on \ </br>
-D PKG_REACTION=on
</p>

<p>
make </br>
make install
</p>
