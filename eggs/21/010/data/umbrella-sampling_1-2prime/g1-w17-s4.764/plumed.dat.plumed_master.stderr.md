**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w17-s4.764/plumed.dat   
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
[fv-az529-343:07116] *** Process received signal ***
[fv-az529-343:07116] Signal: Aborted (6)
[fv-az529-343:07116] Signal code:  (-6)
[fv-az529-343:07116] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7626642520]
[fv-az529-343:07116] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f76266969fc]
[fv-az529-343:07116] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7626642476]
[fv-az529-343:07116] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f76266287f3]
[fv-az529-343:07116] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7626aa4f26]
[fv-az529-343:07116] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7626ab6d9c]
[fv-az529-343:07116] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7626ab6e07]
[fv-az529-343:07116] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7626ab70bb]
[fv-az529-343:07116] [ 8] plumed_master(+0x12ebf)[0x55b41928febf]
[fv-az529-343:07116] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7626629d90]
[fv-az529-343:07116] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7626629e40]
[fv-az529-343:07116] [11] plumed_master(+0x13155)[0x55b419290155]
[fv-az529-343:07116] *** End of error message ***
</pre>
{% endraw %}
