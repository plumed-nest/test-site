**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1anr/11-MAMY/2-Production/plumed.dat   
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
[fv-az695-456:70632] *** Process received signal ***
[fv-az695-456:70632] Signal: Aborted (6)
[fv-az695-456:70632] Signal code:  (-6)
[fv-az695-456:70632] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff882842520]
[fv-az695-456:70632] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff8828969fc]
[fv-az695-456:70632] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff882842476]
[fv-az695-456:70632] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff8828287f3]
[fv-az695-456:70632] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff882ca2b9e]
[fv-az695-456:70632] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff882cae20c]
[fv-az695-456:70632] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff882cae277]
[fv-az695-456:70632] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff882cae52b]
[fv-az695-456:70632] [ 8] plumed(+0x12f48)[0x5580be8f4f48]
[fv-az695-456:70632] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff882829d90]
[fv-az695-456:70632] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff882829e40]
[fv-az695-456:70632] [11] plumed(+0x131e5)[0x5580be8f51e5]
[fv-az695-456:70632] *** End of error message ***
</pre>
{% endraw %}
