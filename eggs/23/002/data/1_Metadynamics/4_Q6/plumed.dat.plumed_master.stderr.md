**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/4_Q6/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action LOCAL_AVERAGE with label @s28 : cannot understand the following words from the input line : LOWMEM
[fv-az774-16:70460] *** Process received signal ***
[fv-az774-16:70460] Signal: Aborted (6)
[fv-az774-16:70460] Signal code:  (-6)
[fv-az774-16:70460] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f06f1e42520]
[fv-az774-16:70460] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f06f1e969fc]
[fv-az774-16:70460] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f06f1e42476]
[fv-az774-16:70460] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f06f1e287f3]
[fv-az774-16:70460] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f06f22a2b9e]
[fv-az774-16:70460] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f06f22ae20c]
[fv-az774-16:70460] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f06f22ae277]
[fv-az774-16:70460] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f06f22ae52b]
[fv-az774-16:70460] [ 8] plumed_master(+0x14274)[0x55cec1bbe274]
[fv-az774-16:70460] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f06f1e29d90]
[fv-az774-16:70460] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f06f1e29e40]
[fv-az774-16:70460] [11] plumed_master(+0x14ed5)[0x55cec1bbeed5]
[fv-az774-16:70460] *** End of error message ***
</pre>
{% endraw %}
