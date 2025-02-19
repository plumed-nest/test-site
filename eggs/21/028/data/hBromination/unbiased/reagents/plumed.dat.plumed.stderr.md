**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/reagents/plumed.dat   
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
[fv-az1326-415:11934] *** Process received signal ***
[fv-az1326-415:11934] Signal: Aborted (6)
[fv-az1326-415:11934] Signal code:  (-6)
[fv-az1326-415:11934] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbe30445330]
[fv-az1326-415:11934] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbe3049eb2c]
[fv-az1326-415:11934] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbe3044527e]
[fv-az1326-415:11934] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbe304288ff]
[fv-az1326-415:11934] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbe308a5ff5]
[fv-az1326-415:11934] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbe308bb0da]
[fv-az1326-415:11934] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbe308a5a55]
[fv-az1326-415:11934] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbe308a5a6f]
[fv-az1326-415:11934] [ 8] plumed(+0x146dd)[0x55da8564f6dd]
[fv-az1326-415:11934] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbe3042a1ca]
[fv-az1326-415:11934] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbe3042a28b]
[fv-az1326-415:11934] [11] plumed(+0x15365)[0x55da85650365]
[fv-az1326-415:11934] *** End of error message ***
</pre>
{% endraw %}
