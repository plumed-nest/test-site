**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w18-s4.980/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az529-343:07140] *** Process received signal ***
[fv-az529-343:07140] Signal: Aborted (6)
[fv-az529-343:07140] Signal code:  (-6)
[fv-az529-343:07140] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f10cac42520]
[fv-az529-343:07140] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f10cac969fc]
[fv-az529-343:07140] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f10cac42476]
[fv-az529-343:07140] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f10cac287f3]
[fv-az529-343:07140] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f10cb0a4f26]
[fv-az529-343:07140] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f10cb0b6d9c]
[fv-az529-343:07140] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f10cb0b6e07]
[fv-az529-343:07140] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f10cb0b70bb]
[fv-az529-343:07140] [ 8] plumed(+0x12f48)[0x563a2cbf8f48]
[fv-az529-343:07140] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f10cac29d90]
[fv-az529-343:07140] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f10cac29e40]
[fv-az529-343:07140] [11] plumed(+0x131e5)[0x563a2cbf91e5]
[fv-az529-343:07140] *** End of error message ***
</pre>
{% endraw %}
