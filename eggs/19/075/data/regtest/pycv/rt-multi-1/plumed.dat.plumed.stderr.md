**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13
Maybe a missing space or a typo?
[fv-az659-178:71801] *** Process received signal ***
[fv-az659-178:71801] Signal: Aborted (6)
[fv-az659-178:71801] Signal code:  (-6)
[fv-az659-178:71801] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f02f6642520]
[fv-az659-178:71801] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f02f66969fc]
[fv-az659-178:71801] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f02f6642476]
[fv-az659-178:71801] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f02f66287f3]
[fv-az659-178:71801] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f02f6aa2b9e]
[fv-az659-178:71801] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f02f6aae20c]
[fv-az659-178:71801] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f02f6aae277]
[fv-az659-178:71801] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f02f6aae52b]
[fv-az659-178:71801] [ 8] plumed(+0x12f48)[0x5593594a0f48]
[fv-az659-178:71801] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f02f6629d90]
[fv-az659-178:71801] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f02f6629e40]
[fv-az659-178:71801] [11] plumed(+0x131e5)[0x5593594a11e5]
[fv-az659-178:71801] *** End of error message ***
</pre>
{% endraw %}
