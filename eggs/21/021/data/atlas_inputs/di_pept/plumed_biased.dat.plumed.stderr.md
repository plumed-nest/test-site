**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/di_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATLAS LABEL=at REFERENCE=cluster_plumed.dat PACE=500 ARG=t1,t2 SIGMA=0.10 BIASFACTOR=10 HEIGHT=2.0 GRID_MAX=5.0 GRID_BIN=500 TEMP=300 TRUNCATE_GRIDS REGULARISE=1E-6 STATIC_WALL=0.0 ADAPTIVE_WALL=1.0
Maybe a missing space or a typo?
[fv-az979-741:06906] *** Process received signal ***
[fv-az979-741:06906] Signal: Aborted (6)
[fv-az979-741:06906] Signal code:  (-6)
[fv-az979-741:06906] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fddb7242520]
[fv-az979-741:06906] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fddb72969fc]
[fv-az979-741:06906] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fddb7242476]
[fv-az979-741:06906] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fddb72287f3]
[fv-az979-741:06906] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fddb76a4f26]
[fv-az979-741:06906] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fddb76b6d9c]
[fv-az979-741:06906] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fddb76b6e07]
[fv-az979-741:06906] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fddb76b70bb]
[fv-az979-741:06906] [ 8] plumed(+0x12f48)[0x560be595bf48]
[fv-az979-741:06906] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fddb7229d90]
[fv-az979-741:06906] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fddb7229e40]
[fv-az979-741:06906] [11] plumed(+0x131e5)[0x560be595c1e5]
[fv-az979-741:06906] *** End of error message ***
</pre>
{% endraw %}
