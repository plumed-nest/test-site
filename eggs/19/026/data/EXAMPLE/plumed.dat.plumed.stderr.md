**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: HBOND_COORD SPECIES=2665-10353:4 HYDROGENS=2666-10354:4,2667-10355:4 RCUTOO=0.324 RCUTOH=0.25 ACUT=0.20pi LABEL=hb
Maybe a missing space or a typo?
[fv-az736-136:10643] *** Process received signal ***
[fv-az736-136:10643] Signal: Aborted (6)
[fv-az736-136:10643] Signal code:  (-6)
[fv-az736-136:10643] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f98f0642520]
[fv-az736-136:10643] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f98f06969fc]
[fv-az736-136:10643] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f98f0642476]
[fv-az736-136:10643] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f98f06287f3]
[fv-az736-136:10643] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f98f0aa4f26]
[fv-az736-136:10643] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f98f0ab6d9c]
[fv-az736-136:10643] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f98f0ab6e07]
[fv-az736-136:10643] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f98f0ab70bb]
[fv-az736-136:10643] [ 8] plumed(+0x12f48)[0x558efc4abf48]
[fv-az736-136:10643] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f98f0629d90]
[fv-az736-136:10643] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f98f0629e40]
[fv-az736-136:10643] [11] plumed(+0x131e5)[0x558efc4ac1e5]
[fv-az736-136:10643] *** End of error message ***
</pre>
{% endraw %}
