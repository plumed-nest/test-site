**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: HBOND_COORD SPECIES=2665-10353:4 HYDROGENS=2666-10354:4,2667-10355:4 RCUTOO=0.324 RCUTOH=0.25 ACUT=0.20pi LABEL=hb
Maybe a missing space or a typo?
[fv-az975-63:75874] *** Process received signal ***
[fv-az975-63:75874] Signal: Aborted (6)
[fv-az975-63:75874] Signal code:  (-6)
[fv-az975-63:75874] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f68acc42520]
[fv-az975-63:75874] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f68acc969fc]
[fv-az975-63:75874] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f68acc42476]
[fv-az975-63:75874] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f68acc287f3]
[fv-az975-63:75874] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f68ad0a2b9e]
[fv-az975-63:75874] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f68ad0ae20c]
[fv-az975-63:75874] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f68ad0ae277]
[fv-az975-63:75874] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f68ad0ae52b]
[fv-az975-63:75874] [ 8] plumed(+0x12f48)[0x5633eb63af48]
[fv-az975-63:75874] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f68acc29d90]
[fv-az975-63:75874] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f68acc29e40]
[fv-az975-63:75874] [11] plumed(+0x131e5)[0x5633eb63b1e5]
[fv-az975-63:75874] *** End of error message ***
</pre>
{% endraw %}
