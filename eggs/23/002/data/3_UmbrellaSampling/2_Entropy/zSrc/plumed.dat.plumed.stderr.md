**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  3_UmbrellaSampling/2_Entropy/zSrc/plumed.dat   
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
[fv-az529-343:05369] *** Process received signal ***
[fv-az529-343:05369] Signal: Aborted (6)
[fv-az529-343:05369] Signal code:  (-6)
[fv-az529-343:05369] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe344442520]
[fv-az529-343:05369] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe3444969fc]
[fv-az529-343:05369] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe344442476]
[fv-az529-343:05369] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe3444287f3]
[fv-az529-343:05369] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe3448a4f26]
[fv-az529-343:05369] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe3448b6d9c]
[fv-az529-343:05369] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe3448b6e07]
[fv-az529-343:05369] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe3448b70bb]
[fv-az529-343:05369] [ 8] plumed(+0x12f48)[0x55a19dfeff48]
[fv-az529-343:05369] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe344429d90]
[fv-az529-343:05369] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe344429e40]
[fv-az529-343:05369] [11] plumed(+0x131e5)[0x55a19dff01e5]
[fv-az529-343:05369] *** End of error message ***
</pre>
{% endraw %}
