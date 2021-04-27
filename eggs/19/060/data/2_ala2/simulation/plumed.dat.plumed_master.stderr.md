**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  2_ala2/simulation/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: NN_VES LABEL=nn ARG=phi NODES=48,24,12 OPTIM=ADAM ACTIVATION=RELU GRID_MIN=-pi GRID_MAX=pi GRID_BIN=50 TEMP=300. AVE_STRIDE=500 PRINT_STRIDE=1000 TARGET_STRIDE=1 GAMMA=10 LRATE=0.001 TAU_KL=10000 DECAY=1000 ADAPTIVE_DECAY=0.5
Maybe a missing space or a typo?
[fv-az99-305:36065] *** Process received signal ***
[fv-az99-305:36065] Signal: Aborted (6)
[fv-az99-305:36065] Signal code:  (-6)
[fv-az99-305:36065] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f91080df210]
[fv-az99-305:36065] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f91080df18b]
[fv-az99-305:36065] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f91080be859]
[fv-az99-305:36065] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9108346951]
[fv-az99-305:36065] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f910835247c]
[fv-az99-305:36065] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f91083524e7]
[fv-az99-305:36065] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f91083527ed]
[fv-az99-305:36065] [ 7] plumed_master(+0xf568)[0x561eaf356568]
[fv-az99-305:36065] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f91080c00b3]
[fv-az99-305:36065] [ 9] plumed_master(+0xf79e)[0x561eaf35679e]
[fv-az99-305:36065] *** End of error message ***
</pre>
{% endraw %}
