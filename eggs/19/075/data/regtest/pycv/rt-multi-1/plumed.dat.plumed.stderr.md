**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13
Maybe a missing space or a typo?
[fv-az979-741:06613] *** Process received signal ***
[fv-az979-741:06613] Signal: Aborted (6)
[fv-az979-741:06613] Signal code:  (-6)
[fv-az979-741:06613] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4183a42520]
[fv-az979-741:06613] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4183a969fc]
[fv-az979-741:06613] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4183a42476]
[fv-az979-741:06613] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4183a287f3]
[fv-az979-741:06613] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f4183ea4f26]
[fv-az979-741:06613] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f4183eb6d9c]
[fv-az979-741:06613] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f4183eb6e07]
[fv-az979-741:06613] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4183eb70bb]
[fv-az979-741:06613] [ 8] plumed(+0x12f48)[0x560e7e01df48]
[fv-az979-741:06613] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4183a29d90]
[fv-az979-741:06613] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4183a29e40]
[fv-az979-741:06613] [11] plumed(+0x131e5)[0x560e7e01e1e5]
[fv-az979-741:06613] *** End of error message ***
</pre>
{% endraw %}
