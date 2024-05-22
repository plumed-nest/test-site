**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  2_Commitor/plumed.dat   
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
[fv-az1435-553:40089] *** Process received signal ***
[fv-az1435-553:40089] Signal: Aborted (6)
[fv-az1435-553:40089] Signal code:  (-6)
[fv-az1435-553:40089] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8b76442520]
[fv-az1435-553:40089] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8b764969fc]
[fv-az1435-553:40089] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8b76442476]
[fv-az1435-553:40089] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8b764287f3]
[fv-az1435-553:40089] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8b768a2b9e]
[fv-az1435-553:40089] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8b768ae20c]
[fv-az1435-553:40089] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8b768ae277]
[fv-az1435-553:40089] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8b768ae52b]
[fv-az1435-553:40089] [ 8] plumed(+0x12f48)[0x55eb96ff3f48]
[fv-az1435-553:40089] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8b76429d90]
[fv-az1435-553:40089] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8b76429e40]
[fv-az1435-553:40089] [11] plumed(+0x131e5)[0x55eb96ff41e5]
[fv-az1435-553:40089] *** End of error message ***
</pre>
{% endraw %}
