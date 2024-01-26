**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-2-jax/plumed.dat   
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
[fv-az979-741:06645] *** Process received signal ***
[fv-az979-741:06645] Signal: Aborted (6)
[fv-az979-741:06645] Signal code:  (-6)
[fv-az979-741:06645] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7747842520]
[fv-az979-741:06645] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f77478969fc]
[fv-az979-741:06645] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7747842476]
[fv-az979-741:06645] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f77478287f3]
[fv-az979-741:06645] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7747ca4f26]
[fv-az979-741:06645] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7747cb6d9c]
[fv-az979-741:06645] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7747cb6e07]
[fv-az979-741:06645] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7747cb70bb]
[fv-az979-741:06645] [ 8] plumed(+0x12f48)[0x563901de4f48]
[fv-az979-741:06645] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7747829d90]
[fv-az979-741:06645] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7747829e40]
[fv-az979-741:06645] [11] plumed(+0x131e5)[0x563901de51e5]
[fv-az979-741:06645] *** End of error message ***
</pre>
{% endraw %}
