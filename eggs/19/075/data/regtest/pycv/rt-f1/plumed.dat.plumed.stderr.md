**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=dAB2 ARG=dAB IMPORT=pythonfunction FUNCTION=square PERIODIC=NO
Maybe a missing space or a typo?
[fv-az979-741:06451] *** Process received signal ***
[fv-az979-741:06451] Signal: Aborted (6)
[fv-az979-741:06451] Signal code:  (-6)
[fv-az979-741:06451] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbc1fa42520]
[fv-az979-741:06451] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbc1fa969fc]
[fv-az979-741:06451] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbc1fa42476]
[fv-az979-741:06451] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbc1fa287f3]
[fv-az979-741:06451] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fbc1fea4f26]
[fv-az979-741:06451] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fbc1feb6d9c]
[fv-az979-741:06451] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fbc1feb6e07]
[fv-az979-741:06451] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbc1feb70bb]
[fv-az979-741:06451] [ 8] plumed(+0x12f48)[0x55e013de6f48]
[fv-az979-741:06451] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbc1fa29d90]
[fv-az979-741:06451] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbc1fa29e40]
[fv-az979-741:06451] [11] plumed(+0x131e5)[0x55e013de71e5]
[fv-az979-741:06451] *** End of error message ***
</pre>
{% endraw %}
