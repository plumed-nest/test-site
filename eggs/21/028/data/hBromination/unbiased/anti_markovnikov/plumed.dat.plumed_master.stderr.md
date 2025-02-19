**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/anti_markovnikov/plumed.dat   
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
[fv-az1326-415:11840] *** Process received signal ***
[fv-az1326-415:11840] Signal: Aborted (6)
[fv-az1326-415:11840] Signal code:  (-6)
[fv-az1326-415:11840] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbbe5045330]
[fv-az1326-415:11840] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbbe509eb2c]
[fv-az1326-415:11840] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbbe504527e]
[fv-az1326-415:11840] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbbe50288ff]
[fv-az1326-415:11840] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbbe54a5ff5]
[fv-az1326-415:11840] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbbe54bb0da]
[fv-az1326-415:11840] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbbe54a5a55]
[fv-az1326-415:11840] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbbe54a5a6f]
[fv-az1326-415:11840] [ 8] plumed_master(+0x146dd)[0x563db85de6dd]
[fv-az1326-415:11840] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbbe502a1ca]
[fv-az1326-415:11840] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbbe502a28b]
[fv-az1326-415:11840] [11] plumed_master(+0x15365)[0x563db85df365]
[fv-az1326-415:11840] *** End of error message ***
</pre>
{% endraw %}
