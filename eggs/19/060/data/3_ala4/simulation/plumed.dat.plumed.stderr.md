**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  3_ala4/simulation/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: NN_VES TEMP=300.0 LABEL=bias ARG=phi1,phi2,phi3,psi1,psi2,psi3 NODES=96,48,24 OPTIM=ADAM ACTIVATION=RELU GRID_MIN=-pi,-pi,-pi,-pi,-pi,-pi GRID_MAX=pi,pi,pi,pi,pi,pi GRID_BIN=300,300,300,300,300,300 AVE_STRIDE=500 PRINT_STRIDE=100 TARGET_STRIDE=1 LRATE=0.001 GAMMA=10 TAU_KL=100000 MODE_DECAY=4 DECAY_STEP_START=10000 DECAY=2000 ADAPTIVE_DECAY=20 MC_POINTS=20000 MC_SIGMA=0.5,0.5,0.5,0.5,0.5,0.5 CALC_MC_ERR=0 MC_CONVERGENCE_TEST=0 L2_weight=0.2 SERIAL CALC_RCT
Maybe a missing space or a typo?
[fv-az99-305:36081] *** Process received signal ***
[fv-az99-305:36081] Signal: Aborted (6)
[fv-az99-305:36081] Signal code:  (-6)
[fv-az99-305:36081] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fcdc5790210]
[fv-az99-305:36081] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fcdc579018b]
[fv-az99-305:36081] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fcdc576f859]
[fv-az99-305:36081] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fcdc59f7951]
[fv-az99-305:36081] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fcdc5a0347c]
[fv-az99-305:36081] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fcdc5a034e7]
[fv-az99-305:36081] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fcdc5a03799]
[fv-az99-305:36081] [ 7] plumed(+0xf47d)[0x55a559ddf47d]
[fv-az99-305:36081] [ 8] plumed(+0x14004)[0x55a559de4004]
[fv-az99-305:36081] [ 9] plumed(+0xf698)[0x55a559ddf698]
[fv-az99-305:36081] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fcdc57710b3]
[fv-az99-305:36081] [11] plumed(+0xf76e)[0x55a559ddf76e]
[fv-az99-305:36081] *** End of error message ***
</pre>
{% endraw %}
