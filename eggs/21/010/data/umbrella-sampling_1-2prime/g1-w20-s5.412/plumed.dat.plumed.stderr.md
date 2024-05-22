**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w20-s5.412/plumed.dat   
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
[fv-az1435-553:42000] *** Process received signal ***
[fv-az1435-553:42000] Signal: Aborted (6)
[fv-az1435-553:42000] Signal code:  (-6)
[fv-az1435-553:42000] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8176242520]
[fv-az1435-553:42000] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f81762969fc]
[fv-az1435-553:42000] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8176242476]
[fv-az1435-553:42000] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f81762287f3]
[fv-az1435-553:42000] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f81766a2b9e]
[fv-az1435-553:42000] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f81766ae20c]
[fv-az1435-553:42000] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f81766ae277]
[fv-az1435-553:42000] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f81766ae52b]
[fv-az1435-553:42000] [ 8] plumed(+0x12f48)[0x55e646d59f48]
[fv-az1435-553:42000] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8176229d90]
[fv-az1435-553:42000] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8176229e40]
[fv-az1435-553:42000] [11] plumed(+0x131e5)[0x55e646d5a1e5]
[fv-az1435-553:42000] *** End of error message ***
</pre>
{% endraw %}
