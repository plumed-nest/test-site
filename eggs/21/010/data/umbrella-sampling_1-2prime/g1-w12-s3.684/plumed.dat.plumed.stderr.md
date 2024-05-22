**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w12-s3.684/plumed.dat   
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
[fv-az1435-553:41720] *** Process received signal ***
[fv-az1435-553:41720] Signal: Aborted (6)
[fv-az1435-553:41720] Signal code:  (-6)
[fv-az1435-553:41720] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa9d9e42520]
[fv-az1435-553:41720] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa9d9e969fc]
[fv-az1435-553:41720] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa9d9e42476]
[fv-az1435-553:41720] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa9d9e287f3]
[fv-az1435-553:41720] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa9da2a2b9e]
[fv-az1435-553:41720] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa9da2ae20c]
[fv-az1435-553:41720] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa9da2ae277]
[fv-az1435-553:41720] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa9da2ae52b]
[fv-az1435-553:41720] [ 8] plumed(+0x12f48)[0x5576a6115f48]
[fv-az1435-553:41720] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa9d9e29d90]
[fv-az1435-553:41720] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa9d9e29e40]
[fv-az1435-553:41720] [11] plumed(+0x131e5)[0x5576a61161e5]
[fv-az1435-553:41720] *** End of error message ***
</pre>
{% endraw %}
