**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w13-s3.900/plumed.dat   
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
[fv-az1435-553:41751] *** Process received signal ***
[fv-az1435-553:41751] Signal: Aborted (6)
[fv-az1435-553:41751] Signal code:  (-6)
[fv-az1435-553:41751] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3dc7242520]
[fv-az1435-553:41751] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3dc72969fc]
[fv-az1435-553:41751] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3dc7242476]
[fv-az1435-553:41751] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3dc72287f3]
[fv-az1435-553:41751] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3dc76a2b9e]
[fv-az1435-553:41751] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3dc76ae20c]
[fv-az1435-553:41751] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3dc76ae277]
[fv-az1435-553:41751] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3dc76ae52b]
[fv-az1435-553:41751] [ 8] plumed(+0x12f48)[0x562e86372f48]
[fv-az1435-553:41751] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3dc7229d90]
[fv-az1435-553:41751] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3dc7229e40]
[fv-az1435-553:41751] [11] plumed(+0x131e5)[0x562e863731e5]
[fv-az1435-553:41751] *** End of error message ***
</pre>
{% endraw %}
