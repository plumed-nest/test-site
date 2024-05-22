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
[fv-az1109-238:41413] *** Process received signal ***
[fv-az1109-238:41413] Signal: Aborted (6)
[fv-az1109-238:41413] Signal code:  (-6)
[fv-az1109-238:41413] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5daa642520]
[fv-az1109-238:41413] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5daa6969fc]
[fv-az1109-238:41413] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5daa642476]
[fv-az1109-238:41413] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5daa6287f3]
[fv-az1109-238:41413] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5daaaa2b9e]
[fv-az1109-238:41413] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5daaaae20c]
[fv-az1109-238:41413] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5daaaae277]
[fv-az1109-238:41413] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5daaaae52b]
[fv-az1109-238:41413] [ 8] plumed(+0x12f48)[0x564810442f48]
[fv-az1109-238:41413] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5daa629d90]
[fv-az1109-238:41413] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5daa629e40]
[fv-az1109-238:41413] [11] plumed(+0x131e5)[0x5648104431e5]
[fv-az1109-238:41413] *** End of error message ***
</pre>
{% endraw %}
