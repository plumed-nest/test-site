**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_2d/pca_2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATLAS LABEL=rr ARG=d1.x,d1.y REFERENCE=cluster.dat PACE=500 SIGMA=0.20 BIASFACTOR=10 HEIGHT=2.0 GRID_MAX=6.0 GRID_BIN=600 TEMP=1 TRUNCATE_GRIDS REGULARISE=0.00000001 STATIC_WALL=0.0 ADAPTIVE_WALL=1.0
Maybe a missing space or a typo?
[fv-az1110-714:71636] *** Process received signal ***
[fv-az1110-714:71636] Signal: Aborted (6)
[fv-az1110-714:71636] Signal code:  (-6)
[fv-az1110-714:71636] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe096642520]
[fv-az1110-714:71636] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe0966969fc]
[fv-az1110-714:71636] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe096642476]
[fv-az1110-714:71636] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe0966287f3]
[fv-az1110-714:71636] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe096aa2b9e]
[fv-az1110-714:71636] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe096aae20c]
[fv-az1110-714:71636] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe096aae277]
[fv-az1110-714:71636] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe096aae52b]
[fv-az1110-714:71636] [ 8] plumed(+0x12f48)[0x5594cb0fbf48]
[fv-az1110-714:71636] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe096629d90]
[fv-az1110-714:71636] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe096629e40]
[fv-az1110-714:71636] [11] plumed(+0x131e5)[0x5594cb0fc1e5]
[fv-az1110-714:71636] *** End of error message ***
</pre>
{% endraw %}
