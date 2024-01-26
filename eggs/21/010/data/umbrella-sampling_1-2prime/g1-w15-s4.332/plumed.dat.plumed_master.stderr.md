**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w15-s4.332/plumed.dat   
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
[fv-az529-343:07053] *** Process received signal ***
[fv-az529-343:07053] Signal: Aborted (6)
[fv-az529-343:07053] Signal code:  (-6)
[fv-az529-343:07053] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f87f6842520]
[fv-az529-343:07053] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f87f68969fc]
[fv-az529-343:07053] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f87f6842476]
[fv-az529-343:07053] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f87f68287f3]
[fv-az529-343:07053] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f87f6ca4f26]
[fv-az529-343:07053] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f87f6cb6d9c]
[fv-az529-343:07053] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f87f6cb6e07]
[fv-az529-343:07053] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f87f6cb70bb]
[fv-az529-343:07053] [ 8] plumed_master(+0x12ebf)[0x55b78a07aebf]
[fv-az529-343:07053] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f87f6829d90]
[fv-az529-343:07053] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f87f6829e40]
[fv-az529-343:07053] [11] plumed_master(+0x13155)[0x55b78a07b155]
[fv-az529-343:07053] *** End of error message ***
</pre>
{% endraw %}
