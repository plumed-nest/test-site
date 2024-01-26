**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=distcv FUNCTION=cv
Maybe a missing space or a typo?
[fv-az979-741:06395] *** Process received signal ***
[fv-az979-741:06395] Signal: Aborted (6)
[fv-az979-741:06395] Signal code:  (-6)
[fv-az979-741:06395] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7f7ec42520]
[fv-az979-741:06395] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7f7ec969fc]
[fv-az979-741:06395] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7f7ec42476]
[fv-az979-741:06395] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7f7ec287f3]
[fv-az979-741:06395] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7f7f0a4f26]
[fv-az979-741:06395] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7f7f0b6d9c]
[fv-az979-741:06395] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7f7f0b6e07]
[fv-az979-741:06395] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7f7f0b70bb]
[fv-az979-741:06395] [ 8] plumed_master(+0x12ebf)[0x55ecef63eebf]
[fv-az979-741:06395] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7f7ec29d90]
[fv-az979-741:06395] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7f7ec29e40]
[fv-az979-741:06395] [11] plumed_master(+0x13155)[0x55ecef63f155]
[fv-az979-741:06395] *** End of error message ***
</pre>
{% endraw %}
