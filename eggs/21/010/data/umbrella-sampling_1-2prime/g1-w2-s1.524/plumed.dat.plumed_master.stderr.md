**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w2-s1.524/plumed.dat   
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
[fv-az529-343:07210] *** Process received signal ***
[fv-az529-343:07210] Signal: Aborted (6)
[fv-az529-343:07210] Signal code:  (-6)
[fv-az529-343:07210] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa8bc842520]
[fv-az529-343:07210] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa8bc8969fc]
[fv-az529-343:07210] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa8bc842476]
[fv-az529-343:07210] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa8bc8287f3]
[fv-az529-343:07210] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa8bcca4f26]
[fv-az529-343:07210] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa8bccb6d9c]
[fv-az529-343:07210] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa8bccb6e07]
[fv-az529-343:07210] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa8bccb70bb]
[fv-az529-343:07210] [ 8] plumed_master(+0x12ebf)[0x55aa96896ebf]
[fv-az529-343:07210] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa8bc829d90]
[fv-az529-343:07210] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa8bc829e40]
[fv-az529-343:07210] [11] plumed_master(+0x13155)[0x55aa96897155]
[fv-az529-343:07210] *** End of error message ***
</pre>
{% endraw %}
