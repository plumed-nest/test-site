**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  2_ala2/simulation/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: NN_VES LABEL=nn ARG=phi NODES=48,24,12 OPTIM=ADAM ACTIVATION=RELU GRID_MIN=-pi GRID_MAX=pi GRID_BIN=50 TEMP=300. AVE_STRIDE=500 PRINT_STRIDE=1000 TARGET_STRIDE=1 GAMMA=10 LRATE=0.001 TAU_KL=10000 DECAY=1000 ADAPTIVE_DECAY=0.5
Maybe a missing space or a typo?
[fv-az99-305:36057] *** Process received signal ***
[fv-az99-305:36057] Signal: Aborted (6)
[fv-az99-305:36057] Signal code:  (-6)
[fv-az99-305:36057] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f00d9d29210]
[fv-az99-305:36057] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f00d9d2918b]
[fv-az99-305:36057] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f00d9d08859]
[fv-az99-305:36057] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f00d9f90951]
[fv-az99-305:36057] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f00d9f9c47c]
[fv-az99-305:36057] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f00d9f9c4e7]
[fv-az99-305:36057] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f00d9f9c799]
[fv-az99-305:36057] [ 7] plumed(+0xf47d)[0x564962c4f47d]
[fv-az99-305:36057] [ 8] plumed(+0x14004)[0x564962c54004]
[fv-az99-305:36057] [ 9] plumed(+0xf698)[0x564962c4f698]
[fv-az99-305:36057] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f00d9d0a0b3]
[fv-az99-305:36057] [11] plumed(+0xf76e)[0x564962c4f76e]
[fv-az99-305:36057] *** End of error message ***
</pre>
{% endraw %}
