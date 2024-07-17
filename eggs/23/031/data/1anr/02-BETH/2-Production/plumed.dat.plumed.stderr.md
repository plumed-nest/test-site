**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/02-BETH/2-Production/plumed.dat   
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
[fv-az695-456:70359] *** Process received signal ***
[fv-az695-456:70359] Signal: Aborted (6)
[fv-az695-456:70359] Signal code:  (-6)
[fv-az695-456:70359] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f380c642520]
[fv-az695-456:70359] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f380c6969fc]
[fv-az695-456:70359] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f380c642476]
[fv-az695-456:70359] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f380c6287f3]
[fv-az695-456:70359] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f380caa2b9e]
[fv-az695-456:70359] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f380caae20c]
[fv-az695-456:70359] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f380caae277]
[fv-az695-456:70359] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f380caae52b]
[fv-az695-456:70359] [ 8] plumed(+0x12f48)[0x558138da9f48]
[fv-az695-456:70359] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f380c629d90]
[fv-az695-456:70359] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f380c629e40]
[fv-az695-456:70359] [11] plumed(+0x131e5)[0x558138daa1e5]
[fv-az695-456:70359] *** End of error message ***
</pre>
{% endraw %}
