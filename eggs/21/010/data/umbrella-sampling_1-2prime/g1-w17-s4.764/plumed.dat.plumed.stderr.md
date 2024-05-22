**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w17-s4.764/plumed.dat   
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
[fv-az1435-553:41875] *** Process received signal ***
[fv-az1435-553:41875] Signal: Aborted (6)
[fv-az1435-553:41875] Signal code:  (-6)
[fv-az1435-553:41875] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f03cce42520]
[fv-az1435-553:41875] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f03cce969fc]
[fv-az1435-553:41875] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f03cce42476]
[fv-az1435-553:41875] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f03cce287f3]
[fv-az1435-553:41875] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f03cd2a2b9e]
[fv-az1435-553:41875] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f03cd2ae20c]
[fv-az1435-553:41875] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f03cd2ae277]
[fv-az1435-553:41875] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f03cd2ae52b]
[fv-az1435-553:41875] [ 8] plumed(+0x12f48)[0x5618723f7f48]
[fv-az1435-553:41875] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f03cce29d90]
[fv-az1435-553:41875] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f03cce29e40]
[fv-az1435-553:41875] [11] plumed(+0x131e5)[0x5618723f81e5]
[fv-az1435-553:41875] *** End of error message ***
</pre>
{% endraw %}
