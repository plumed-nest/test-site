**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-2/plumed.dat   
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
[fv-az1109-238:41318] *** Process received signal ***
[fv-az1109-238:41318] Signal: Aborted (6)
[fv-az1109-238:41318] Signal code:  (-6)
[fv-az1109-238:41318] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f14a0442520]
[fv-az1109-238:41318] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f14a04969fc]
[fv-az1109-238:41318] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f14a0442476]
[fv-az1109-238:41318] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f14a04287f3]
[fv-az1109-238:41318] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f14a08a2b9e]
[fv-az1109-238:41318] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f14a08ae20c]
[fv-az1109-238:41318] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f14a08ae277]
[fv-az1109-238:41318] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f14a08ae52b]
[fv-az1109-238:41318] [ 8] plumed(+0x12f48)[0x56194b727f48]
[fv-az1109-238:41318] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f14a0429d90]
[fv-az1109-238:41318] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f14a0429e40]
[fv-az1109-238:41318] [11] plumed(+0x131e5)[0x56194b7281e5]
[fv-az1109-238:41318] *** End of error message ***
</pre>
{% endraw %}
