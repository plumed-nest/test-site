**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  3_UmbrellaSampling/1_PIV/zSrc/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PAIRENTROPY LABEL=s ATOMS=1-4394 MAXR=2.5 SIGMA=0.05 NLIST NL_CUTOFF=2.8 NL_STRIDE=10
Maybe a missing space or a typo?
[fv-az529-343:05337] *** Process received signal ***
[fv-az529-343:05337] Signal: Aborted (6)
[fv-az529-343:05337] Signal code:  (-6)
[fv-az529-343:05337] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc5acc42520]
[fv-az529-343:05337] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc5acc969fc]
[fv-az529-343:05337] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc5acc42476]
[fv-az529-343:05337] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc5acc287f3]
[fv-az529-343:05337] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fc5ad0a4f26]
[fv-az529-343:05337] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fc5ad0b6d9c]
[fv-az529-343:05337] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fc5ad0b6e07]
[fv-az529-343:05337] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc5ad0b70bb]
[fv-az529-343:05337] [ 8] plumed(+0x12f48)[0x55655436ff48]
[fv-az529-343:05337] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc5acc29d90]
[fv-az529-343:05337] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc5acc29e40]
[fv-az529-343:05337] [11] plumed(+0x131e5)[0x5565543701e5]
[fv-az529-343:05337] *** End of error message ***
</pre>
{% endraw %}
