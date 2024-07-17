**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=cc1 ARG=t1,t2,t3 IMPORT=pythonfunction FUNCTION=cc1 PERIODIC=NO
Maybe a missing space or a typo?
[fv-az659-178:71676] *** Process received signal ***
[fv-az659-178:71676] Signal: Aborted (6)
[fv-az659-178:71676] Signal code:  (-6)
[fv-az659-178:71676] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7ac6042520]
[fv-az659-178:71676] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7ac60969fc]
[fv-az659-178:71676] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7ac6042476]
[fv-az659-178:71676] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7ac60287f3]
[fv-az659-178:71676] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7ac64a2b9e]
[fv-az659-178:71676] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7ac64ae20c]
[fv-az659-178:71676] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7ac64ae277]
[fv-az659-178:71676] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7ac64ae52b]
[fv-az659-178:71676] [ 8] plumed(+0x12f48)[0x55aefb575f48]
[fv-az659-178:71676] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7ac6029d90]
[fv-az659-178:71676] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7ac6029e40]
[fv-az659-178:71676] [11] plumed(+0x131e5)[0x55aefb5761e5]
[fv-az659-178:71676] *** End of error message ***
</pre>
{% endraw %}
