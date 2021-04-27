**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  1_wolfe_quapp_potential/single_replica/inputs/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: NN_VES LABEL=nn ARG=p.x NODES=48,24,12 OPTIM=ADAM ACTIVATION=RELU GRID_MIN=-3. GRID_MAX=3. GRID_BIN=50 TEMP=1. AVE_STRIDE=500 PRINT_STRIDE=1000 TARGET_STRIDE=1 GAMMA=10 LRATE=0.001 TAU_KL=50000 DECAY=5000 ADAPTIVE_DECAY=0.5
Maybe a missing space or a typo?
[fv-az99-305:36041] *** Process received signal ***
[fv-az99-305:36041] Signal: Aborted (6)
[fv-az99-305:36041] Signal code:  (-6)
[fv-az99-305:36041] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f276abe2210]
[fv-az99-305:36041] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f276abe218b]
[fv-az99-305:36041] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f276abc1859]
[fv-az99-305:36041] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f276ae49951]
[fv-az99-305:36041] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f276ae5547c]
[fv-az99-305:36041] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f276ae554e7]
[fv-az99-305:36041] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f276ae557ed]
[fv-az99-305:36041] [ 7] plumed_master(+0xf568)[0x559b065f9568]
[fv-az99-305:36041] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f276abc30b3]
[fv-az99-305:36041] [ 9] plumed_master(+0xf79e)[0x559b065f979e]
[fv-az99-305:36041] *** End of error message ***
</pre>
{% endraw %}
