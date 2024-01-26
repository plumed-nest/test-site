**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=pycv FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az979-741:06363] *** Process received signal ***
[fv-az979-741:06363] Signal: Aborted (6)
[fv-az979-741:06363] Signal code:  (-6)
[fv-az979-741:06363] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fcd8f042520]
[fv-az979-741:06363] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fcd8f0969fc]
[fv-az979-741:06363] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fcd8f042476]
[fv-az979-741:06363] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fcd8f0287f3]
[fv-az979-741:06363] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fcd8f4a4f26]
[fv-az979-741:06363] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fcd8f4b6d9c]
[fv-az979-741:06363] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fcd8f4b6e07]
[fv-az979-741:06363] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fcd8f4b70bb]
[fv-az979-741:06363] [ 8] plumed_master(+0x12ebf)[0x561c89bc2ebf]
[fv-az979-741:06363] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fcd8f029d90]
[fv-az979-741:06363] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fcd8f029e40]
[fv-az979-741:06363] [11] plumed_master(+0x13155)[0x561c89bc3155]
[fv-az979-741:06363] *** End of error message ***
</pre>
{% endraw %}
