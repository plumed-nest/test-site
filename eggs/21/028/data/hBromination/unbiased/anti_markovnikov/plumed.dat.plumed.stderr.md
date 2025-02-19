**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/anti_markovnikov/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:263) void PLMD::Keywords::addFlag(const std::string&, bool, const std::string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1326-415:11822] *** Process received signal ***
[fv-az1326-415:11822] Signal: Aborted (6)
[fv-az1326-415:11822] Signal code:  (-6)
[fv-az1326-415:11822] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7b95045330]
[fv-az1326-415:11822] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7b9509eb2c]
[fv-az1326-415:11822] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7b9504527e]
[fv-az1326-415:11822] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7b950288ff]
[fv-az1326-415:11822] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7b954a5ff5]
[fv-az1326-415:11822] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7b954bb0da]
[fv-az1326-415:11822] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7b954a5a55]
[fv-az1326-415:11822] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7b954a5a6f]
[fv-az1326-415:11822] [ 8] plumed(+0x146dd)[0x5572a89276dd]
[fv-az1326-415:11822] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7b9502a1ca]
[fv-az1326-415:11822] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7b9502a28b]
[fv-az1326-415:11822] [11] plumed(+0x15365)[0x5572a8928365]
[fv-az1326-415:11822] *** End of error message ***
</pre>
{% endraw %}
