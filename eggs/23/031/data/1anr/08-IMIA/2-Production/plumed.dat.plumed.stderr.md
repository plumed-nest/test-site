**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/08-IMIA/2-Production/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: SHADOW LABEL=rmsd ATOMS=rna NOPBC UPDATE=100
Maybe a missing space or a typo?
[fv-az695-456:70542] *** Process received signal ***
[fv-az695-456:70542] Signal: Aborted (6)
[fv-az695-456:70542] Signal code:  (-6)
[fv-az695-456:70542] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f86eb442520]
[fv-az695-456:70542] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f86eb4969fc]
[fv-az695-456:70542] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f86eb442476]
[fv-az695-456:70542] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f86eb4287f3]
[fv-az695-456:70542] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f86eb8a2b9e]
[fv-az695-456:70542] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f86eb8ae20c]
[fv-az695-456:70542] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f86eb8ae277]
[fv-az695-456:70542] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f86eb8ae52b]
[fv-az695-456:70542] [ 8] plumed(+0x12f48)[0x555cda0acf48]
[fv-az695-456:70542] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f86eb429d90]
[fv-az695-456:70542] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f86eb429e40]
[fv-az695-456:70542] [11] plumed(+0x131e5)[0x555cda0ad1e5]
[fv-az695-456:70542] *** End of error message ***
</pre>
{% endraw %}