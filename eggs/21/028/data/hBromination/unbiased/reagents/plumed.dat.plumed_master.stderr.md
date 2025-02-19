**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/reagents/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:476) void PLMD::Keywords::addFlag(std::string_view, bool, std::string_view)
+++ assertion failed: !defaultValue
the second argument to addFlag must be false COMPONENTS
[fv-az1326-415:11952] *** Process received signal ***
[fv-az1326-415:11952] Signal: Aborted (6)
[fv-az1326-415:11952] Signal code:  (-6)
[fv-az1326-415:11952] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd00a645330]
[fv-az1326-415:11952] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd00a69eb2c]
[fv-az1326-415:11952] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd00a64527e]
[fv-az1326-415:11952] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd00a6288ff]
[fv-az1326-415:11952] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd00aaa5ff5]
[fv-az1326-415:11952] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd00aabb0da]
[fv-az1326-415:11952] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd00aaa5a55]
[fv-az1326-415:11952] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd00aaa5a6f]
[fv-az1326-415:11952] [ 8] plumed_master(+0x146dd)[0x5650e49996dd]
[fv-az1326-415:11952] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd00a62a1ca]
[fv-az1326-415:11952] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd00a62a28b]
[fv-az1326-415:11952] [11] plumed_master(+0x15365)[0x5650e499a365]
[fv-az1326-415:11952] *** End of error message ***
</pre>
{% endraw %}
