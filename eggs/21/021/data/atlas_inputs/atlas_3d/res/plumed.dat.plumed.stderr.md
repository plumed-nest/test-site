**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_3d/res/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATLAS LABEL=rr ARG=d1.x,d1.y,d1.z REFERENCE=cluster.dat PACE=500 SIGMA=0.2 BIASFACTOR=10 HEIGHT=3.0 GRID_MAX=5.0 GRID_BIN=500 TEMP=1 TRUNCATE_GRIDS REGULARISE=1E-8 ADAPTIVE_WALL=1.0 STATIC_WALL=0.0
Maybe a missing space or a typo?
[fv-az979-741:06779] *** Process received signal ***
[fv-az979-741:06779] Signal: Aborted (6)
[fv-az979-741:06779] Signal code:  (-6)
[fv-az979-741:06779] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8912e42520]
[fv-az979-741:06779] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8912e969fc]
[fv-az979-741:06779] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8912e42476]
[fv-az979-741:06779] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8912e287f3]
[fv-az979-741:06779] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f89132a4f26]
[fv-az979-741:06779] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f89132b6d9c]
[fv-az979-741:06779] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f89132b6e07]
[fv-az979-741:06779] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f89132b70bb]
[fv-az979-741:06779] [ 8] plumed(+0x12f48)[0x55a01c613f48]
[fv-az979-741:06779] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8912e29d90]
[fv-az979-741:06779] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8912e29e40]
[fv-az979-741:06779] [11] plumed(+0x131e5)[0x55a01c6141e5]
[fv-az979-741:06779] *** End of error message ***
</pre>
{% endraw %}
