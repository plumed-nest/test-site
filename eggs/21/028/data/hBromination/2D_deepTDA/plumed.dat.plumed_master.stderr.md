**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/2D_deepTDA/plumed.dat   
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
[fv-az1326-415:11785] *** Process received signal ***
[fv-az1326-415:11785] Signal: Aborted (6)
[fv-az1326-415:11785] Signal code:  (-6)
[fv-az1326-415:11785] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2fca445330]
[fv-az1326-415:11785] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2fca49eb2c]
[fv-az1326-415:11785] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2fca44527e]
[fv-az1326-415:11785] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2fca4288ff]
[fv-az1326-415:11785] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2fca8a5ff5]
[fv-az1326-415:11785] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2fca8bb0da]
[fv-az1326-415:11785] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2fca8a5a55]
[fv-az1326-415:11785] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2fca8a5a6f]
[fv-az1326-415:11785] [ 8] plumed_master(+0x146dd)[0x5624943296dd]
[fv-az1326-415:11785] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2fca42a1ca]
[fv-az1326-415:11785] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2fca42a28b]
[fv-az1326-415:11785] [11] plumed_master(+0x15365)[0x56249432a365]
[fv-az1326-415:11785] *** End of error message ***
</pre>
{% endraw %}
