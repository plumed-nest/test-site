**Project ID:** [plumID:19.053]({{ '/' | absolute_url }}eggs/19/053/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: MORE_THAN LABEL=smapfcc ARG=fcc SWITCH=SMAP R_0=0.5 A=8 B=8
Maybe a missing space or a typo?
[fv-az841-65:73580] *** Process received signal ***
[fv-az841-65:73580] Signal: Aborted (6)
[fv-az841-65:73580] Signal code:  (-6)
[fv-az841-65:73580] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3221242520]
[fv-az841-65:73580] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f32212969fc]
[fv-az841-65:73580] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3221242476]
[fv-az841-65:73580] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f32212287f3]
[fv-az841-65:73580] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f32216a2b9e]
[fv-az841-65:73580] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f32216ae20c]
[fv-az841-65:73580] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f32216ae277]
[fv-az841-65:73580] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f32216ae52b]
[fv-az841-65:73580] [ 8] plumed(+0x12f48)[0x564de9769f48]
[fv-az841-65:73580] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3221229d90]
[fv-az841-65:73580] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3221229e40]
[fv-az841-65:73580] [11] plumed(+0x131e5)[0x564de976a1e5]
[fv-az841-65:73580] *** End of error message ***
</pre>
{% endraw %}
