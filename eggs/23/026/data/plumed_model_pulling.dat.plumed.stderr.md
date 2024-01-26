**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_pulling.dat   
Download: [zipped raw stdout](plumed_model_pulling.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_model_pulling.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1-421 IMPORT=model FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az1542-52:04442] *** Process received signal ***
[fv-az1542-52:04442] Signal: Aborted (6)
[fv-az1542-52:04442] Signal code:  (-6)
[fv-az1542-52:04442] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7feebf442520]
[fv-az1542-52:04442] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7feebf4969fc]
[fv-az1542-52:04442] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7feebf442476]
[fv-az1542-52:04442] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7feebf4287f3]
[fv-az1542-52:04442] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7feebf8a4f26]
[fv-az1542-52:04442] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7feebf8b6d9c]
[fv-az1542-52:04442] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7feebf8b6e07]
[fv-az1542-52:04442] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7feebf8b70bb]
[fv-az1542-52:04442] [ 8] plumed(+0x12f48)[0x5622c687af48]
[fv-az1542-52:04442] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7feebf429d90]
[fv-az1542-52:04442] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7feebf429e40]
[fv-az1542-52:04442] [11] plumed(+0x131e5)[0x5622c687b1e5]
[fv-az1542-52:04442] *** End of error message ***
</pre>
{% endraw %}
