**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w21-s5.628/plumed.dat   
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
[fv-az774-16:72415] *** Process received signal ***
[fv-az774-16:72415] Signal: Aborted (6)
[fv-az774-16:72415] Signal code:  (-6)
[fv-az774-16:72415] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f339ec42520]
[fv-az774-16:72415] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f339ec969fc]
[fv-az774-16:72415] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f339ec42476]
[fv-az774-16:72415] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f339ec287f3]
[fv-az774-16:72415] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f339f0a2b9e]
[fv-az774-16:72415] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f339f0ae20c]
[fv-az774-16:72415] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f339f0ae277]
[fv-az774-16:72415] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f339f0ae52b]
[fv-az774-16:72415] [ 8] plumed(+0x12f48)[0x55f7330e6f48]
[fv-az774-16:72415] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f339ec29d90]
[fv-az774-16:72415] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f339ec29e40]
[fv-az774-16:72415] [11] plumed(+0x131e5)[0x55f7330e71e5]
[fv-az774-16:72415] *** End of error message ***
</pre>
{% endraw %}
