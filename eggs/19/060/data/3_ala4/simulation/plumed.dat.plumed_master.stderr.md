**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  3_ala4/simulation/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: NN_VES TEMP=300.0 LABEL=bias ARG=phi1,phi2,phi3,psi1,psi2,psi3 NODES=96,48,24 OPTIM=ADAM ACTIVATION=RELU GRID_MIN=-pi,-pi,-pi,-pi,-pi,-pi GRID_MAX=pi,pi,pi,pi,pi,pi GRID_BIN=300,300,300,300,300,300 AVE_STRIDE=500 PRINT_STRIDE=100 TARGET_STRIDE=1 LRATE=0.001 GAMMA=10 TAU_KL=100000 MODE_DECAY=4 DECAY_STEP_START=10000 DECAY=2000 ADAPTIVE_DECAY=20 MC_POINTS=20000 MC_SIGMA=0.5,0.5,0.5,0.5,0.5,0.5 CALC_MC_ERR=0 MC_CONVERGENCE_TEST=0 L2_weight=0.2 SERIAL CALC_RCT
Maybe a missing space or a typo?
[fv-az99-305:36089] *** Process received signal ***
[fv-az99-305:36089] Signal: Aborted (6)
[fv-az99-305:36089] Signal code:  (-6)
[fv-az99-305:36089] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f743227c210]
[fv-az99-305:36089] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f743227c18b]
[fv-az99-305:36089] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f743225b859]
[fv-az99-305:36089] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f74324e3951]
[fv-az99-305:36089] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f74324ef47c]
[fv-az99-305:36089] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f74324ef4e7]
[fv-az99-305:36089] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f74324ef7ed]
[fv-az99-305:36089] [ 7] plumed_master(+0xf568)[0x5597df589568]
[fv-az99-305:36089] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f743225d0b3]
[fv-az99-305:36089] [ 9] plumed_master(+0xf79e)[0x5597df58979e]
[fv-az99-305:36089] *** End of error message ***
</pre>
{% endraw %}
