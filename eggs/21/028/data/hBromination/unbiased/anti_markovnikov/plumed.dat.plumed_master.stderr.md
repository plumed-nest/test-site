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
[fv-az774-16:73116] *** Process received signal ***
[fv-az774-16:73116] Signal: Aborted (6)
[fv-az774-16:73116] Signal code:  (-6)
[fv-az774-16:73116] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fce2b442520]
[fv-az774-16:73116] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fce2b4969fc]
[fv-az774-16:73116] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fce2b442476]
[fv-az774-16:73116] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fce2b4287f3]
[fv-az774-16:73116] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fce2b8a2b9e]
[fv-az774-16:73116] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fce2b8ae20c]
[fv-az774-16:73116] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fce2b8ae277]
[fv-az774-16:73116] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fce2b8ae52b]
[fv-az774-16:73116] [ 8] plumed_master(+0x14274)[0x560d1bc2e274]
[fv-az774-16:73116] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fce2b429d90]
[fv-az774-16:73116] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fce2b429e40]
[fv-az774-16:73116] [11] plumed_master(+0x14ed5)[0x560d1bc2eed5]
[fv-az774-16:73116] *** End of error message ***
</pre>
{% endraw %}
