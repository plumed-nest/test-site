**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  1_wolfe_quapp_potential/single_replica/inputs/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: NN_VES LABEL=nn ARG=p.x NODES=48,24,12 OPTIM=ADAM ACTIVATION=RELU GRID_MIN=-3. GRID_MAX=3. GRID_BIN=50 TEMP=1. AVE_STRIDE=500 PRINT_STRIDE=1000 TARGET_STRIDE=1 GAMMA=10 LRATE=0.001 TAU_KL=50000 DECAY=5000 ADAPTIVE_DECAY=0.5
Maybe a missing space or a typo?
[fv-az99-305:36033] *** Process received signal ***
[fv-az99-305:36033] Signal: Aborted (6)
[fv-az99-305:36033] Signal code:  (-6)
[fv-az99-305:36033] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efc86f11210]
[fv-az99-305:36033] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efc86f1118b]
[fv-az99-305:36033] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efc86ef0859]
[fv-az99-305:36033] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efc87178951]
[fv-az99-305:36033] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efc8718447c]
[fv-az99-305:36033] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efc871844e7]
[fv-az99-305:36033] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7efc87184799]
[fv-az99-305:36033] [ 7] plumed(+0xf47d)[0x55701e34147d]
[fv-az99-305:36033] [ 8] plumed(+0x14004)[0x55701e346004]
[fv-az99-305:36033] [ 9] plumed(+0xf698)[0x55701e341698]
[fv-az99-305:36033] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efc86ef20b3]
[fv-az99-305:36033] [11] plumed(+0xf76e)[0x55701e34176e]
[fv-az99-305:36033] *** End of error message ***
</pre>
{% endraw %}
