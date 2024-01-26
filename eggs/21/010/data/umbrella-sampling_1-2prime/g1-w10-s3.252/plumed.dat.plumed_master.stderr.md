**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w10-s3.252/plumed.dat   
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
[fv-az529-343:06897] *** Process received signal ***
[fv-az529-343:06897] Signal: Aborted (6)
[fv-az529-343:06897] Signal code:  (-6)
[fv-az529-343:06897] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f440e842520]
[fv-az529-343:06897] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f440e8969fc]
[fv-az529-343:06897] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f440e842476]
[fv-az529-343:06897] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f440e8287f3]
[fv-az529-343:06897] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f440eca4f26]
[fv-az529-343:06897] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f440ecb6d9c]
[fv-az529-343:06897] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f440ecb6e07]
[fv-az529-343:06897] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f440ecb70bb]
[fv-az529-343:06897] [ 8] plumed_master(+0x12ebf)[0x560a5c596ebf]
[fv-az529-343:06897] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f440e829d90]
[fv-az529-343:06897] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f440e829e40]
[fv-az529-343:06897] [11] plumed_master(+0x13155)[0x560a5c597155]
[fv-az529-343:06897] *** End of error message ***
</pre>
{% endraw %}
