**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/1_PIV/plumed.dat   
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
[fv-az774-16:70357] *** Process received signal ***
[fv-az774-16:70357] Signal: Aborted (6)
[fv-az774-16:70357] Signal code:  (-6)
[fv-az774-16:70357] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f71b9642520]
[fv-az774-16:70357] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f71b96969fc]
[fv-az774-16:70357] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f71b9642476]
[fv-az774-16:70357] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f71b96287f3]
[fv-az774-16:70357] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f71b9aa2b9e]
[fv-az774-16:70357] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f71b9aae20c]
[fv-az774-16:70357] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f71b9aae277]
[fv-az774-16:70357] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f71b9aae52b]
[fv-az774-16:70357] [ 8] plumed(+0x12f48)[0x56049dc0cf48]
[fv-az774-16:70357] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f71b9629d90]
[fv-az774-16:70357] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f71b9629e40]
[fv-az774-16:70357] [11] plumed(+0x131e5)[0x56049dc0d1e5]
[fv-az774-16:70357] *** End of error message ***
</pre>
{% endraw %}
