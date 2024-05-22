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
[fv-az1543-369:41366] *** Process received signal ***
[fv-az1543-369:41366] Signal: Aborted (6)
[fv-az1543-369:41366] Signal code:  (-6)
[fv-az1543-369:41366] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1fa7042520]
[fv-az1543-369:41366] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1fa70969fc]
[fv-az1543-369:41366] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1fa7042476]
[fv-az1543-369:41366] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1fa70287f3]
[fv-az1543-369:41366] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1fa74a2b9e]
[fv-az1543-369:41366] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1fa74ae20c]
[fv-az1543-369:41366] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1fa74ae277]
[fv-az1543-369:41366] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1fa74ae52b]
[fv-az1543-369:41366] [ 8] plumed(+0x12f48)[0x5582e5d43f48]
[fv-az1543-369:41366] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1fa7029d90]
[fv-az1543-369:41366] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1fa7029e40]
[fv-az1543-369:41366] [11] plumed(+0x131e5)[0x5582e5d441e5]
[fv-az1543-369:41366] *** End of error message ***
</pre>
{% endraw %}
