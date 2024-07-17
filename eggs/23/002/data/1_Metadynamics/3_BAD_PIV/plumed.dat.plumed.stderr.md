**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/3_BAD_PIV/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PAIRENTROPY LABEL=s ATOMS=1-4394 MAXR=2.5 SIGMA=0.05 NLIST NL_CUTOFF=2.8 NL_STRIDE=10
Maybe a missing space or a typo?
[fv-az774-16:70421] *** Process received signal ***
[fv-az774-16:70421] Signal: Aborted (6)
[fv-az774-16:70421] Signal code:  (-6)
[fv-az774-16:70421] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8992242520]
[fv-az774-16:70421] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f89922969fc]
[fv-az774-16:70421] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8992242476]
[fv-az774-16:70421] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f89922287f3]
[fv-az774-16:70421] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f89926a2b9e]
[fv-az774-16:70421] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f89926ae20c]
[fv-az774-16:70421] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f89926ae277]
[fv-az774-16:70421] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f89926ae52b]
[fv-az774-16:70421] [ 8] plumed(+0x12f48)[0x55e7a0bf4f48]
[fv-az774-16:70421] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8992229d90]
[fv-az774-16:70421] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8992229e40]
[fv-az774-16:70421] [11] plumed(+0x131e5)[0x55e7a0bf51e5]
[fv-az774-16:70421] *** End of error message ***
</pre>
{% endraw %}
