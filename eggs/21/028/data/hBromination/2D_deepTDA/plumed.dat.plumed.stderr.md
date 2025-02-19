**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/2D_deepTDA/plumed.dat   
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
[fv-az1326-415:11767] *** Process received signal ***
[fv-az1326-415:11767] Signal: Aborted (6)
[fv-az1326-415:11767] Signal code:  (-6)
[fv-az1326-415:11767] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdcaa645330]
[fv-az1326-415:11767] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdcaa69eb2c]
[fv-az1326-415:11767] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdcaa64527e]
[fv-az1326-415:11767] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdcaa6288ff]
[fv-az1326-415:11767] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdcaaaa5ff5]
[fv-az1326-415:11767] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdcaaabb0da]
[fv-az1326-415:11767] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdcaaaa5a55]
[fv-az1326-415:11767] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdcaaaa5a6f]
[fv-az1326-415:11767] [ 8] plumed(+0x146dd)[0x55a7d98766dd]
[fv-az1326-415:11767] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdcaa62a1ca]
[fv-az1326-415:11767] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdcaa62a28b]
[fv-az1326-415:11767] [11] plumed(+0x15365)[0x55a7d9877365]
[fv-az1326-415:11767] *** End of error message ***
</pre>
{% endraw %}
