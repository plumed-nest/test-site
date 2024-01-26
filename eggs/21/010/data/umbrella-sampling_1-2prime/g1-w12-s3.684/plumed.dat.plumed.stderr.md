**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w12-s3.684/plumed.dat   
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
[fv-az529-343:06951] *** Process received signal ***
[fv-az529-343:06951] Signal: Aborted (6)
[fv-az529-343:06951] Signal code:  (-6)
[fv-az529-343:06951] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0731c42520]
[fv-az529-343:06951] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0731c969fc]
[fv-az529-343:06951] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0731c42476]
[fv-az529-343:06951] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0731c287f3]
[fv-az529-343:06951] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f07320a4f26]
[fv-az529-343:06951] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f07320b6d9c]
[fv-az529-343:06951] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f07320b6e07]
[fv-az529-343:06951] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f07320b70bb]
[fv-az529-343:06951] [ 8] plumed(+0x12f48)[0x55fa83139f48]
[fv-az529-343:06951] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0731c29d90]
[fv-az529-343:06951] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0731c29e40]
[fv-az529-343:06951] [11] plumed(+0x131e5)[0x55fa8313a1e5]
[fv-az529-343:06951] *** End of error message ***
</pre>
{% endraw %}
