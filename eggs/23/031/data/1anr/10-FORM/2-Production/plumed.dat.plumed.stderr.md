**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/10-FORM/2-Production/plumed.dat   
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
[fv-az532-512:05270] *** Process received signal ***
[fv-az532-512:05270] Signal: Aborted (6)
[fv-az532-512:05270] Signal code:  (-6)
[fv-az532-512:05270] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd55ee42520]
[fv-az532-512:05270] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd55ee969fc]
[fv-az532-512:05270] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd55ee42476]
[fv-az532-512:05270] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd55ee287f3]
[fv-az532-512:05270] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fd55f2a4f26]
[fv-az532-512:05270] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fd55f2b6d9c]
[fv-az532-512:05270] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fd55f2b6e07]
[fv-az532-512:05270] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd55f2b70bb]
[fv-az532-512:05270] [ 8] plumed(+0x12f48)[0x55fe734c9f48]
[fv-az532-512:05270] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd55ee29d90]
[fv-az532-512:05270] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd55ee29e40]
[fv-az532-512:05270] [11] plumed(+0x131e5)[0x55fe734ca1e5]
[fv-az532-512:05270] *** End of error message ***
</pre>
{% endraw %}
