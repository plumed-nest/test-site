**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w27-s6.924/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az774-16:72604] *** Process received signal ***
[fv-az774-16:72604] Signal: Aborted (6)
[fv-az774-16:72604] Signal code:  (-6)
[fv-az774-16:72604] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f629ba42520]
[fv-az774-16:72604] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f629ba969fc]
[fv-az774-16:72604] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f629ba42476]
[fv-az774-16:72604] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f629ba287f3]
[fv-az774-16:72604] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f629bea2b9e]
[fv-az774-16:72604] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f629beae20c]
[fv-az774-16:72604] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f629beae277]
[fv-az774-16:72604] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f629beae52b]
[fv-az774-16:72604] [ 8] plumed(+0x12f48)[0x55d450d70f48]
[fv-az774-16:72604] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f629ba29d90]
[fv-az774-16:72604] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f629ba29e40]
[fv-az774-16:72604] [11] plumed(+0x131e5)[0x55d450d711e5]
[fv-az774-16:72604] *** End of error message ***
</pre>
{% endraw %}
