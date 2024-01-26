**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_6d/pca_1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATLAS LABEL=at ARG=d1.x,d1.y,d1.z,d2.x,d2.y,d2.z REFERENCE=cluster.dat PACE=500 SIGMA=0.2 BIASFACTOR=15 HEIGHT=3.0 GRID_MAX=7.0 GRID_BIN=500 TEMP=1 TRUNCATE_GRIDS REGULARISE=1E-10 ADAPTIVE_WALL=1.0 STATIC_WALL=0.0
Maybe a missing space or a typo?
[fv-az979-741:06810] *** Process received signal ***
[fv-az979-741:06810] Signal: Aborted (6)
[fv-az979-741:06810] Signal code:  (-6)
[fv-az979-741:06810] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f65b3a42520]
[fv-az979-741:06810] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f65b3a969fc]
[fv-az979-741:06810] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f65b3a42476]
[fv-az979-741:06810] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f65b3a287f3]
[fv-az979-741:06810] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f65b3ea4f26]
[fv-az979-741:06810] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f65b3eb6d9c]
[fv-az979-741:06810] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f65b3eb6e07]
[fv-az979-741:06810] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f65b3eb70bb]
[fv-az979-741:06810] [ 8] plumed(+0x12f48)[0x559c815dbf48]
[fv-az979-741:06810] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f65b3a29d90]
[fv-az979-741:06810] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f65b3a29e40]
[fv-az979-741:06810] [11] plumed(+0x131e5)[0x559c815dc1e5]
[fv-az979-741:06810] *** End of error message ***
</pre>
{% endraw %}
