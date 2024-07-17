**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/05-MEPY/2-Production/plumed.dat   
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
[fv-az695-456:70450] *** Process received signal ***
[fv-az695-456:70450] Signal: Aborted (6)
[fv-az695-456:70450] Signal code:  (-6)
[fv-az695-456:70450] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f79b4242520]
[fv-az695-456:70450] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f79b42969fc]
[fv-az695-456:70450] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f79b4242476]
[fv-az695-456:70450] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f79b42287f3]
[fv-az695-456:70450] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f79b46a2b9e]
[fv-az695-456:70450] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f79b46ae20c]
[fv-az695-456:70450] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f79b46ae277]
[fv-az695-456:70450] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f79b46ae52b]
[fv-az695-456:70450] [ 8] plumed(+0x12f48)[0x55858c132f48]
[fv-az695-456:70450] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f79b4229d90]
[fv-az695-456:70450] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f79b4229e40]
[fv-az695-456:70450] [11] plumed(+0x131e5)[0x55858c1331e5]
[fv-az695-456:70450] *** End of error message ***
</pre>
{% endraw %}
