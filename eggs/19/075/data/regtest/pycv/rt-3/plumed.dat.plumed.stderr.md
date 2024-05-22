**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-3/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=distcv FUNCTION=cv
Maybe a missing space or a typo?
[fv-az1109-238:41351] *** Process received signal ***
[fv-az1109-238:41351] Signal: Aborted (6)
[fv-az1109-238:41351] Signal code:  (-6)
[fv-az1109-238:41351] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f41e9c42520]
[fv-az1109-238:41351] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f41e9c969fc]
[fv-az1109-238:41351] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f41e9c42476]
[fv-az1109-238:41351] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f41e9c287f3]
[fv-az1109-238:41351] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f41ea0a2b9e]
[fv-az1109-238:41351] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f41ea0ae20c]
[fv-az1109-238:41351] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f41ea0ae277]
[fv-az1109-238:41351] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f41ea0ae52b]
[fv-az1109-238:41351] [ 8] plumed(+0x12f48)[0x56550864af48]
[fv-az1109-238:41351] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f41e9c29d90]
[fv-az1109-238:41351] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f41e9c29e40]
[fv-az1109-238:41351] [11] plumed(+0x131e5)[0x56550864b1e5]
[fv-az1109-238:41351] *** End of error message ***
</pre>
{% endraw %}
