**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w2-s1.524/plumed.dat   
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
[fv-az1435-553:41968] *** Process received signal ***
[fv-az1435-553:41968] Signal: Aborted (6)
[fv-az1435-553:41968] Signal code:  (-6)
[fv-az1435-553:41968] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4502642520]
[fv-az1435-553:41968] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f45026969fc]
[fv-az1435-553:41968] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4502642476]
[fv-az1435-553:41968] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f45026287f3]
[fv-az1435-553:41968] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4502aa2b9e]
[fv-az1435-553:41968] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4502aae20c]
[fv-az1435-553:41968] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4502aae277]
[fv-az1435-553:41968] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4502aae52b]
[fv-az1435-553:41968] [ 8] plumed(+0x12f48)[0x560a49f37f48]
[fv-az1435-553:41968] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4502629d90]
[fv-az1435-553:41968] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4502629e40]
[fv-az1435-553:41968] [11] plumed(+0x131e5)[0x560a49f381e5]
[fv-az1435-553:41968] *** End of error message ***
</pre>
{% endraw %}
