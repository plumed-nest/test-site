**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/tetra_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATLAS LABEL=at REFERENCE=cluster_plumed.dat PACE=500 ARG=t1,t2,t3,t4,t5,t6 SIGMA=0.1 BIASFACTOR=10 HEIGHT=2.0 GRID_MAX=3.5 GRID_BIN=500 TEMP=300 TRUNCATE_GRIDS REGULARISE=1E-12 STATIC_WALL=0.00 ADAPTIVE_WALL=1.00
Maybe a missing space or a typo?
[fv-az1110-714:71889] *** Process received signal ***
[fv-az1110-714:71889] Signal: Aborted (6)
[fv-az1110-714:71889] Signal code:  (-6)
[fv-az1110-714:71889] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb11d842520]
[fv-az1110-714:71889] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb11d8969fc]
[fv-az1110-714:71889] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb11d842476]
[fv-az1110-714:71889] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb11d8287f3]
[fv-az1110-714:71889] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb11dca2b9e]
[fv-az1110-714:71889] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb11dcae20c]
[fv-az1110-714:71889] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb11dcae277]
[fv-az1110-714:71889] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb11dcae52b]
[fv-az1110-714:71889] [ 8] plumed(+0x12f48)[0x55b8e0821f48]
[fv-az1110-714:71889] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb11d829d90]
[fv-az1110-714:71889] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb11d829e40]
[fv-az1110-714:71889] [11] plumed(+0x131e5)[0x55b8e08221e5]
[fv-az1110-714:71889] *** End of error message ***
</pre>
{% endraw %}
