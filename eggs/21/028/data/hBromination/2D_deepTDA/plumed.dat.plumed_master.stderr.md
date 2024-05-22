**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/2D_deepTDA/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:211) void PLMD::Keywords::addFlag(const string&, bool, const string&)
+++ assertion failed: !def
the second argument to addFlag must be false COMPONENTS
[fv-az1106-239:42626] *** Process received signal ***
[fv-az1106-239:42626] Signal: Aborted (6)
[fv-az1106-239:42626] Signal code:  (-6)
[fv-az1106-239:42626] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f208be42520]
[fv-az1106-239:42626] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f208be969fc]
[fv-az1106-239:42626] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f208be42476]
[fv-az1106-239:42626] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f208be287f3]
[fv-az1106-239:42626] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f208c2a2b9e]
[fv-az1106-239:42626] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f208c2ae20c]
[fv-az1106-239:42626] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f208c2ae277]
[fv-az1106-239:42626] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f208c2ae52b]
[fv-az1106-239:42626] [ 8] plumed_master(+0x14274)[0x5585a8fc5274]
[fv-az1106-239:42626] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f208be29d90]
[fv-az1106-239:42626] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f208be29e40]
[fv-az1106-239:42626] [11] plumed_master(+0x14ed5)[0x5585a8fc5ed5]
[fv-az1106-239:42626] *** End of error message ***
</pre>
{% endraw %}
