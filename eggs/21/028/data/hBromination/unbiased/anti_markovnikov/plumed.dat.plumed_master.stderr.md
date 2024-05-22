**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/anti_markovnikov/plumed.dat   
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
[fv-az1106-239:42670] *** Process received signal ***
[fv-az1106-239:42670] Signal: Aborted (6)
[fv-az1106-239:42670] Signal code:  (-6)
[fv-az1106-239:42670] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa8f1442520]
[fv-az1106-239:42670] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa8f14969fc]
[fv-az1106-239:42670] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa8f1442476]
[fv-az1106-239:42670] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa8f14287f3]
[fv-az1106-239:42670] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa8f18a2b9e]
[fv-az1106-239:42670] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa8f18ae20c]
[fv-az1106-239:42670] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa8f18ae277]
[fv-az1106-239:42670] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa8f18ae52b]
[fv-az1106-239:42670] [ 8] plumed_master(+0x14274)[0x563ae8b92274]
[fv-az1106-239:42670] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa8f1429d90]
[fv-az1106-239:42670] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa8f1429e40]
[fv-az1106-239:42670] [11] plumed_master(+0x14ed5)[0x563ae8b92ed5]
[fv-az1106-239:42670] *** End of error message ***
</pre>
{% endraw %}
