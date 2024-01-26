**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=jaxcv FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az979-741:06523] *** Process received signal ***
[fv-az979-741:06523] Signal: Aborted (6)
[fv-az979-741:06523] Signal code:  (-6)
[fv-az979-741:06523] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3fa3042520]
[fv-az979-741:06523] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3fa30969fc]
[fv-az979-741:06523] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3fa3042476]
[fv-az979-741:06523] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3fa30287f3]
[fv-az979-741:06523] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f3fa34a4f26]
[fv-az979-741:06523] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f3fa34b6d9c]
[fv-az979-741:06523] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f3fa34b6e07]
[fv-az979-741:06523] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3fa34b70bb]
[fv-az979-741:06523] [ 8] plumed_master(+0x12ebf)[0x555728c28ebf]
[fv-az979-741:06523] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3fa3029d90]
[fv-az979-741:06523] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3fa3029e40]
[fv-az979-741:06523] [11] plumed_master(+0x13155)[0x555728c29155]
[fv-az979-741:06523] *** End of error message ***
</pre>
{% endraw %}
