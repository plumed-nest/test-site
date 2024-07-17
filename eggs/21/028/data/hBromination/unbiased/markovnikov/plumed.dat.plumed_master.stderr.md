**Project ID:** [plumID:21.028]({{ '/' | absolute_url }}eggs/21/028/)  
Stderr for source:  hBromination/unbiased/markovnikov/plumed.dat   
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
[fv-az774-16:73160] *** Process received signal ***
[fv-az774-16:73160] Signal: Aborted (6)
[fv-az774-16:73160] Signal code:  (-6)
[fv-az774-16:73160] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe0a2c42520]
[fv-az774-16:73160] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe0a2c969fc]
[fv-az774-16:73160] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe0a2c42476]
[fv-az774-16:73160] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe0a2c287f3]
[fv-az774-16:73160] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe0a30a2b9e]
[fv-az774-16:73160] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe0a30ae20c]
[fv-az774-16:73160] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe0a30ae277]
[fv-az774-16:73160] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe0a30ae52b]
[fv-az774-16:73160] [ 8] plumed_master(+0x14274)[0x56247d8f9274]
[fv-az774-16:73160] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe0a2c29d90]
[fv-az774-16:73160] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe0a2c29e40]
[fv-az774-16:73160] [11] plumed_master(+0x14ed5)[0x56247d8f9ed5]
[fv-az774-16:73160] *** End of error message ***
</pre>
{% endraw %}
