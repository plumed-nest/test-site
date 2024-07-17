**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/12-ACEY/2-Production/plumed.dat   
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
[fv-az695-456:70662] *** Process received signal ***
[fv-az695-456:70662] Signal: Aborted (6)
[fv-az695-456:70662] Signal code:  (-6)
[fv-az695-456:70662] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f23e4a42520]
[fv-az695-456:70662] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f23e4a969fc]
[fv-az695-456:70662] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f23e4a42476]
[fv-az695-456:70662] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f23e4a287f3]
[fv-az695-456:70662] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f23e4ea2b9e]
[fv-az695-456:70662] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f23e4eae20c]
[fv-az695-456:70662] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f23e4eae277]
[fv-az695-456:70662] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f23e4eae52b]
[fv-az695-456:70662] [ 8] plumed(+0x12f48)[0x55d9541cef48]
[fv-az695-456:70662] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f23e4a29d90]
[fv-az695-456:70662] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f23e4a29e40]
[fv-az695-456:70662] [11] plumed(+0x131e5)[0x55d9541cf1e5]
[fv-az695-456:70662] *** End of error message ***
</pre>
{% endraw %}
