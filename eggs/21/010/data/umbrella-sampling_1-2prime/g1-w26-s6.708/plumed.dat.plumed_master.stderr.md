**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w26-s6.708/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az529-343:07432] *** Process received signal ***
[fv-az529-343:07432] Signal: Aborted (6)
[fv-az529-343:07432] Signal code:  (-6)
[fv-az529-343:07432] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4d66042520]
[fv-az529-343:07432] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4d660969fc]
[fv-az529-343:07432] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4d66042476]
[fv-az529-343:07432] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4d660287f3]
[fv-az529-343:07432] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f4d664a4f26]
[fv-az529-343:07432] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f4d664b6d9c]
[fv-az529-343:07432] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f4d664b6e07]
[fv-az529-343:07432] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4d664b70bb]
[fv-az529-343:07432] [ 8] plumed_master(+0x12ebf)[0x556b831d8ebf]
[fv-az529-343:07432] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4d66029d90]
[fv-az529-343:07432] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4d66029e40]
[fv-az529-343:07432] [11] plumed_master(+0x13155)[0x556b831d9155]
[fv-az529-343:07432] *** End of error message ***
</pre>
{% endraw %}
