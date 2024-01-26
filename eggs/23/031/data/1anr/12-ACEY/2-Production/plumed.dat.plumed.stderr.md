**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/12-ACEY/2-Production/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: SHADOW LABEL=rmsd ATOMS=rna NOPBC UPDATE=100
Maybe a missing space or a typo?
[fv-az532-512:05331] *** Process received signal ***
[fv-az532-512:05331] Signal: Aborted (6)
[fv-az532-512:05331] Signal code:  (-6)
[fv-az532-512:05331] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f62a2442520]
[fv-az532-512:05331] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f62a24969fc]
[fv-az532-512:05331] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f62a2442476]
[fv-az532-512:05331] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f62a24287f3]
[fv-az532-512:05331] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f62a28a4f26]
[fv-az532-512:05331] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f62a28b6d9c]
[fv-az532-512:05331] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f62a28b6e07]
[fv-az532-512:05331] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f62a28b70bb]
[fv-az532-512:05331] [ 8] plumed(+0x12f48)[0x558f743d1f48]
[fv-az532-512:05331] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f62a2429d90]
[fv-az532-512:05331] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f62a2429e40]
[fv-az532-512:05331] [11] plumed(+0x131e5)[0x558f743d21e5]
[fv-az532-512:05331] *** End of error message ***
</pre>
{% endraw %}
