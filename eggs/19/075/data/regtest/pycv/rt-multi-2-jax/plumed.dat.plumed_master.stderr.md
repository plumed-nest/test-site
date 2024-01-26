**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-2-jax/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13
Maybe a missing space or a typo?
[fv-az979-741:06653] *** Process received signal ***
[fv-az979-741:06653] Signal: Aborted (6)
[fv-az979-741:06653] Signal code:  (-6)
[fv-az979-741:06653] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f80c2842520]
[fv-az979-741:06653] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f80c28969fc]
[fv-az979-741:06653] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f80c2842476]
[fv-az979-741:06653] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f80c28287f3]
[fv-az979-741:06653] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f80c2ca4f26]
[fv-az979-741:06653] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f80c2cb6d9c]
[fv-az979-741:06653] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f80c2cb6e07]
[fv-az979-741:06653] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f80c2cb70bb]
[fv-az979-741:06653] [ 8] plumed_master(+0x12ebf)[0x559a28ff8ebf]
[fv-az979-741:06653] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f80c2829d90]
[fv-az979-741:06653] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f80c2829e40]
[fv-az979-741:06653] [11] plumed_master(+0x13155)[0x559a28ff9155]
[fv-az979-741:06653] *** End of error message ***
</pre>
{% endraw %}
