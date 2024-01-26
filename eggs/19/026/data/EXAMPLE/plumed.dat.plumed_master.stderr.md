**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: HBOND_COORD SPECIES=2665-10353:4 HYDROGENS=2666-10354:4,2667-10355:4 RCUTOO=0.324 RCUTOH=0.25 ACUT=0.20pi LABEL=hb
Maybe a missing space or a typo?
[fv-az736-136:10651] *** Process received signal ***
[fv-az736-136:10651] Signal: Aborted (6)
[fv-az736-136:10651] Signal code:  (-6)
[fv-az736-136:10651] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5142642520]
[fv-az736-136:10651] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f51426969fc]
[fv-az736-136:10651] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5142642476]
[fv-az736-136:10651] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f51426287f3]
[fv-az736-136:10651] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f5142aa4f26]
[fv-az736-136:10651] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f5142ab6d9c]
[fv-az736-136:10651] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f5142ab6e07]
[fv-az736-136:10651] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5142ab70bb]
[fv-az736-136:10651] [ 8] plumed_master(+0x12ebf)[0x556aa2f1eebf]
[fv-az736-136:10651] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5142629d90]
[fv-az736-136:10651] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5142629e40]
[fv-az736-136:10651] [11] plumed_master(+0x13155)[0x556aa2f1f155]
[fv-az736-136:10651] *** End of error message ***
</pre>
{% endraw %}
