**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  2_Commitor/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: PAIRENTROPY LABEL=s ATOMS=1-4394 MAXR=2.5 SIGMA=0.05 NLIST NL_CUTOFF=2.8 NL_STRIDE=10
Maybe a missing space or a typo?
[fv-az529-343:05313] *** Process received signal ***
[fv-az529-343:05313] Signal: Aborted (6)
[fv-az529-343:05313] Signal code:  (-6)
[fv-az529-343:05313] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9cbfe42520]
[fv-az529-343:05313] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9cbfe969fc]
[fv-az529-343:05313] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9cbfe42476]
[fv-az529-343:05313] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9cbfe287f3]
[fv-az529-343:05313] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f9cc02a4f26]
[fv-az529-343:05313] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f9cc02b6d9c]
[fv-az529-343:05313] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f9cc02b6e07]
[fv-az529-343:05313] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9cc02b70bb]
[fv-az529-343:05313] [ 8] plumed_master(+0x12ebf)[0x55d2dce1debf]
[fv-az529-343:05313] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9cbfe29d90]
[fv-az529-343:05313] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9cbfe29e40]
[fv-az529-343:05313] [11] plumed_master(+0x13155)[0x55d2dce1e155]
[fv-az529-343:05313] *** End of error message ***
</pre>
{% endraw %}
