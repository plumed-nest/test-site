**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w10-s3.252/plumed.dat   
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
[fv-az774-16:72041] *** Process received signal ***
[fv-az774-16:72041] Signal: Aborted (6)
[fv-az774-16:72041] Signal code:  (-6)
[fv-az774-16:72041] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4a4e842520]
[fv-az774-16:72041] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4a4e8969fc]
[fv-az774-16:72041] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4a4e842476]
[fv-az774-16:72041] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4a4e8287f3]
[fv-az774-16:72041] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4a4eca2b9e]
[fv-az774-16:72041] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4a4ecae20c]
[fv-az774-16:72041] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4a4ecae277]
[fv-az774-16:72041] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4a4ecae52b]
[fv-az774-16:72041] [ 8] plumed(+0x12f48)[0x55b25381ff48]
[fv-az774-16:72041] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4a4e829d90]
[fv-az774-16:72041] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4a4e829e40]
[fv-az774-16:72041] [11] plumed(+0x131e5)[0x55b2538201e5]
[fv-az774-16:72041] *** End of error message ***
</pre>
{% endraw %}
