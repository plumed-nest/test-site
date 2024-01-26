**Project ID:** [plumID:23.026]({{ '/' | absolute_url }}eggs/23/026/)  
Stderr for source:  plumed_model_2D_WTD.dat   
Download: [zipped raw stdout](plumed_model_2D_WTD.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_model_2D_WTD.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1-421 IMPORT=model_2D FUNCTION=cv1 COMPONENTS=ncl,nq6
Maybe a missing space or a typo?
[fv-az1542-52:04410] *** Process received signal ***
[fv-az1542-52:04410] Signal: Aborted (6)
[fv-az1542-52:04410] Signal code:  (-6)
[fv-az1542-52:04410] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3dafc42520]
[fv-az1542-52:04410] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3dafc969fc]
[fv-az1542-52:04410] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3dafc42476]
[fv-az1542-52:04410] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3dafc287f3]
[fv-az1542-52:04410] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f3db00a4f26]
[fv-az1542-52:04410] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f3db00b6d9c]
[fv-az1542-52:04410] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f3db00b6e07]
[fv-az1542-52:04410] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3db00b70bb]
[fv-az1542-52:04410] [ 8] plumed(+0x12f48)[0x55ed7f90af48]
[fv-az1542-52:04410] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3dafc29d90]
[fv-az1542-52:04410] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3dafc29e40]
[fv-az1542-52:04410] [11] plumed(+0x131e5)[0x55ed7f90b1e5]
[fv-az1542-52:04410] *** End of error message ***
</pre>
{% endraw %}
