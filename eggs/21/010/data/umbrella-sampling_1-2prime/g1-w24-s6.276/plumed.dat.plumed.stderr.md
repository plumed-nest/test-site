**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w24-s6.276/plumed.dat   
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
[fv-az529-343:07361] *** Process received signal ***
[fv-az529-343:07361] Signal: Aborted (6)
[fv-az529-343:07361] Signal code:  (-6)
[fv-az529-343:07361] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f60e7a42520]
[fv-az529-343:07361] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f60e7a969fc]
[fv-az529-343:07361] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f60e7a42476]
[fv-az529-343:07361] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f60e7a287f3]
[fv-az529-343:07361] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f60e7ea4f26]
[fv-az529-343:07361] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f60e7eb6d9c]
[fv-az529-343:07361] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f60e7eb6e07]
[fv-az529-343:07361] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f60e7eb70bb]
[fv-az529-343:07361] [ 8] plumed(+0x12f48)[0x55766f631f48]
[fv-az529-343:07361] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f60e7a29d90]
[fv-az529-343:07361] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f60e7a29e40]
[fv-az529-343:07361] [11] plumed(+0x131e5)[0x55766f6321e5]
[fv-az529-343:07361] *** End of error message ***
</pre>
{% endraw %}
