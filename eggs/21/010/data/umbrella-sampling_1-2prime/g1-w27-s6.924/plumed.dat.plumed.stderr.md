**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w27-s6.924/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az529-343:07455] *** Process received signal ***
[fv-az529-343:07455] Signal: Aborted (6)
[fv-az529-343:07455] Signal code:  (-6)
[fv-az529-343:07455] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa883842520]
[fv-az529-343:07455] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa8838969fc]
[fv-az529-343:07455] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa883842476]
[fv-az529-343:07455] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa8838287f3]
[fv-az529-343:07455] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa883ca4f26]
[fv-az529-343:07455] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa883cb6d9c]
[fv-az529-343:07455] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa883cb6e07]
[fv-az529-343:07455] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa883cb70bb]
[fv-az529-343:07455] [ 8] plumed(+0x12f48)[0x564a83994f48]
[fv-az529-343:07455] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa883829d90]
[fv-az529-343:07455] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa883829e40]
[fv-az529-343:07455] [11] plumed(+0x131e5)[0x564a839951e5]
[fv-az529-343:07455] *** End of error message ***
</pre>
{% endraw %}
